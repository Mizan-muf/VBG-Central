# VBG 1.4.2 → VBG-Z 2.0 baseline comparison

Status: observation only. This records the imported rules; it does not choose the future base-game design.

## Core changes introduced by VBG-Z

| Area | Base VBG 1.4.2 | VBG-Z 2.0 | Design effect |
|---|---|---|---|
| Resolution | `Stat + Trait` d10 pool, maximum 4 dice, highest die vs fixed 7 | `1d20 + Stat + Trait` vs TN 10/15/20/25+ | Replaces the core probability model with margin-of-success play. |
| Outcomes | 1–6 failure; 7–9 success with cost; 10 critical | Failure by 5+; success with cost by 1–4; clean success by 0–5; critical by 6+ | Adds clean success and makes cost/consequence depend on TN margin. |
| Expertise | Pool 5+ gives a boost or reduced cost | No equivalent rule | Removes high-pool narrative reward. |
| Stats | Three 0–3 stats; max +2 at creation | Three stats, described as -1 to +2; max +2 at creation | Retains the stat names but changes their numeric meaning and cap language. |
| Starting traits | 1 Major (+2), 2 Minor (+1) | 1 Major (+2), 1 Minor (+1), plus Specialization | Narrows background breadth and moves spotlight powers to a separate domain. |
| Abilities | Open-ended magical/heroic Domain, 0–3 Strain scales | Tactical Specialization, fixed 0–2 Strain techniques | Grounds powers in survival-horror fiction and limits scale. |
| Health and recovery | 5 Strain, 2 starting Armor; scene and downtime recovery | 4 Strain, no starting Armor; no natural recovery | Turns attrition and supplies into the principal survival pressure. |
| Damage | Narrative wounds; spend Strain or Armor to soak | Armor absorbs first; then Strain; Downed and death timer | Adds explicit lethality and condition handling. |
| Inventory | 5 slots; backpack adds 5 | Strict 4 slots; compact items stack four per slot | Makes loadout choice materially restrictive. |
| Time and actions | No formal per-turn action structure | 1 Major + 1 Minor + free actions; 24-hour side initiative | Establishes a repeatable asynchronous combat procedure. |
| Combat space | Fiction-first positioning | Four distance bands, cover, disengagement, called shots, grab counter | Makes tactical location and weapon handling explicit. |
| Equipment | General slot sizes | Weapons, ammo, durability, herbs, armor, key items | Adds a survival-resource economy. |
| Escalation | GM reaction on failure | Area Noise Clock, breach milestones, safe-room isolation | Converts noise into an objective, shared threat meter. |
| Threats | Generic creature blueprint | B.O.W. cards, infection, V-ACT revival, boss pursuit | Adds horror-specific enemy behaviour and campaign pressure. |
| Progression | 10/15/20/20/25 PP costs; stat cap 3 | 10/15/20/25 PP costs; specialization and inventory upgrades | Shifts progression away from broad supernatural growth. |

## Base rules retained or extended well

- Force, Finesse, and Focus remain the three universal attributes.
- Major and Minor Traits still express character identity and add +2/+1 respectively.
- Monsters remain player-facing: they create threats and force player rolls instead of rolling attacks.
- Armor boxes, slot-based inventory, PP, and asynchronous play persist.
- The module preserves the base game's success-with-cost ethos, then formalizes it.

## Cross-document conflicts to resolve before publication

| Topic | Conflicting text | Recommended decision |
|---|---|---|
| VBG-Z Strain capacity | Player rulebook says “Max 10,” starts at 4; dossier and glossary define 4 boxes; infection caps at 2/1. | Decide whether 4 is the permanent maximum or current boxes within a 10-point maximum; state both current and maximum consistently. |
| VBG-Z stat cap | Glossary PP shop caps stats at +2; GM compendium caps them at +3. | Choose one cap and update all three VBG-Z references. |
| Natural recovery | Base game allows Catch Your Breath and full-rest recovery; VBG-Z GM compendium forbids natural Strain recovery. | Make this an explicit VBG-Z override in the player rulebook and glossary. |
| Noise Clock start | GM compendium defines 0–6; glossary defines 1–6 and resets after a breach to 1. | Use 0–6 or 1–6 everywhere; define a sector's starting value and post-breach reset. |
| Called shots | Glossary makes called shots TN 20 with armor/dismemberment effects; Specialization offers a 1-Strain version that bypasses armor. | Define the default called-shot rule and the specialization's distinct benefit. |
| Armor wording | Player rulebook says marked armor negates physical damage; other text calls marked boxes ruined. | Define whether a box is expended, damaged, or both, and when each state repairs. |
| Healing language | Player rulebook calls G+G a full restoration of “all 4 Strain”; base says 5 starting Strain; glossary repeats 4. | Finalize VBG-Z capacity before item values are locked. |
| Trait loadouts | Major traits grant weapons/utilities, but 4-slot starting inventory has no explicit accounting or universal starter kit. | State which loadout items are mandatory, their slots, and how overflow is handled. |
| Firearm data | Player rulebook lists a generic handgun as 15 rounds; glossary gives model-specific ammo, magazine, and range values. | Establish one canonical equipment catalog and have the player book reference it. |
| Terms and headings | Glossary has two sections numbered 6; “Near” appears in weapon text but distance bands say Melee/Close/Far/Distant. | Normalize headings and vocabulary during the edit pass. |

## Source files reviewed

### Base game

- `base rules/Very Basic RPG (VBG).md`
- `base rules/VBG Major Traits.md`
- `base rules/VBG Minor Traits.md`
- `base rules/VBG Abilities.md`
- `base rules/VBG MONSTER _ CREATURE BLUEPRINT.md`

### Zombie module

- `Zombie Module/VBG-Z_ Player Rulebook (Zombie Survival Edition).md`
- `Zombie Module/VBG-Z_ Master Rules Glossary & Keyword Specification.md`
- `Zombie Module/VBG-Z_ Survivor Traits & Specializations Catalog.md`
- `Zombie Module/VBG-Z_ GM Survival Horror Compendium.md`

