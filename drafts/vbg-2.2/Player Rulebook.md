# Very Basic RPG 2.2 — Player Rulebook

**Status:** working draft · **Revised:** 2026-09-24  
**Owns:** shared player-facing mechanics — resolution, character creation, scenes, perception, abilities, harm, inventory, and progression.

> A working draft does not replace a published rule until approved. Anything marked pending is not playable; see the [Decision Log](Decision%20Log.md).

## 1. Start here

VBG is an asynchronous, fiction-first RPG. Players declare what their characters attempt; the GM presents the situation, risks, and threats, then resolves uncertain outcomes.

Use this book to create a character and play scenes. The [GM Guide](GM%20Guide.md) explains adjudication, while the [Creature Blueprint](Creature%20Blueprint.md) and [Item Glossary](Item%20Glossary.md) supply creature and item details.

### Key terms

This list is the single definition of each term. Later sections use them without redefining them.

| Term | Meaning |
|---|---|
| **Scene** | A contained situation with shared stakes. It ends when those stakes resolve and no threat presses the group. A threat scene uses the resolution cycle in §4. |
| **Cycle** | One GM scene post, up to 24 hours for player posts, then one GM resolution. The cycle is the only unit of time inside a scene: VBG has no round and no turn. It is also one resolution round for ongoing hazards and sustained effects. |
| **Declared Action** | The single specific thing a player states their character attempts in a post, with its intended outcome. It is what a roll resolves and what a cost or consequence attaches to. |
| **Stat** | Force, Finesse, or Focus. See §3. |
| **Trait** | A Major Trait (+2) or Minor Trait (+1) describing who the character is. |
| **Ability Domain** | A GM-approved sphere of effect the character can produce by spending Strain. See §5. |
| **Major Action / Minor Action** | The actions available in each player post. Free Actions are negligible extras. See §4. |
| **Conditional response** | A single "if X, then Y" declared in the post, which spends the Minor Action if it triggers. See §4. |
| **Target Number (TN)** | The difficulty a roll must meet. See §2. |
| **Strain** | A character's capacity to use abilities and absorb harm. |
| **Armor** | Boxes that absorb physical damage before Strain. |
| **Downed** | At 0 Strain. The character has taken an Injury and is on a deadline. See §6. |
| **Injury** | A named Condition inflicted by going Downed, with a stated practical effect. See §6. |
| **Engaged** | Something within Melee / Reach is actively pressing the character. See §4. |
| **Awareness** | What a creature currently knows about the characters: Unaware, Searching, or Aware. See §4. |
| **Noise Clock** | A 0–6 track per area, measuring how much attention the area has drawn. See §4. |
| **Resistance** | A creature's single defeat track. See §4. |
| **Progression Point (PP)** | The award spent on character upgrades. See §8. |

## 2. Core resolution

### Declare the action

State the intended outcome and, when acting independently, an appropriate Target Number (TN) before rolling.

The GM may reject a proposed TN **that does not fit the fiction, whether it is too low or too high**. This is the single veto standard in VBG, and the same standard covers a Trait the player claims is relevant when it is not.

Roll when an action attempts to force an outcome on another creature or when its outcome is uncertain. Producing an ability's approved effect alone does not require a roll; uncertain aim, timing, or control in using that effect does. Helping a willing recipient does not by itself require a roll, though uncertain circumstances can.

### Roll

`1d20 + relevant Stat + applicable Trait bonus`

- Add Force, Finesse, or Focus.
- Add one relevant Major Trait (+2) and one relevant Minor Trait (+1) at most.
- **The player asserts which Traits are relevant** in the post, subject to the veto standard above.
- The GM states a TN where one is known; otherwise, the player proposes it before rolling.

| TN | Difficulty | Example |
|---:|---|---|
| 10 | Routine | A low-pressure task with ordinary obstacles. |
| 15 | Risky | Combat, stealth, or a pressured action. |
| 20 | Desperate | A life-or-death maneuver or precise high-risk feat. |
| 25+ | Extreme | An extraordinary feat against a major threat or impossible conditions. |

