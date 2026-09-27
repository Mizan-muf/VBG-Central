# VBG — Combat Module (Charge & Battle Map)

**Status:** experimental module, **untested** · **Revised:** 2026-09-24

**Owns:** an alternative combat package for VBG — the ability resource, the harm/ability split, and a position-based movement layer for use with a visual battle map.

> This optional module lists its overrides below and uses the [current core](../../rules/README.md) for everything else. It is separate from [Arcana Deck](../arcana-deck/README.md); their resource systems are not combined.

## 0. How this plugs in

A scene runs **either** base VBG combat ([Player Rulebook](../../rules/player-rulebook.md) §4–§6) **or** this module — never both, and never switched mid-scene. The GM states which at the top of the scene post. A character's numbers do not change depending on which is running; only the procedure around them does.

**What this module changes:**

| Subsystem | Change |
|---|---|
| Ability cost | Abilities spend a new resource, **Charge**, instead of Strain. |
| Harm | Unchanged — but now genuinely simple, since abilities no longer touch it. |
| Movement | Named positions on a real map, instead of the four fictional distance bands. |

**What this module inherits unchanged**, and does not restate: the d20 + Stat + Trait roll, the TN table, the four outcome tiers and their cost/critical limits, character creation, Downed / Injury / death, Resistance and creature defeat, the Item Glossary, and Progression except the one new line in §4. All of it is exactly as [Player Rulebook](../../rules/player-rulebook.md), [GM Guide](../../rules/gm-guide.md), [Creature Blueprint](../../rules/creature-blueprint.md), and [Item Glossary](../../rules/item-glossary.md) already state it.

**Why this exists.** In base VBG, Strain pays for abilities and is also what keeps a character conscious. Every attempt to add texture to ability use — a second track, a debt, a noise penalty — ends up being a second way to get hurt, because it's stacked on the same 4-point pool that's already your HP. This module removes that collision at the root: abilities stop touching Strain at all.

## 1. Charge — the ability resource

Every character has **Charge**, alongside Strain. Strain is now purely what keeps you conscious. Charge is purely what lets you use an ability.

**Base Charge: 5.** Record it next to Strain on the sheet: `Strain 4/4 · Charge 5/5`.

### Cost

Identical shape to base VBG's old Strain costs — only the pool changes.

| Scale | Charge cost | Action |
|---|---:|---|
| **Minor-scale ability** | 0 | A small 0-cost utility ability may use a Minor Action. |
| **Standard-scale ability** | 1 | Major Action. |
| **Major-scale ability** | 2 | Major Action. |

Attacks always use a Major Action, even at 0 Charge — same rule as base VBG, same reason.

### The headline change

> **Running out of Charge can never Down you.** If you have 0 Charge, you cannot use a Standard- or Major-scale ability until it recovers. That is the entire consequence. There is no version of "spend your last point and go Downed" anymore — that was a Strain rule, and abilities don't touch Strain here.

