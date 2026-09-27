# Living World — positions, routes, and firing lanes

> **Archived 2026-09-27 — historical material, not current rules.** Setting references describe a removed setting. Use the repository’s `rules/` and `modules/` indexes for current material.

**Status:** tactical prototype, not tested rules · **Revised:** 2026-09-24  
**Owns:** battlefield geometry, movement budgets, occupancy, range, cover, engagement, and movement timing.

## 1. Design choice

The user wants a novel-feeling, precise movement system for frequent combat. Prototype a **position-and-route map**: characters occupy named tactical positions, move along explicit routes, and attack through separately defined lanes. A position might be the bridge crank, a truck's rear, a roof lip, or a flooded stair landing. It is a small physical foothold, not an entire room.

The tactical questions become: which route can I hold; where can I expose that target; can I reach the control before the gate shuts; who can cover my crossing? Changeable routes and directional protection give the map mechanical work to do.

This is a design direction, not a claim of historical originality. **C9 is an explicit local override:** tactical maps replace the base's estimated movement distances with route costs and printed range bands. Retain the labels Reach / Close / Far / Distant for effects; do not derive their legality from freeform descriptions or a second grid. Off-map travel still needs the base's transition procedure.

## 2. Map specification

Each encounter needs roughly **6–10 positions**, with enough distinct approaches to support a meaningful choice. More positions are justified only by more tactical decisions.

| Element | Required data |
|---|---|
| Position | ID, name, elevation, occupancy capacity, terrain/hazards, interactable objects, whether it is an escape endpoint. |
| Movement route | Endpoints, direction, Pace cost, size/access restriction, narrow/broad passage, route state, any crossing trigger and its safe stop. |
| Attack lane | Ordered source/target position pair; range band; sight; line of effect; directional cover; which methods differ. |
| Feature | Exact action needed to change it, TN if uncertain, state change, timing, and failure consequence. |
| Unit | Stable ID, position/footprint, occupancy size, current movement balance, engagement/control states. |

**Keep travel and attack geometry separate.** A ladder may be expensive to climb while the roof is an easy shot. A long detour around a wall does not make the straight shot legal. Never calculate firing range from the shortest walking route.

Every relevant pair needs an attack-lane entry or the packet-wide default **blocked**. Each same-position pair is Reach, subject to any explicit barrier. Reciprocal lanes may share range and visibility while granting different cover. A position large enough to contain different melee distances needs to be split.

## 3. Budget and route states

**Prototype budget: 2 Pace per cycle**, shared between opening and closing movement. Normal routes cost 1; difficult routes cost 2. Multiple difficult-terrain tags do not multiply that cost. No Pace carry-over, free movement from a Minor, or reset between stages.

**Drive — Major:** commit the Major at declaration to gain 2 additional Pace that cycle, maximum 4. This deliberately replaces the base's prohibition on a Sprint-like action within this optional module. It buys travel, not immunity to crossing threats, an extra attack, or guaranteed escape. Test its value against offensive and protective Majors.

| Route state | Exact meaning |
|---|---|
| Open | Pay its printed cost to traverse if access and capacity permit. |
| Contested | Traversable, but the named announced crossing/departure threat applies unless answered. No unspecified opportunity attacks. |
| Sealed | Cannot traverse until a listed action opens it. A high movement budget does not bypass a sealed route. |
| Unstable | Traversal has a listed check or timed condition, with exact success/failure endpoints and consequences. A traversal check consumes an entry Major; it is not a free third roll beside an attack and defense. |

Use intermediate exposed positions for long crossings; do not leave tokens “somewhere on the edge.” Any route that requires more than 2 Pace under ordinary conditions needs intermediate positions or must explicitly require Drive/another approved capability. Running out of movement is a reason not to begin that edge, not permission to invent a landing.

## 4. One cycle, explicit map snapshots

The [Combat Module](combat-module-plan.md) owns action commitments and damage. Its staged cycle uses these positions:

1. **Opening snapshot:** publish unit positions, rotating movement priority, enemy routes, threats, lane changes, and route state. Lock PC pre-route, action position, post-route, and one legal fallback before dice.
2. **Entry maneuvers:** resolve any declared Major specifically used to open a route, disengage, or enable this cycle's travel. It replaces that actor's main-stage Major. Grant a committed Drive budget here. No second Major later.
3. **Opening movement:** resolve locked routes in published unit priority. Apply crossing triggers and hazards immediately. A unit Downed here cannot perform a later action.
4. **Setup and action snapshot:** resolve setup actions from reached positions, then freeze the resulting map for simultaneous main actions and ordinary remaining threats. Recheck target legality now.
5. **Fallout snapshot:** this document owns the order: **harm → control and feature changes → forced movement → closing movement**. Within each category use published source priority; contradictory changes need a packet rule or a staff ruling before the dependent result proceeds. A unit valid at the action snapshot still gets its simultaneous action despite incoming harm there, subject to the last-Strain exception in Combat.
6. **Closing movement:** eligible units use their remaining Pace on their locked post-route. Downed units cannot move themselves. A route whose starting position changed needs its already declared fallback or is cancelled.

