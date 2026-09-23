# Living World — player-run encounters

**Status:** design proposal; player-run PvE requirement confirmed, procedures require testing · **Revised:** 2026-09-24  
**Owns:** encounter permissions, player-run PvE, simultaneous play-and-run safeguards, encounter packets, and their review.

## 1. Confirmed direction and explicit authority extension

The user has specified frequent combat and monster encounters run by authorised players, including people authorised to play their own PC while running an encounter. This is a core server capability, not an exceptional favour requiring a staff DM at every fight.

**Local authority extension:** Port Vane's [Campaign Format §2](../port-vane/Campaign%20Format.md) reserves the world's response to DMs. This module delegates defined monster behaviour, tactical resolution, and specified immediate consequences to an authorised encounter runner inside an approved encounter packet. Institutional responses, unrestricted world invention, and lasting consequences outside that packet remain with staff. The setting source itself is unchanged.

A player can propose a fight or recruit a group without holding runner permissions. Someone with the appropriate endorsement must open and resolve it. Social hosting, faction rank, veteran status, and willingness to run do not themselves confer that endorsement.

## 2. Permissions

| Permission | Permitted work | Boundary |
|---|---|---|
| Player | Play a PC, propose tactics and encounters, verify public results | Cannot run monsters or decide another participant's outcome by default. |
| Encounter runner | Run approved packet families for other PCs; adjudicate their listed effects | No own PC in the encounter without the separate play-and-run endorsement. |
| Play-and-run runner | Run and participate using an approved public, deterministic packet | No hidden scenario information, improvised enemy tactics, changed rewards, or self-decided disputes. |
| Encounter reviewer | Verify and post fixed packet rewards when uninvolved in that encounter | Separate endorsement; no own PC, alternate character, or shared-asset beneficiary in the claim. |
| DM / world steward | Authorise packets and endorsements; handle exceptions, major world consequences, and lasting harm | Conflicts of interest still require an independent decision. |

Endorsements record packet families, permitted tiers, whether simultaneous participation is allowed, and review authority. Initial runner training covers the combat/movement reference, two matching adjudication exercises, and one observed encounter. Play-and-run adds a hidden-information and conflict-of-interest exercise. These are proposed competency checks, not a requirement to recruit professional GMs.

Start with Tier I and approved Tier II packets. Tier III, secrets-dependent hunts, bespoke enemy powers, major setting changes, and PvP remain staff-run until separately delegated. A permission can be narrowed after repeated errors; resolve conduct issues through moderation, not fictional retaliation.

## 3. What an approved encounter packet contains

| Required field | Why it is fixed before entry |
|---|---|
| Packet ID/version; allowed runner permissions | The scope of delegation is checkable. |
| Setting/site constraints and available instance allowance | Runners cannot invent unlimited incursions or place monsters in contradictory ongoing scenes. |
| Eligible party size and capability band | Composition determines the published variant before play; no scaling after seeing rolls. |
| Starting map and position IDs | Terrain, entry, cover, hazards, elevation, and exits use the movement rules. |
| Monster cards and public behaviour policies | Every move, target, trigger, tie-break, and retreat rule has an owner. |
| Objectives, threat budget, reinforcement limit | A win condition and bounded pressure prevent endless waves. |
| Full action data | Reach, timing, TN, target shape, consequence, interruption, costs, and any resistance/protection. |
| Attention input/output and incident ID | Loudness cannot reset or double-charge between encounters. |
| Stakes and stop conditions | Wounds, defeat, escape, lethal risks, and escalation boundaries are known. |
| Fixed reward schedule and supply reservation | Outcome-dependent awards are specified; no creation of private loot tables. |
| Closure/recovery rules and review record | Current resources and later claims have a single handoff. |

A packet is a reusable procedure attached to a legitimate local situation. It is not a quest-board prerequisite or a compulsory expedition. Players may initiate a defence, pursue a sighting already established in play, or contest a route; a runner selects a permitted packet and registers a valid instance.

## 4. Encounter lifecycle

1. **Register.** Select an authorised packet variant, reserve its instance/reward allowance and location/time, name the runner and any reviewer, and snapshot participant resources. A complete in-scope registration needs no live staff approval. A mismatch becomes a staff request, not a silent exception.
2. **Disclose.** Publish map, applicable rules version, objective, stakes, runner participation, allowed effects, and party eligibility. Players opt into the disclosed encounter. PvE authority does not grant PvP permission against another party member.
3. **Lock the monster briefing.** Derive enemy intents from the public policy, publish intended routes/threat IDs, and fix them before PC declarations or rolls. New information can change the next briefing or a prewritten conditional, not rewrite an existing threat to counter a posted tactic.
4. **Collect and resolve.** Use [Combat](Combat%20Module%20Plan.md) and [Movement](Movement%20and%20Positioning%20Plan.md). Apply deterministic rules inside the packet. A runner cannot invent an ability midfight or quietly lower Resistance to rescue their own PC.
5. **Record immediately.** Log current Strain, Armor, spent supplies, positions, attention events, and Downed state as they occur. Those changes apply now; pending reward review never restores spent resources.
6. **Close.** Publish the final snapshot, objective result, monster/claim IDs, participants, resource deltas, recovery eligibility, and any requested lasting outcome. Participants may flag discrepancies; silence is not permission to expand stakes.
7. **Review.** An independent authorised reviewer verifies fixed rewards and posts the ledger transaction. Staff handle lasting harm, unlisted discoveries, standing, and city consequences. Disputed deltas stay reserved; unrelated play uses the uncontested current snapshot.