Combat is TN 15 unless the fiction says otherwise.

### Resolve the result

| Margin | Outcome | Result |
|---|---|---|
| Miss by 5+ | Failure | The action fails and the situation worsens. |
| Miss by 1–4 | Success with Cost | The action succeeds with a meaningful cost. |
| Meet TN to beat it by 5 | Clean Success | The action succeeds without an added cost. |
| Beat TN by 6+ | Critical Success | The action succeeds and gains a meaningful advantage. |

For **Success with Cost**, the player proposes a cost suited to the stakes: a narrative consequence, Strain loss, Armor spent absorbing damage, or a resource spent. The GM may reject a cost that is too mild or does not fit. A cost:

- never kills the character,
- never touches another player's character or property without that player's agreement,
- never exceeds what the action stood to gain.

For a **Critical Success**, the player chooses a fitting narrative advantage or something gained through the situation. A critical:

- never adds damage — nothing in VBG deals more than 1 (§6),
- never grants a second action,
- never exceeds what was declared.

A Clean Success grants the declared objective but no automatic critical benefit.

On **Failure**, the player narrates a meaningful consequence. The GM resolves it when it is unclear, too mild, or relies on hidden information. Failure does not grant an additional reaction roll.

## 3. Create a character

1. Set Force, Finesse, and Focus to **−1**, then allocate **6 points** among them. All 6 points are spent, no Stat can exceed **+2** at creation, and no Stat can be reduced below −1 to buy points elsewhere.
2. Choose **one Major Trait (+2)**: an archetype, profession, or defining identity.
3. Choose **one Minor Trait (+1)**: a skill, habit, background, or secondary edge.
4. Choose one GM-approved Ability Domain. Define in one sentence what it controls. The approval standard, with accepted and rejected examples, is in [GM Guide](GM%20Guide.md) §3.
5. Record **4 Strain**, **no Armor**, and **4 Inventory Slots**.
6. Choose at most **two starting items** from the Major Trait or backstory. The count is based on items, not slot cost; a kit counts as one item only if its contents are defined. Starting gear cannot include Armor, which is Restricted or Rare — see [Item Glossary](Item%20Glossary.md) §2.

Legal spreads include +2 / +2 / −1, +2 / +1 / 0, and +1 / +1 / +1. The +2 / +2 / −1 spread spends exactly 6 and is intended: a specialist with a real hole in them.

Traits are fiction-first, and no trait catalog is required to play. A setting module may supply one; see its own document set.

| Stat | Covers |
|---|---|
| **Force** | Physical power, endurance, intimidation, lifting, melee, and resisting harm. |
| **Finesse** | Agility, speed, stealth, precision, aim, and manual dexterity. |
| **Focus** | Perception, knowledge, technical work, composure, and mental resilience. |

### Example character

> **Vey, street alchemist**
>
> **Stats:** Force **+1**, Finesse **+2**, Focus **0**. Starting from −1 in each, that spends 2, 3, and 1 of the 6 points, and no Stat exceeds +2.  
> **Major Trait (+2):** Street Alchemist — mixes and handles volatile compounds for a living.  
> **Minor Trait (+1):** Dockhand — years of hauling cargo along the river wharf.  
> **Ability Domain:** Flame — shapes and directs open fire that already burns or that Vey kindles by hand.  
> **Strain:** 4 · **Armor:** none · **Inventory:** 4 slots.  
> **Starting items:** a coil of rope (1/2 slot, Silent) and an oil lantern (1/2 slot, Silent, and a light source that announces you) — both drawn from the Dockhand background. See [Item Glossary](Item%20Glossary.md) §6.
>
> Throwing a burst of flame at a target uses Finesse for aim, +2 for Street Alchemist, and no Minor Trait, since Dockhand does not apply: `1d20 + 2 + 2`.

## 4. Play a scene

### Actions and posts

During an active scene, each player post includes one Major Action, one Minor Action, movement, and any conditional response. It may also include Free Actions.

