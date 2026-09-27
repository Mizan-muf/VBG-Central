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

- `archive/v1.4.2/very-basic-rpg-vbg.md`
- `archive/v1.4.2/vbg-major-traits.md`
- `archive/v1.4.2/vbg-minor-traits.md`
- `archive/v1.4.2/vbg-abilities.md`
- `archive/v1.4.2/vbg-monster-creature-blueprint.md`

### Zombie module

- `modules/zombie/vbg-z-player-rulebook-zombie-survival-edition.md`
- `modules/zombie/vbg-z-master-rules-glossary-keyword-specification.md`
- `modules/zombie/vbg-z-survivor-traits-specializations-catalog.md`
- `modules/zombie/vbg-z-gm-survival-horror-compendium.md`

## Arcana Deck — proposed VBG 2.2 overrides

**Status:** untested module design; not adopted base rules. This section compares the separate [Arcana Deck design](../modules/arcana-deck/README.md) against VBG 2.2, not the historical VBG-Z comparison above. The module distinguishes user-confirmed mechanics from proposed supporting rules and owns all procedures and trial values.

| Area | VBG 2.2 baseline | Arcana Deck proposal |
|---|---|---|
| Roll trigger | An uncertain outcome or forcing an outcome on another creature. | Roll only for uncertainty. Drawing, playing, and combining cards do not inherently trigger checks. |
| Domain access | Approved Domains can use the scale rules in Player Rulebook §5. | Each Domain starts with Minor cards; PP unlocks Standard and Major. Recommend defined decks per Domain sharing types/ranks. |
| Ability resource | Ordinary abilities pay scale-based Strain. | Remove Strain entirely; abilities spend cards and actions, with no HP or Charge activation cost. |
| Health | Start with 4 Strain, shared by health and ability costs. | Start at 5 HP; retain 1 damage per hit, Armor, and creature Resistance. Downed and Injury procedures use HP. |
| Recovery and healing | Recover Strain; healing abilities use Strain Transfer. | Proposed HP conversion for recovery/items; replace Strain Transfer with defined healing cards. Values and restrictions are owned by module §7. |
| Card availability | No magical hand or daily draw allowance. | At most three active cards across all Domains; seven daily random reveals initially, increased with PP. |
| Drawing | Drawing an ordinary item uses a Minor Action. | Each random card draw costs either a Minor or Major Action. No free opening hand or refill. Proposed staged reveal permits spending the remaining action afterward. |
| Minor card play | Small utility abilities may use a Minor Action. | A Minor card can spend either action, retaining Minor scope. Attacks still require the Major Action. |
| Combinations | One Major Action and one Minor Action per cycle; no card-combo procedure. | Two Minor cards or Minor + Standard/Major can use both actions. No extra action, automatic roll, rank promotion, or damage increase. |
| Progression | Player Rulebook §8 lists the permitted PP purchases. | Add daily-draw/per-Domain rank purchases; replace maximum-Strain upgrade with maximum HP. Prices and caps remain trial proposals. |
