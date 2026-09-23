# Very Basic RPG 2.2 — Item Glossary

**Status:** working draft · **Revised:** 2026-09-24  
**Owns:** item statistics, acquisition and value bands, stack sizes, kit contents, consumable values, material quantities, scrap, and crafting.

> A working draft does not replace a published rule until approved. Anything marked pending is not playable; see the [Decision Log](Decision%20Log.md).

Shared inventory rules stay in the [Player Rulebook](Player%20Rulebook.md) §7. This document supplies the item-specific detail those rules point to.

**The rule that governs this entire document:** every hit in VBG deals exactly 1 damage, and nothing raises it ([Player Rulebook](Player%20Rulebook.md) §6). **No item below has a damage value.** A weapon is worth carrying because of what it lets you reach, break, conceal, or do quietly — never because it hits harder.

## 1. Entry format

Each entry states:

| Field | Meaning |
|---|---|
| **Slot** | 1, 1/2, or 1/4 of an Inventory Slot. |
| **Band** | Common, Restricted, or Rare. See §2. |
| **Noise** | Silent, Quiet (+1), or Loud (+2) onto the area's Noise Clock when used ([Player Rulebook](Player%20Rulebook.md) §4). **Every item carries one.** |
| **Effect** | What it actually does. Never a damage value. Any numerical bonus is stated explicitly here or does not exist. |
| **Uses** | Stack quantity, charges, or depletion, where applicable. |

An item with no listed effect is ordinary gear: it satisfies the fiction and nothing more, which is often all that is needed.

## 2. Acquisition and value

VBG has **no currency**. Coins, credits, and cash may exist in a setting's fiction and characters may argue about them, but nothing in these rules converts them into equipment. Items are obtained through four paths and sorted into three bands.

### The four paths

| Path | How it works |
|---|---|
| **Recovered** | Taken from a place or a body in play. Needs a scene, and carrying it out is usually the actual problem. |
| **Issued** | Granted by a faction, employer, patron, or authority the character answers to. Comes with an expectation, and can be taken back. |
| **Traded** | Given in exchange for something the other party wants: an item, a service, a debt, a secret. The GM plays the other party; the trade is a scene, not a purchase. |
| **Crafted** | Built from materials with tools and safe time. See §8. |

### The three bands

A band is **what a payment reaches**, not an amount. Bands do not make change: three Common acquisitions never add up to a Restricted one.

| Band | Availability |
|---|---|
| **Common** | Obtained freely between scenes with a plausible source. No scene needed. Rope, a lamp, a blade, bandages, basic material units. |
| **Restricted** | Requires one of the four paths, played out. Armor, firearms, medical kits, quality tools. A character cannot simply have one. |
| **Rare** | Obtained in play only, through a scene that cost something. Never issued casually, never traded for ordinary goods, never crafted outright. Suppressed weapons, hooded lamps, heavy armor, trauma supplies. |

### Starting gear

A character begins with **at most two items**, drawn from their Major Trait or backstory, and both must be **Common** ([Player Rulebook](Player%20Rulebook.md) §3). Starting gear cannot include Armor, which is Restricted or Rare by definition.

## 3. Weapons

Weapons grant **effects**, never damage. An unarmed character attacking with a Declared Action deals the same 1 damage as anyone else; what they lack is reach, concealment, quiet, and the ability to get through things.