| Major Action | Minor Action |
|---|---|
| A Declared Action performed, with or without intent of harm | Draw or put away an item |
| Use a 1–2 Strain ability | Use a small 0-Strain utility ability |
| Escape by dedicating the action to getting away | Open an ordinary unlocked door |
| Perform substantial treatment, or stabilize a Downed character | Hand an item to someone within reach |
| Force, repair, or manipulate something under pressure | Briefly interact with an accessible object |
| Assist another character's roll | Trigger a declared conditional response |

A Minor Action can require a roll if uncertain; a roll does not itself make it a Major Action. Free Actions include brief speech, dropping a carried item, and negligible actions that create no meaningful advantage. The GM can reclassify an action with meaningful time, risk, or effect.

**An omitted part of a post is forfeited.** A post that declares a Major Action but no movement simply does not move. There is no query and no default; the missed-window default below applies to silence only.

### Conditional responses

A post may carry **one** conditional response: a single stated "if X, then Y".

- Declaring it is free. It costs nothing if it never triggers, and it lapses at the end of the cycle.
- When it triggers, it **spends the Minor Action**. A post that already spent its Minor Action elsewhere cannot also trigger a conditional.
- It resolves in the cycle it was declared in, at step 3 below.
- It may not be a Major Action, an attack, or a 1–2 Strain ability. A conditional is a guard, a shove, a grab, a door, a 0-Strain effect — not a second attack.

### Resolution cycle

1. The GM posts the current scene, threats, stakes, known TNs, the area's Noise Clock, and each creature's awareness.
2. Players have up to 24 hours to post their actions and rolls.
3. The GM resolves all outcomes together, updates the scene, and begins the next cycle.

Everything in a cycle resolves in this order:

| Step | Resolves |
|---:|---|
| 1 | **Movement** — all declared movement, in the fiction established by the last GM post. |
| 2 | **Actions and threats together** — every Declared Action and every creature threat, simultaneously. |
| 3 | **Conditional responses** — those whose trigger actually occurred. |
| 4 | **Consequences** — damage, costs, injuries, hazards, clocks, and position updates. |

Three consequences of that order:

- **All hits land.** If two characters both hit a creature with 2 Resistance in one cycle, both hits land, the creature falls, and the excess is wasted. Damage is never redirected to another target.
- **A character Downed during a cycle still resolves the action they declared.** Being Downed is a step-4 consequence.
- **Post order is not initiative.** It settles nothing except two declarations that genuinely cannot both be true, such as two characters claiming the same single handhold.

One roll can resolve an action and an incoming threat when the action addresses it, such as shoving away an attacker. An unrelated action does not automatically protect the character.

If a player misses the window, their character takes cover or follows the group where possible. **This default does not apply to a Downed character**, who does nothing at all while their deadline keeps running (§6). The GM does not spend scarce resources without prior permission; unavoidable consequences still apply.

### Answering a threat

Creatures do not roll. A threat is announced with its reach and its unresolved consequence, and a character has exactly three answers:

1. **Address it with the Major Action** — the Declared Action meaningfully deals with the threat, and one roll resolves both.
2. **Answer it with a conditional response** — if it was declared, it triggers, and it spends the Minor Action.
3. **Take the consequence.**

**A threat never grants a defensive roll.** A creature card's **Response / TN** field is the difficulty of a *suggested answering action*, not a save. Nothing is rolled by simply being attacked.

### Movement and distance

VBG uses fictional distance bands rather than a grid.

| Band | Distance | Use |
|---|---:|---|
| **Melee / Reach** | 0–5 ft | Touching, grappling, hand-to-hand combat. |
| **Close / Room** | 5–20 ft | A room, small office, or short corridor. |
| **Far / Hallway** | 20–60 ft | A long hallway, street section, or warehouse floor. |
| **Distant / Line of Sight** | 60+ ft | A plaza, rooftop, highway, or similarly broad space. |

- Name an origin and destination for each movement declaration.
- Movement accompanying an action reaches up to Close / Room along the actual route. Staying in one room does not allow unlimited back-and-forth travel.
- There is no Sprint action or purchasable extra movement allowance.
- Terrain, pursuit, encumbrance, conditions, and obstacles can restrict movement.
- Crossing an unobstructed room without danger does not require a roll.
- Long-distance travel uses a **Transition Scene**; see §4 *Scenes without threats*.