A clean closure releases a PC for their next compatible scene using their actual remaining resources, even if its payout awaits review. They cannot spend pending loot, heal by opening another thread, or enter a fight whose legality depends on an unresolved injury. Record linked waves as one incident and recovery boundary.

## 5. Running while playing

For simultaneous participation, require an **open packet**: no secret map, concealed weaknesses, private NPC agenda, unrevealed random tables, or runner-only information. Surprises may be public conditional triggers with uncertain timing. If genuine hidden information matters, use staff or a nonparticipating runner separately endorsed for that packet type.

- Publish monster decisions before locking the runner's PC declaration. All players may inspect the same information; no PC gets access to a secret preparation step.
- Derive target choices from printed priorities and public tie-breaks. Example: highest registered active Domain attraction → shortest legal route → lowest stable character ID. These priorities belong to that monster, not every Carrion.
- Resolve equal movement claims and branch choices by the movement procedure. Neither the runner nor their PC receives precedence.
- Costs and consequences use printed entries. The runner may propose a creative action for their own PC, but cannot approve an unlisted benefit, favourable TN change, new critical reward, or new weakness. Use a listed fallback or pause that disputed component for an independent ruling.
- Public dice and event records remain visible. Fix clerical errors with an appended correction rather than silently changing a roll, target, or map.
- Rewards for the runner's PC use the same outcome schedule and eligibility as everyone else's, validated independently. Hosting adds no combat PP, loot, or progression multiplier; service recognition is nonmechanical.
- Any participant can flag a rules discrepancy. An independent reviewer can verify a calculation or apply a published correction. If no existing rule settles it, pause the affected resolution for an uninvolved DM/world steward; reward-review endorsement does not confer new-rule authority. Do not decide it by party vote or by who benefits most.

The runner is allowed ordinary tactical decisions for their PC. Their monster decisions are constrained by the packet. This makes participation possible without pretending that hidden information can simply be forgotten.

## 6. Exceptions and lasting stakes

Stop at the smallest affected boundary when the fight leaves its approved scope: an unlisted Domain interaction, a PC attacking another PC, a disputed irreversible injury, reinforcement beyond the packet budget, or a claimed city-wide consequence. Keep unrelated social play moving; do not continue a dependent combat branch on an invented ruling.

An adopted lethal packet must include an approved death/rescue procedure before it is available. A runner applies its immediate Downed and rescue rules; staff verify any permanent outcome. Staff review checks the rule and agreed stakes rather than granting a runner discretion to kill or spare particular PCs. Until that procedure exists, such packets remain test fixtures without permanent character stakes.

NPC witnesses, institutional recognition, new world clues, property transfer, and faction responses require the named staff authority unless an exact bounded result was approved in the packet. A public monster behaviour clue on a packet is encounter information; it does not authorise inventing new lore elsewhere.

## 7. Frequency, rewards, and repeated fights

Frequent combat should be available without unlimited reward production. [World Systems](World%20Systems%20Plan.md) still owns award rates, supplies, and ownership.

- Each canonical encounter has a unique instance ID and a reserved reward allowance. A reusable packet is not an infinite source of corpses or cash.
- Reopening a thread, rotating runners, changing PCs to alts, retreating and returning, or splitting a swarm cannot pay the same objective or salvage claim again.
- PP uses the common contribution cap; fights remain worthwhile for concrete objectives, access, materials, experience of play, and relationships. New monster kills do not generate extra advancement outside that schedule.
- After an area's permitted instances or resources are exhausted, publish that fact. Offer another legitimate situation or explicitly noncanonical practice; never rebrand practice loot as campaign supplies.
- Runner-only service can be recognised publicly without awarding their off-scene PC resources or implying that NPC kills happened to that PC.

## 8. Runner sheet and acceptance checks

~~~text
INSTANCE / PACKET VERSION / RUNNER ENDORSEMENT:
PARTY / RUNNER'S PC IF ANY / INDEPENDENT REVIEWER:
LOCATION / FICTIONAL TIME / INCIDENT / RESERVED REWARD ALLOWANCE:
OPENING SNAPSHOT / MAP VERSION / OBJECTIVE / STAKES:
EACH CYCLE: monster policy result; threat IDs; locked declarations; rolls;
            movement snapshots; resource deltas; attention events; exceptions
CLOSURE: objective result; remaining resources; recovery boundary;
         reward claims; lasting-outcome requests; corrections; reviewer
~~~

Test the same packet with a staff DM, runner-only player, and play-and-run player. Identical inputs must produce identical legal moves, targets, damage, resource changes, and reward claims. Include a runner's endangered PC, unfavourable tie-break, attempted self-award, host handoff, missing player, unclear creative effect, and exhausted reward allowance.

Measure staff minutes per player-run fight, review latency, disputes, and runner effort. Routine cycles should need no live staff intervention; exceptions remain visible. Increase simultaneous fight capacity only when there are enough endorsed runners and independent reviewers to sustain it.