Movement priority is a published circular order of stable unit IDs, including monsters; move its first ID to the end each cycle. It resolves occupancy and crossing ties only, not attack initiative. Resolve each unit's route fully before the next within a stage. Joining units take a packet-defined place at the next briefing. Arrival order of Discord posts never changes priority.

For voluntary movement, validate the next edge and destination before charging its Pace. Once a legal crossing starts, charge the full edge cost and resolve its printed crossing trigger at the origin-side checkpoint; if interrupted, remain at that named origin unless the entry explicitly specifies another safe endpoint. On arrival, apply destination hazards. Cost-2 crossings remain atomic: no refund for interruption or invented halfway position. Fall/Downed outcomes must name an endpoint in the route entry. Forced movement uses §7 instead of this Pace charge.

An action can change terrain at its named stage. Opening a shutter during main actions cannot retroactively unblock another attack in the frozen action snapshot; opening it as setup can. Effects specify whether they occur as entry, setup, main, or fallout. A player cannot move an action to an earlier stage after seeing another roll.

## 5. Occupancy, engagement, and transport

- A normal PC occupies 1 capacity; packet cards state larger footprints and which positions they occupy. A large creature remains one entity with one Resistance track. No automatic double hits from occupying several positions.
- Entering a hostile-occupied position is possible only if capacity permits and the declared route allows entry. It creates Reach contact and resolves any already announced entry threat. Monsters cannot add a free attack simply because someone approached.
- Full positions block arrival. Players may predeclare an allied swap; resolve it as one transaction when both routes, budgets, permissions, and capacities are legal. Hostile swaps and unannounced pass-throughs are unavailable.
- A narrow route admits no opposing hostile traversals in the same movement stage. The first legal crossing in published priority reserves its direction for that stage; a contrary mover stops before the edge or uses their locked fallback. A broad route permits opposing passage unless its printed threats or endpoint capacity stop it. This is an explicit scheduling abstraction, not simultaneous midpoint combat.
- A losing claim on capacity stops at the last legal position or takes its locked fallback. No free shove, collision damage, or refund for edges already travelled. Untraversed edges cost nothing.
- Engaged means a named hostile threatens departure from that Reach position. The threat must identify the departure route(s), trigger, response, and consequence, and count against the monster's threat budget. Engagement alone generates no extra attacks.
- **Disengage — Major:** resolve its declared protection against named departure threats before moving. Publish which threats it covers; success permits the declared route without those threats, while movement still costs Pace. A reserved Minor defense answers only one threat and cannot retry a failed Major against it.
- A Downed body still occupies capacity. Picking up a willing/Downed casualty costs a Minor at Reach; carrying combines their occupancy and makes normal routes cost 2 Pace unless a card says otherwise. Size/access limits still apply. Putting them down costs a Minor and requires capacity. Rescue under fire may require a Major addressing the threat as well.

Carry, push, or exchange choices cannot create an extra action for the passenger. Unwilling PC transport requires the agreed PvP procedure; creature grappling needs an approved maneuver.

## 6. Lanes, cover, and areas

Check **identified target → sight → line of effect → range → protection** independently. A known target behind smoke is different from a target behind concrete. A weapon or Domain entry must state any method that bypasses a particular restriction.

**Prototype cover rule:** a lane giving the target partial cover adds +2 to a PC's attack TN; an incoming threat through a lane protecting the PC reduces its response TN by 2. Full protection blocks that attack method. It does not become Armor, cancel an unrelated hazard, or protect a route crossing automatically. Two cover sources do not stack.

For a combined attack/protective action use Combat's higher-of-two-adjusted-TNs rule. Example: attack TN 15 becomes 17 against cover; threat response TN 20 becomes 18 with the defender's cover; the combined TN is 18. Do not cancel the adjustments or also add a defense bonus. Setup bonuses remain separately capped under Combat. Print the resulting TN before dice.

**Angles replace a universal flanking bonus:** reaching another position can provide a clear lane around the target's directional cover or access an exposed creature seam. That permission is the advantage; no automatic +2 merely for approaching from another side.

An area effect names its exact affected position IDs and/or crossing routes before rolling. An origin and propagation rule must be printed on the effect; adjacency alone does not spread it through closed doors. Resolve main-stage occupants from the action snapshot; entry hazards use traversal time. A target occupying several affected positions is exposed once to the same effect per cycle.