### Engagement

**Engaged** means something within Melee / Reach is actively pressing the character — attacking, grappling, blocking, or holding them in place. It is a state the GM states in the scene post, not a thing a player declares.

- Accompanying movement **cannot leave the band** while engaged. Walking away from an engaged enemy is not movement; it is an Escape.
- Being engaged does not prevent acting. It restricts where the character can be at the end of the cycle.

### Escape

Escape costs a **Major Action** dedicated to getting away.

| Situation | TN |
|---|---:|
| Not engaged; running before anything closes | 10 |
| Engaged by one threat | 15 |
| Engaged by several, or the route out is cut off | 20 |

- **Success** puts one band between the character and everything that was engaging them.
- **A second consecutive successful Escape** takes them out of the scene entirely.
- **Success with Cost** still escapes; the cost is paid from the usual list — dropped gear, a Strain, a worse position for someone else.
- **Failure** means still engaged, and the GM applies the situation's consequence.

Escape is not a movement multiplier and grants no extra distance beyond the band stated above.

### Pursuit

When something chases a character who did not break away:

- **A pursuer closes one band per cycle** unless something holds it off — a hazard, a blocked route, a successful answering action.
- **Two consecutive cycles at greater distance loses it.** The pursuer gives up, loses the trail, or is simply left behind.

### Cover

Cover is stated by the GM as part of the scene. Because creatures never roll, **cover buys action economy, not difficulty.**

| State | Effect |
|---|---|
| **None** | Threats apply normally. |
| **Partial** | Answers **one ranged threat per cycle** with a Free Action. A second ranged threat in the same cycle must be addressed or taken normally. |
| **Full** | Ranged threats cannot reach the character at all — and the character cannot make ranged attacks out of it. Leaving full cover to attack is part of the Declared Action. |

Taking cover is ordinary movement when cover is within reach of it.

### Awareness

Every creature is in one of three states toward the characters, **stated openly in the scene post**. None of it is hidden information.

| State | Meaning |
|---|---|
| **Unaware** | Does not know anyone is there. |
| **Searching** | Knows something is there; does not know where. |
| **Aware** | Knows where, and acts on it. |

- Awareness **rises one step** when a creature sees, hears, or is hit by a character — which of those apply is decided by the creature's **Senses** field ([Creature Blueprint](Creature%20Blueprint.md) §3).
- Awareness **falls one step** after a full cycle with nothing to find.
- **Acting against an Unaware target resolves one outcome band better** — a Failure becomes a Success with Cost, a Clean Success becomes a Critical. It never deals more damage, because nothing does.

### Light

| State | Effect |
|---|---|
| **Lit** | Normal. |
| **Dim** | Sight-dependent targeting treats the target as **one band further away**. |
| **Dark** | Sight is removed past Melee / Reach, in both directions. |

A carried light source fixes the problem and announces the carrier: it raises the awareness of anything that hunts by sight and can see it.

### Noise

Every action carries a noise rating. Items carry one too; see [Item Glossary](Item%20Glossary.md) §1.

| Rating | Ticks | Examples |
|---|---:|---|
| **Silent** | 0 | Moving carefully, a blade, a bow, quiet speech. |
| **Quiet** | +1 | An ordinary scuffle, forcing a wooden door, a failed attempt to move unseen. |
| **Loud** | +2 | Gunfire, breaking through a wall, shouting for help, an explosion. |

Each area runs a **Noise Clock from 0 to 6**. The GM states it in every scene post; it is never hidden.

| Clock | What it means |
|---:|---|
| **0** | Nothing has drawn attention. |
| **1–3** | Ambient stirring. Something distant has noticed the area. |
| **4–5** | Something is actively searching the area. **+2 TN to move unseen.** |
| **6** | It arrives. The GM introduces the threat the area has been building toward, then **resets the clock to 1**. |