| Weapon | Slot | Band | Noise | Effect |
|---|---:|---|---|---|
| **Light blade** — knife, shiv, dagger | 1/4 | Common | Silent | Concealable: a search does not find it without a reason to look. Drawn as a **Free Action** instead of a Minor Action. |
| **One-handed melee weapon** — club, hatchet, sword | 1/2 | Common | Quiet | Leaves the other hand free. Nothing else; it is the baseline armed character. |
| **Heavy weapon** — maul, axe, sledge | 1 | Common | Quiet | Two hands. Counts as a **breaching tool**: satisfies a creature condition or obstacle that requires heavy force to open. |
| **Polearm** — spear, pike, boat hook | 1 | Common | Quiet | Attacks at **Close / Room** without closing to Melee, and holds a band against one approaching threat. |
| **Bow or crossbow** | 1 | Common | Silent | Ranged attack to **Far / Hallway** without ticking the Noise Clock. Requires a free hand and ammunition. |
| **Sidearm** — pistol, revolver | 1/2 | Restricted | **Loud** | Ranged attack to **Far / Hallway**. Fired from partial cover without leaving it. |
| **Long arm** — shotgun, rifle | 1 | Restricted | **Loud** | Ranged attack to **Distant / Line of Sight**. Counts as a breaching tool at Close or nearer. |
| **Suppressed firearm** | 1/2 or 1 | **Rare** | Quiet | A sidearm or long arm whose noise drops from Loud to Quiet. This is the single most valuable property an item can have in a scene with a clock running. |
| **Shield** | 1 | Restricted | Silent | Answers **one melee threat per cycle** with a Free Action, the way partial cover answers a ranged one. Occupies a hand. |
| **Thrown explosive** | 1/2 | **Rare** | **Loud** | Creates a Close / Room hazard for one cycle without spending Strain. Single use. Deals 1 damage, like everything else. |

### Ammunition

| Stack | Slot | Band | Notes |
|---|---:|---|---|
| **Arrows or bolts, 10** | 1/2 | Common | Recoverable after a scene on a Clean Success or better. |
| **Cartridges, 12** | 1/4 | Restricted | Not recoverable. |

Ammunition is tracked per stack, not per shot. A stack depletes when a **Failure** or a **Success with Cost** paid in ammunition says it does, or when the GM states a scene has emptied it. VBG does not count individual rounds.

## 4. Healing and treatment

Consumables interact with two separate things: **Strain**, which comes back on its own, and **Injuries**, which do not ([Player Rulebook](Player%20Rulebook.md) §6).

| Item | Slot | Band | Noise | Effect | Uses |
|---|---:|---|---|---|---|
| **Bandages and dressings** | 1/4 | Common | Silent | Major Action within Melee / Reach: restore **1 Strain** to another character. Once per character per scene. | Stack of 3 |
| **Medical kit** | 1 | Restricted | Silent | Counts as **medical supplies**, making stabilization of a Downed character automatic instead of TN 10. Major Action: restore **2 Strain** to another character, once per character per scene. | 5 uses |
| **Trauma supplies** | 1/2 | **Rare** | Silent | Over downtime and roughly a day of safety, removes **one Injury**, including a Lasting one. Nothing else in the game does this. | Single use |
| **Stimulant** | 1/4 | Restricted | Silent | Free Action: restore **1 Strain** to yourself. The next scene begins with 1 less maximum Strain. | Single use |

**The limits.** No consumable restores Strain to the user except the stimulant, and no consumable heals a character above their maximum. A character may benefit from **one healing consumable per scene**, from any source — bandages and a medical kit do not stack on the same person in the same scene. Catch Your Breath is separate and still applies.

## 5. Armor

Armor is boxes that absorb physical damage before Strain. It is **never starting gear** and is acquired through the four paths in §2.

| Item | Slot | Band | Noise | Boxes | Repair material |
|---|---:|---|---|---:|---|
| **Padded or layered clothing** | 1 | Restricted | Silent | 1 | Fabric or leather |
| **Reinforced vest or brigandine** | 1 | Restricted | Quiet | 2 | Leather and metal |
| **Plate, riot gear, or heavy shell** | 1 | **Rare** | Quiet | 3 | Metal |

- Worn Armor occupies **1 slot** regardless of type. A character can wear only one Armor item.
- Armor absorbs **physical** damage, which is all damage unless a rule says otherwise ([Player Rulebook](Player%20Rulebook.md) §6).
- Armor **cannot pay ability Strain costs**.
- Quiet armor ticks the Noise Clock when the character moves under pressure — running, climbing, fighting — not when they stand still or walk.
- A spent box is repaired per §7. When **all** boxes are spent, the item becomes scrap (§8).

## 6. Tools, kits, and supplies

A kit counts as **one item** for starting gear only if its contents are defined here. This is the rule that stops a "kit" concealing unlimited equipment.