Every area entry also has a maximum footprint/scale, and the map marks which listed position groups fit it. A whole courtyard cannot count as one small foothold, and a “two-position” effect cannot join two distant rooftops. Canonical packet authors approve footprints before play; a runner cannot stretch an area by renaming locations.

Allied occupants are included unless the effect is explicitly selective. If potential friendly harm falls outside the affected players' agreed stakes, choose a legal different effect/area before commitment or pause for agreement. Consent never appears automatically because a template includes an ally.

## 7. Forced movement and special traversal

Forced-movement effects specify origin requirements, permitted direction/path, maximum number of route steps, legal destinations, and whether a particular sealed route can be breached. Choose the path before the roll. A push does not inherit Drive's budget or the target's voluntary movement allowance.

Resolve multiple pushes in published source priority, checking each from the resulting position. If an earlier push invalidates a later locked path's origin, use its predeclared alternative or cancel that displacement; never translate the path silently. An attack that already resolved is not refunded. Stop before a sealed route or capacity conflict unless the effect explicitly breaks it. No default chain-pushing, wall damage, falling, or lethal collision. Forced movement can expose someone to a printed hazard; it does not trigger voluntary departure attacks unless their threat explicitly includes it.

Ladders, climbs, jumps, water crossings, and elevation changes are route entries, not universal improvised distance contests. Print cost, hands/tools, legal arrival, and failure endpoint. A failed jump cannot acquire a fatal fall consequence that was never disclosed. Flight/teleportation needs an approved effect defining which graph restrictions it bypasses; naming that power does not grant unrestricted access to every position.

Hazards use one effect ID: entering, being pushed through, and finishing in that same hazard do not charge it repeatedly in one cycle. Distinct overlapping hazards need the approved combined-exposure rule. Leaving the encounter requires a printed escape endpoint and its pursuit conditions; reaching the edge of the diagram is insufficient.

## 8. Small worked map

**Test fixture:** all positions capacity 2, all units size 1. Routes are bidirectional unless shown otherwise.

~~~mermaid
graph LR
    A["A · Truck Rear"] ---|1 Pace| B["B · Chain Winch"]
    B ---|1 Pace| C["C · Bridge Crank"]
    C ---|"1 Pace · SEALED"| E["E · Refuge"]
    A ---|2 Pace| D["D · Roof Lip"]
    D ---|1 Pace| B
~~~

| Relevant attack lane | Range | Sight/effect | Cover |
|---|---|---|---|
| A → C | Far | Clear | C has partial cover from A. |
| D → C | Far | Clear | No cover: the elevated angle bypasses C's barricade. |
| A → B / B → A | Close | Clear | B has none from A; A has partial from B. |
| A ↔ D | Close | Clear | Neither protected. |
| B ↔ D | Close | Clear | Neither protected. |
| B ↔ C | Close | Clear | Neither protected. |
| C → A | Far | Clear | A has partial cover from C. |
| C → D | Far | Clear | Neither protected. |

Every other unlisted cross-position shot is blocked for this fixture; same-position Reach remains legal. E is an escape endpoint only when the bridge route is opened by its scenario action, which also opens a clear Close lane C↔E. Drawing a link to E does not unlock it.

Vey starts A with 2 Pace and an approved test weapon effective at Far; this example grants no extra Domain range. Their declaration is **opening A→D (2); shoot C from D; no closing movement**. The clear D→C lane removes the barricade's protection, but Vey must spend all movement reaching it. They cannot shoot from D and claim to end behind the truck.

Mara starts B. Their declaration is **opening B→C (1); operate crank at C; closing C→B (1)**. A location-locked threat against C resolves while Mara acts there; retreat afterward cannot erase it. If fallout pushes Mara from C to A, the C→B retreat is invalid unless an A-origin fallback was already declared and affordable.

In a separate capacity test, C already holds one size-1 defender and another size-1 unit arrives before Mara, filling its capacity of 2. Mara then stays B or uses the locked fallback; the crank action cannot reach C. Its Major remains committed, but an effect that never legally begins consumes no activation resource. The packet's closing-movement and remaining-Pace rules still apply.

## 9. Reproducibility gate

Two independent authorised runners must resolve identical locked inputs to identical position IDs, legal lanes, costs, triggers, and harm. Include: contested capacity, opposing narrow-route travel, allied swap, entry-stage Downed, interrupted cost-2 traversal, exhausted Pace, altered route origin, setup-created cover, main-stage closed door, target leaving a lane, branching pushes, carried casualty, a jump without a landing, an area containing an ally, and a hazard crossed twice.

Test the same encounters with straight attack, route control, reposition-and-fire, rescue, Drive, and retreat plans. Keep the model only if positioning changes worthwhile choices without producing recurring geometry disputes. Initial target: map comprehension within five minutes, movement resolution within five minutes per cycle, and no private runner judgment needed for printed interactions.