**Decay:** −1 per cycle in which nothing above Silent occurs, and −1 on leaving the area for a new one without pursuit. It never drops below 0, and leaving and re-entering repeatedly does not farm reductions.

**One clock per scene.** A setting module may add its own noise *triggers* — a calibre table, a rating on a piece of local equipment — but it never runs a second clock alongside this one.

### Moving unseen

Moving unseen is an ordinary Declared Action, not a subsystem.

| Conditions | TN |
|---|---:|
| Good cover, darkness, or a distracted watcher | 10 |
| Ordinary conditions | 15 |
| Open ground, alert watchers, or carrying something awkward | 20 |

- **+2 TN** while the area's Noise Clock is at 4 or higher.
- **Failure** ticks the clock +1 and raises the nearest creature's awareness one step.
- **No roll is needed at all** in Dark or full cover against a creature whose Senses are sight-based — its Senses field decides, not the player's hopes.

### Assist

Spend a **Major Action** to give another character's roll **+1**. One assist per roll; assists do not stack. The assisting character must be able to plausibly help, in reach and in fiction.

### Threats and creature defeat

Creatures do not roll attack dice. They present threats, attacks, hazards, and pressure that require player responses. The GM resolves failed player rolls through the normal outcome rules, without an extra reaction roll.

Creatures use **Resistance boxes** as one defeat track. Each 1 damage removes 1 box; removing the last box defeats the creature without a finishing hit. Defeat may mean incapacitation, surrender, retreat, or death according to the declared action and situation. Fictional solutions can also overcome a creature.

Resistance is a creature's overall staying power, including protection. It is not player-style Armor: even unarmored creatures have it, and it never becomes scrap. Creature conditions apply before removing Resistance; a successful roll does not itself bypass an immunity or special defeat condition.

### Scenes without threats

Investigation, negotiation, downtime, and travel are **deliberately freeform**. They use the resolution rules in §2 and nothing else: no cycle, no action economy, no post order. The GM sets a posting rhythm to suit the table.

The perception layer still applies where it matters — the Noise Clock keeps running in an area, awareness still rises and falls, and light still restricts what can be seen.

**Transition Scene.** Long-distance travel that is too long or too routine to run cycle by cycle resolves as a Transition Scene.

1. The GM states the route, roughly how long it takes, and breaks it into **one to three legs**. Each leg gets exactly one obstacle: terrain, a checkpoint, weather, a stretch that has to be crossed quietly.
2. Each leg takes **one roll**. Either every character rolls, or one character rolls for the group with assists (§4) from the rest — the GM says which before rolls are made.
3. Resolve each leg by the ordinary outcome table.
   - **Clean Success or better:** the leg is crossed with resources intact.
   - **Success with Cost:** crossed, having spent something real — a consumable, a use of an item, 1 Strain, extra time, or a Condition.
   - **Failure:** the GM either delays the group, puts them somewhere other than where they meant to be, or **converts the leg into a threat scene**, which then runs on the cycle as normal.
4. **Noise carries, position does not.** Arriving at a new area without pursuit starts its clock one lower than the fiction would otherwise set, minimum 0. Nothing about the previous area's position, cover, or engagement carries over.
5. Catch Your Breath is available at the end of a Transition Scene; Full Rest is available only if the destination is actually safe.

A Transition Scene never awards PP by itself. Getting somewhere is not an accomplishment; what happened on the way might be.

## 5. Use abilities

An Ability Domain is open-ended within its approved scope, but cannot produce miraculous or unlimited effects. No ability exceeds Major scale.

| Scale | Strain cost | Scope |
|---|---:|---|
| **Minor-scale ability** | 0 | A small effect on one object or tightly limited spot. |
| **Standard-scale ability** | 1 | A substantial effect on one target or small cluster. This includes a **targeted attack on a single creature**. |
| **Major-scale ability** | 2 | A significant effect across one Close / Room-sized area. |