| Item | Slot | Band | Noise | Effect / contents |
|---|---:|---|---|---|
| **Rope, 50 ft** | 1/2 | Common | Silent | Ordinary gear. Climbing, binding, hauling. |
| **Oil lantern or torch** | 1/2 | Common | Silent | Light source: fixes **Dim** or **Dark**, and announces the carrier to anything that hunts by sight. |
| **Hooded lamp** | 1/2 | **Rare** | Silent | A light source that does **not** announce the carrier: directional, shuttered, visible only in the direction it is pointed. |
| **Repair tools** | 1 | Restricted | Quiet | Required for Armor repair (§7) and crafting (§8). Contents: hammer, files, punch, needle, thread, wire. |
| **Lockpicks or entry tools** | 1/4 | Restricted | Silent | Opening a lock without force becomes a Declared Action at TN 15 rather than impossible. Contents: picks, tension bar, shim. |
| **Climbing kit** | 1/2 | Common | Quiet | Contents: 50 ft rope, three anchors, harness. Lowers a climbing TN one band where an anchor can be set. |
| **Rations and water, 3 days** | 1/2 | Common | Silent | Required for a Transition Scene of more than one leg ([Player Rulebook](Player%20Rulebook.md) §4). |
| **Ignition supplies** | 1/4 | Common | Quiet | Matches, flint, lighter fluid. Contents: enough for a scene. |
| **Pouch or pack** | — | Common | Silent | Organizes existing slots. **Grants no capacity.** Extra capacity comes only from PP upgrades. |
| **Equipment case** | — | Restricted | Quiet | Organizes existing slots and protects fragile contents from a scene's consequences. Grants no capacity. |
| **Keys, tokens, small valuables** | 1/4 | Varies | Silent | Per defined bundle. Band is set by what the thing opens or is worth to someone. |

## 7. Materials and repair

A **material unit** is the quantity that repairs one thing once.

| Material | Slot | Band | Repairs |
|---|---:|---|---|
| **Metal unit** | 1/4 | Common | Plate, vest, blades, tools |
| **Leather unit** | 1/4 | Common | Vest, harness, padded clothing |
| **Fabric unit** | 1/4 | Common | Padded clothing, bindings |
| **Wood unit** | 1/4 | Common | Hafts, shafts, shields, bows |

**Armor repair:** restore **1 Armor box** with safety, repair tools, **one appropriate material unit**, and roughly one hour ([Player Rulebook](Player%20Rulebook.md) §6). No roll, given all four. Remove the material unit from inventory.

Material units stack at 4 units per 1/4 slot of the same material.

## 8. Scrap and crafting

### Scrap

When every box of an Armor item is spent, the item **becomes scrap** and cannot be restored by ordinary repair.

| Scrap | Slot | Yields |
|---|---:|---|
| **Armor scrap** | 1/2 | 2 material units of its construction material, recovered through crafting below. |
| **Broken tool or weapon scrap** | 1/4 | 1 material unit. |

### Crafting

Crafting requires **repair tools, safe time measured in downtime rather than cycles, and the materials listed**. It is not done during a threat scene.

| Goal | Requirement | Roll |
|---|---|---|
| Reclaim material units from scrap | Tools, a safe hour per unit | None |
| Make or replace a **Common** item | Tools, 1 appropriate material unit | None |
| Make or replace a **Restricted** item | Tools, 2 appropriate material units, and one Restricted-grade component obtained in play | TN 15 |
| Rebuild Armor from scrap | Tools, material units equal to the item's box count, plus the scrap | TN 15 |
| Make a **Rare** item | — | **Not possible.** Rare items are obtained in play, never manufactured. |

A **Failure** consumes the materials. A **Success with Cost** produces the item and consumes one extra material unit, or produces it with a stated flaw the GM names.

## 9. Shared constraints

These belong to the [Player Rulebook](Player%20Rulebook.md) and every entry above satisfies them:

- A character starts with at most two Common items selected through their Major Trait or backstory.
- Inventory starts at 4 slots and can reach 6 through PP upgrades. PP is never spent on items.
- Fractional item sizes consume actual capacity. Stacking requires a defined quantity.
- No item deals more than 1 damage, because nothing does.
- A numerical bonus exists only where an entry states it.

---

**Document set:** [Index](README.md) · [Player Rulebook](Player%20Rulebook.md) · [GM Guide](GM%20Guide.md) · [Creature Blueprint](Creature%20Blueprint.md) · **Item Glossary** · [Decision Log](Decision%20Log.md)