Everything else in [Player Rulebook](../../rules/player-rulebook.md) §5 about abilities is unchanged: scope, default reach, sustained effects (still spend the matching action type each cycle, still no further Charge cost to maintain), and hazard rules (a hazard still costs only the ability's Charge to create; catching a creature in it still needs a roll).

### Strain Transfer

Strain Transfer is a Standard-scale ability like any other: it costs **1 Charge** to activate, using a Major Action. Separately, and unrelated to Charge, it moves up to **2 Strain** from the healer to the recipient at 1:1, exactly as [Player Rulebook](../../rules/player-rulebook.md) §6 already states.

This is a small, genuine improvement the split gives you for free: in base VBG, the same rule had to clarify that the Strain spent *was* the activation cost, to stop a healer being charged twice out of one pool. Under this module that ambiguity can't arise — the 1 Charge and the up-to-2 Strain are different resources, so there's nothing to double-count.

### Recovery

One recovery rule now restores both pools at once:

- **Catch Your Breath:** recover **1 Strain and 1 Charge**, after a threat ends, once per scene.
- **Full Rest:** recover **all Strain and all Charge**, after roughly eight safe hours.

Item Glossary consumables that restore Strain are unchanged and still only restore Strain — there is no consumable that restores Charge in the base Item Glossary, and this module does not add one. If your table wants an item that restores Charge, write it the way any Item Glossary entry is written and give it a band.

## 2. Harm

**Nothing changes here.** A hit deals 1 damage. Armor absorbs it first, then Strain. At 0 Strain, a character is Downed: an Injury is named, a deadline is announced, stabilization and Strain Transfer both work exactly as [Player Rulebook](../../rules/player-rulebook.md) §6 and [GM Guide](../../rules/gm-guide.md) §6 already state.

The only thing worth flagging is what's now *true* about it: harm is the **only** thing that can Down a character. Not a bad roll on an ability, not running dry, not a resource decision. That was the entire design goal of this module, and it's a direct consequence of §1, not a separate rule.

## 3. Progression

One new line, alongside the existing Progression table in [Player Rulebook](../../rules/player-rulebook.md) §8:

| Upgrade | Cost | Limit |
|---|---:|---|
| +1 maximum Charge | 10 PP | Maximum 10 Charge |

Same cost and cap shape as +1 maximum Strain, so a table already running base VBG's progression doesn't have to learn a new pattern. **These numbers are a starting point, not a balanced result** — this whole module is untested; adjust them after a session or two if Charge feels too generous or too tight.

Character creation ([Player Rulebook](../../rules/player-rulebook.md) §3) gains one line: after recording 4 Strain, no Armor, and 4 Inventory Slots, also record **5 Charge**.

## 4. The battle map layer

This replaces the four abstract distance bands (Melee/Reach, Close/Room, Far/Hallway, Distant/Line of Sight) with **positions on a real map** — one your table can actually look at, not just narrate.

### 4.1 Pick a tool

The rules below are written to work with any of these. Pick based on what your table already has open.

| Tool | What it gives you | Tradeoff |
|---|---|---|
| **Owlbear Rodeo** *(recommended)* | Free, no login for players, works in a phone browser. A real map image, tokens, fog of war, a grid. Share one link per scene. | Needs a map image per scene — free stock battle-map art or a simple built-in grid both work fine. |
| **Google Slides** | Shapes as tokens on a slide, dragged by whoever's turn it is. Zero new accounts. | Two people moving the same token at once can conflict. No fog of war or built-in measuring. |
| **Google Sheets** | A grid of cells; tokens are initials in a cell; walls are marked cells. | Fastest to set up, reads as a spreadsheet rather than a map. Fine for a small, simple room. |
| **Discord-native** | GM posts a monospace grid or numbered image, edits the message each cycle. | No new tool at all, but slow to update and doesn't scale past a handful of positions. |

Whichever tool you use, the scene post still states the same things base VBG always required — threats, TNs, awareness, the Noise Clock if you're running it — the map is an addition, not a replacement for the post.

### 4.2 Positions and movement

- Before the scene, the GM builds a small map: **6–10 squares or named zones** is the right size. Bigger maps just mean more of the map goes unused.
- Each character or creature occupies **one square** at a time.
- **Movement budget: 2 squares per cycle**, accompanying your action — this is the same allowance as base VBG's "reaches up to Close / Room," just made literal instead of fictional. A normal square costs 1 to enter; a square you've marked as difficult terrain (water, rubble, a climb) costs 2.
- **Drive (Major Action):** commit your Major Action entirely to moving, and gain **+2 Pace** that cycle, to a maximum of 4 total. This is the module's one opt-in "sprint" — it costs you your other action to get it, so it's a real tradeoff, not a free bonus.
- **Engagement** is unchanged from base rules: a creature in your square or an adjacent one is engaging you, and leaving while engaged still requires Escape ([Player Rulebook](../../rules/player-rulebook.md) §4).

### 4.3 Range and line of sight

Read these directly off the map — this is the whole reason to use a real map tool instead of a hand-authored table for every pair of positions.

| Band | Squares (roughly) |
|---|---:|
| **Melee / Reach** | Same square, or adjacent |
| **Close / Room** | Up to 3 |
| **Far / Hallway** | Up to 6 |
| **Distant / Line of Sight** | Anything further, still visible |

- **These numbers assume a map roughly 8–10 squares across.** State your own ratio once at the top of the scene if your map is a different size — the point is a consistent, visible answer, not this exact number.
- **Cover and blocked sight are drawn on the map.** If a wall, crate, or other obstacle drawn between two tokens crosses the line between them, that lane is blocked (full cover) or degraded (partial cover) exactly as [Player Rulebook](../../rules/player-rulebook.md) §4 already defines those two states — the map just answers *which one applies* instead of the GM narrating it from scratch each time.
- **Text-only tools** (Sheets, Discord grids): mark which cells block sight directly on the sheet, and count cells for range the same way.

### 4.4 Features

Mark an interactable object directly on the map — a lever, a door, a crank — with a label or icon. No separate table is needed: interacting with it is an ordinary Minor or Major Action per [Player Rulebook](../../rules/player-rulebook.md) §4, with a TN if it's uncertain, stated in the scene post like anything else.

## 5. Worked example

The Bridge Brute ([Creature Blueprint](../../rules/creature-blueprint.md) §5) is at the bridge mouth. Vey, the example character, is on a 6×6 Owlbear Rodeo map: a market stall (B2), open bridge deck (C3–D3), and the far bank (E3), with a stack of crates at C2 drawn as full cover.

> **GM post:** Map linked above. Brute at D3, Aware, watching the crossing. Mira at C3. Club Sweep if unanswered: 1 damage to Mira. Noise Clock 1/6.

> **Vey's post:** Major Action: Flame Domain at the brute, Standard scale, **1 Charge**. Finesse +2, Street Alchemist +2, TN 15.
> Minor Action: draw rope.
> Movement: B2 → C2 (behind the crates), 1 Pace, into full cover.
> Conditional: if the brute charges Mira, I shove her to B3.

Resolution: movement first — Vey reaches C2 and is now in full cover from anything at D3 or beyond, per the map. The attack resolves against the Club Sweep as usual (one roll, since it addresses the threat). Vey pays **1 Charge**, not Strain — their Strain stays untouched at 4/4 regardless of the roll's outcome. If the roll had gone badly enough to cost Strain instead, that would only ever come from the *cost of a Success with Cost* or from being hit, never from casting the ability itself.

## 6. When not to use this module

Not every scene needs a map. A quiet conversation, a single opponent in an empty room, or a scene where positioning genuinely doesn't matter plays faster under base VBG's bands. Reach for this module for the fights where where-you-are is the actual tactical question — a bridge, a cordon, a chokepoint — and default to base combat everywhere else.

## 7. Status

**This is v0.1 and has not been played.** The Pace and range numbers in §4 are a starting point, not a tested result — expect to adjust them after the first real session. Nothing here should be treated as balanced until it's been run at an actual table.

---

**Document set:** **Combat Module** — a standalone add-on. See [VBG 2.2](../../rules/README.md) for the base game this plugs into.