- Pay the listed Strain to produce an approved effect. **Costs measure scale, not damage.** A 2-Strain ability and a punch both deal 1 damage (§6).
- A 1–2 Strain ability uses a Major Action. A small 0-Strain utility ability may use a Minor Action. Attacks always use a Major Action, even at 0 Strain.
- Ability scale and action type are separate. Any roll resolves within the action and does not consume another action.
- You may spend your last Strain. Resolve the ability and attached roll, then become Downed. You cannot spend more Strain than you have, and Armor cannot pay ability costs.
- Default reach is Close / Room. Longer reach needs explicit Domain approval.
- Instant effects resolve immediately.
- Mundane lasting consequences, such as an object catching fire, follow the situation rather than ending automatically with the ability.

### Sustained effects

A sustained effect **spends the matching action type every later cycle** to maintain — a Major-scale effect costs a Major Action each cycle, and this never drops to a Minor or Free Action. No further Strain is spent.

Consequently:

- A character sustaining a Major-scale effect has no Major Action left and cannot attack, Escape, assist, or stabilize while sustaining it.
- **One character cannot sustain two effects of the same action type**, because they have only one of each action.

A sustained effect ends when released, interrupted, or when the user is Downed.

### Hazards and indirect effects

Creating a hazard costs only the ability's Strain. Placing or timing it to directly catch a creature requires a roll. Creatures entering an established hazard suffer its effects.

Creating a hazard in a creature's path does not guarantee it enters. The GM follows the creature's behavior and situation: it may stop, route around it, or push through. Creatures do not roll to make this choice. Describing an attack as environmental does not bypass the roll requirement.

Damaging hazards deal **1 damage to each exposed creature per cycle**, unless a rule states otherwise. Entering and remaining in the same hazard do not cause separate damage twice in that cycle, and **overlapping hazards deal 1 damage in total per cycle, not 1 each**.

| Intent | Cost | Resolution |
|---|---|---|
| Produce a handful of flame. | Minor scale: 0 Strain. | No roll to produce it. |
| Throw that flame precisely at a creature. | Standard scale: 1 Strain. | Major Action and roll for the targeted attack. |
| Tip a jar onto someone's head with a small gale. | Minor scale: 0 Strain. | Major Action and roll; indirect damage still forces an outcome. |
| Move that jar across an empty table. | Minor scale: 0 Strain. | No roll if there is no uncertainty. |
| Raise flame pillars ahead of approaching enemies. | Major scale: 2 Strain. | No roll to create the hazard; creatures respond to it. |
| Raise flame pillars beneath enemies. | Major scale: 2 Strain. | Roll to catch them. |

## 6. Harm and recovery

### Damage and Armor

- A hit deals **1 damage**. Nothing raises it: not ability scale, not a Critical Success, not a weakness, not a weapon, not a called shot. Weapons grant effects, never damage — see [Item Glossary](Item%20Glossary.md) §3.
- **All damage is physical unless the rule dealing it says otherwise.** Fire, force, cold, and open-ended Domain effects are physical, and Armor absorbs them.
- Armor absorbs physical damage first: spend 1 Armor box for each 1 damage. Remaining damage reduces Strain by the same amount.

### Downed, Injury, and death

At 0 Strain, a character is **Downed**. In the same post, the GM does three things:

1. States that the character is Downed.
2. **Names the Injury** the harm caused, with its practical effect — *Injured Leg: movement is restricted by the injury*.
3. **Announces an in-fiction treatment deadline** based on that injury and the danger around them. The 24-hour posting window is never that deadline.

Being Downed is how this game hurts people. **It is not how it kills them.**

| Event | Result |
|---|---|
| **Further hits** on a Downed character | The Injury worsens. They do not kill. |
| **The deadline passes untreated** | The Injury becomes **Lasting** until properly treated. The character does not die of neglect. |
| **A Downed player misses their posting window** | The character does nothing. The take-cover default does not apply, and the deadline keeps running. |

**Stabilization** is a **Major Action within Melee / Reach**: automatic with medical supplies, TN 10 without. It stops the deadline. A stabilized character is conscious at 0 Strain and may speak, take Free Actions, and crawl within their band. They cannot take a Major or Minor Action, and the Injury remains.

**Death requires one of exactly two things**, and nothing else:

- **A stated killing.** A creature card whose action says it kills, or an attacker declaring a killing blow on a helpless character.
- **An announced lethal danger.** Drowning, a long fall, a fire with no exit — announced as lethal by the GM *while it can still be avoided*.

An ordinary blow is never converted into a death after the fact. **No player character dies at another player character's hands without that player's agreement.**

### Conditions

Conditions primarily represent traumatic injuries. Name the injury and its practical effect. Ordinary Strain recovery does not remove injuries; treatment does — see [Item Glossary](Item%20Glossary.md) §4.

### Recovery and repair

- **Catch Your Breath:** recover 1 Strain after a threat ends, once per scene, by the scene definition in §1.
- **Full Rest:** recover all Strain after roughly eight safe hours. It does not remove an Injury.
- **Medical Aid:** consumables restore Strain and treat Injuries; values and requirements are in [Item Glossary](Item%20Glossary.md) §4.
- **Armor Repair:** restore 1 Armor box with safety, tools, one appropriate material unit, and roughly one hour. See [Item Glossary](Item%20Glossary.md) §7.
- **Broken Armor:** when all boxes of an Armor item are spent, it becomes scrap. Rebuilding scrap is crafting — see [Item Glossary](Item%20Glossary.md) §8.

### Healing abilities — Strain Transfer

This procedure applies only to Strain-healing abilities.

1. The healer spends a Major Action and transfers Strain to a recipient at 1:1. Each 1 Strain restored costs the healer 1 Strain.
2. This is the activation cost, not an added charge. A Major Action transfers at most **2 Strain**.
3. A willing recipient needs no roll unless circumstances are uncertain.
4. The healer may spend their last Strain, completing the transfer before becoming Downed.

**Strain Transfer may target a Downed character.** The first 1 Strain transferred ends the Downed state and stops the deadline. It does **not** remove the Injury, which still needs treatment.

Maintaining an effect cannot create further free Strain.

## 7. Inventory and equipment

Items take **1**, **1/2**, or **1/4** Inventory Slot. Fractions consume actual capacity per item or explicitly defined stack. Worn Armor occupies 1 slot.

- Gear grants practical capabilities or benefits. A numerical bonus must be explicitly listed in its rule.
- Containers organize existing slots; they never add capacity beyond PP upgrades.
- Every item entry — stacking, kit contents, uses, weapon effects, Armor values, healing supplies, materials, and noise ratings — lives in the [Item Glossary](Item%20Glossary.md).
- There is no currency. Items are obtained through the four acquisition paths and three value bands in [Item Glossary](Item%20Glossary.md) §2.

## 8. Progression

The GM awards Progression Points (PP) for missions, meaningful roleplay, discoveries, survival, and campaign milestones.

### Awards

Award PP **per session or per completed arc of play, to every player equally** — never per cycle, never for damage dealt, and never as a prize for one player's post.

| Award | For |
|---:|---|
| **+1 PP** | Surviving a threat scene that genuinely risked something. |
| **+1 PP** | Resolving a dangerous situation without violence where violence was the obvious route. |
| **+1 PP** | A discovery that changes what the group knows or can do. |
| **+1 PP** | Meaningful roleplay: acting on a Trait, Domain, or obligation at real cost. |
| **+2 PP** | Completing a mission, contract, or stated objective. |
| **+3 PP** | A campaign milestone. |

A typical session awards **2–5 PP**. At that rate a new Minor Trait arrives every session or two, and a third Ability Domain is the work of several months. Awarding much faster makes the upgrade costs below meaningless; awarding much slower makes progression invisible.

PP is not currency and is never spent on fiction, items, information, or favours. It buys the upgrades in the table and nothing else.

### Upgrades

| Upgrade | Cost | Limit |
|---|---:|---|
| +1 maximum Strain | 10 PP | Maximum 10 Strain |
| New Minor Trait | 5 PP | No ownership cap; one relevant Minor applies per roll |
| Upgrade a Minor Trait to Major | 15 PP | No ownership cap; one relevant Major applies per roll |
| New Ability Domain | 20 PP | Maximum 3 Domains; GM-approved scope |
| +1 Stat | 15 PP | Maximum +5 in each Stat |
| +1 inventory slot | 15 PP | Maximum 6 slots |

An upgrade needs a fictional reason the GM accepts — training, exposure, practice, or the thing that happened last session. The GM may require that reason to have appeared in play before the purchase, and may not require anything else.

There is no Expertise rule: trait and Stat bonuses represent exceptional aptitude.

## 9. Quick reference

Every line below summarizes a rule stated earlier in this book.

- **Roll:** `1d20 + Stat + up to one Major Trait + up to one Minor Trait` (§2).
- **Results:** miss by 5+ fails; miss by 1–4 succeeds with cost; meet TN through +5 is clean; +6 or more is critical (§2).
- **Post:** one Major Action, one Minor Action, movement, one conditional response, and Free Actions. Omitted parts are forfeited (§4).
- **Cycle order:** movement → actions and threats → conditionals → consequences. All hits land; excess is wasted (§4).
- **Threats:** address with the Major Action, answer with a conditional, or take it. No defensive roll (§4).
- **Damage:** every hit deals exactly 1. Armor first, then Strain. 0 Strain is Downed (§6).
- **Downed:** an Injury plus a deadline. Death needs a stated killing or an announced lethal danger (§6).
- **Creature harm:** 1 damage removes 1 Resistance box (§4).
- **Ability scale:** 0 / 1 / 2 Strain for Minor / Standard / Major; scale does not set damage (§5).
- **Noise:** Silent / Quiet +1 / Loud +2 onto a 0–6 area clock. 4–5 brings a search; 6 brings arrival (§4).
- **Awareness:** Unaware / Searching / Aware. Acting against Unaware resolves one band better (§4).
- **Cover:** partial answers one ranged threat per cycle; full blocks ranged threats both ways (§4).
- **Escape:** Major Action, TN 10 / 15 / 20. Success clears one band; twice leaves the scene (§4).

### Worked example: one cycle

The GM opens the cycle. Vey, the example character from §3, is at a market stall; the Bridge Brute from the [Creature Blueprint](Creature%20Blueprint.md) is winding up a club swing at their ally Mira.

> **GM post:** The brute plants itself at the bridge mouth and raises its club over Mira. Club Sweep, Melee reach, TN 15. If nothing answers it, Mira takes 1 damage. Noise Clock 1/6. The brute is Aware; it has been watching the approach since before the scene opened.

Vey posts a response:

> Major Action: I use my flame Domain to throw a focused burst at the bridge brute, keeping it away from Mira. Standard scale, 1 Strain. Finesse +2 and Street Alchemist +2; TN 15. On a Success with Cost, I will take 1 more Strain from the exertion.  
> Minor Action: I draw my rope.  
> Movement: I move from the market stall to the near side of the bridge, staying at Close range.  
> Conditional response: If the brute charges Mira, I shove her behind the stall.

The GM resolves the cycle in order. **Movement** first: Vey reaches the near side of the bridge. **Actions and threats together**: Vey's attack meaningfully addresses the Club Sweep, so one roll covers both. Vey rolls 9, adds Finesse +2 and Street Alchemist +2, for a total of 13 against TN 15 — a miss by 2, so Success with Cost. The attack lands, because all hits land: the brute loses 1 of its 2 Resistance boxes and its swing is driven off Mira.

**Conditionals**: the brute never charged, so Vey's conditional lapses untriggered, costing nothing — and the Minor Action it would have spent was already spent on the rope, which is why the brute charging would have been a problem.

**Consequences**: Vey pays 1 Strain for the Standard-scale ability and 1 Strain for the cost they proposed, dropping from 4 Strain to 2. The flame burst is Loud, so the Noise Clock moves 1 → 3. The GM updates positions and opens the next cycle.

---

**Document set:** [Index](README.md) · **Player Rulebook** · [GM Guide](GM%20Guide.md) · [Creature Blueprint](Creature%20Blueprint.md) · [Item Glossary](Item%20Glossary.md) · [Decision Log](Decision%20Log.md)
