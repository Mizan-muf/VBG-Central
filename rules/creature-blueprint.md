# Very Basic RPG 2.2 — Creature Blueprint

**Status:** current core rules · **Version:** 2.2 · **Revised:** 2026-09-27  
**Owns:** creature construction — tiers, card fields, strengths, weaknesses, conditions, and defeat requirements.

> VBG 2.2 is the current core ruleset. Modules apply only when explicitly adopted; see the [rule authority](README.md#3-rule-authority).

Shared play rules are in the [Player Rulebook](player-rulebook.md). Encounter-running guidance is in the [GM Guide](gm-guide.md).

## 1. Core creature rules

- Creatures do not roll. The GM announces threats; players roll to respond.
- **Resistance** is the only defeat track. It represents toughness, protection, or resolve; even unarmored creatures have it.
- Each 1 damage removes 1 Resistance box. **Every hit deals exactly 1 damage** — no weapon, ability scale, Critical Success, or weakness raises it (Player Rulebook §6). A creature's Resistance is how many hits it takes, and nothing more.
- The last box defeats the creature. The declared action and fiction determine whether it falls, flees, surrenders, or dies.
- Bargains, tricks, and other fitting actions can overcome a creature without removing every box.
- Resistance is not equipment Armor. It does not become scrap and does not change player Armor rules.
- Regeneration must state how many boxes return, when they return, and how to stop it. A defeated creature returns only if its rules explicitly allow it.

## 2. Threat tiers

These are starting guides. Behavior, numbers, terrain, and weaknesses also determine danger.

| Tier | Resistance | Role |
|---|---:|---|
| Minor | 1 | Small threat; dangerous in groups. |
| Standard | 2 | Ordinary encounter. |
| Major | 3–4 | Major obstacle or encounter. |
| Boss | 5+ | Requires preparation or a special approach. |

**Resistance is duration, not difficulty.** A Boss with 6 boxes is not six times as dangerous as a Minor — it is a fight that lasts longer, during which its threats keep landing. What makes a creature hard is everything else on the card: the conditions that must be met before its boxes can be removed at all, the weaknesses that have to be found, the threats it puts out each cycle, and the ground it holds. A card that raises Resistance and nothing else has made the fight slower, not harder. Raise the count only when you want the fight to take more cycles.

## 3. Creature card

Fill every field before the encounter.

**Name:**  
**Tier:**  
**Description:** Appearance, movement, and warning signs.  
**Resistance:** one box per point of the creature's tier.  
**Senses:** how it actually finds people — sight, hearing, smell, vibration, heat, or something stranger. **This field is required.** It is what tells a player whether darkness, silence, or cover will do anything at all, and without it the whole perception layer in [Player Rulebook](player-rulebook.md) §4 is guesswork. State what it cannot do as well: *hunts by sound; effectively blind past Close / Room.*  
**Noise it makes:** what the creature itself ticks onto the Noise Clock when it acts. Most things are Quiet; a Boss tearing through a wall is Loud.  
**Starting awareness:** Unaware, Searching, or Aware of the characters when the scene opens.

### 3.1 Actions

List 3–6 options. The GM need not use every option each cycle.

For each action, state:

- **Name / Warning:** what the creature is about to do.
- **Target / Reach:** whom it affects and at what distance.
- **Response / TN:** a suggested player response and difficulty; other approaches may work.
- **Consequence:** what happens if unresolved. State damage, injury, displacement, or other effects clearly.

### 3.2 Strengths and weaknesses

**Strengths:** explain what makes the creature dangerous, including immunity, regeneration, or unusual abilities.

**Weaknesses:** explain what players can exploit, how they can discover it, and its effect. A weakness never grants extra damage, because nothing does. It lifts a condition, lowers a TN, exposes the creature to something it was immune to, forces a retreat, or satisfies a defeat requirement.

### 3.3 Creature conditions

> **Terminology.** A **creature condition** is a rule about what can harm this creature. A **Condition** on a player character is an injury (Player Rulebook §6). They share a word and nothing else; always write *creature condition* on a card. The card field for what players can exploit is **Weaknesses**, and every document in this set uses that one word for it.

Conditions can alter what harms the creature and how. They can create resistance or immunity, a particular vulnerability, or a required means of injury or defeat.

For each condition, state its trigger, effect, duration when relevant, and a discoverable clue. Apply it before removing Resistance. A successful roll does not bypass it by itself.

### 3.4 Behavior

**Goal:** what it wants.  
**Approach:** how it fights, negotiates, and responds to hazards.  
**Retreat:** what makes it give up early.

### 3.5 Defeat

**Normal:** what losing the last Resistance box means given the player's action.

**Special condition, if any:** state the requirement for lasting defeat, the discoverable clue, and what happens at 0 Resistance before the condition is met.

## 4. Running creatures

- Announce threats before players respond in the 24-hour cycle.
- State the area's Noise Clock in every scene post, and each creature's awareness state. Neither is hidden information.
- A creature's awareness rises a step when it sees, hears, or is hit by a character, and falls a step after a full cycle with nothing to find. Its **Senses** field decides which of those apply.
- Use the Player Rulebook TNs and outcome rules. Success with Cost still succeeds.
- One player roll can answer both an action and a related threat. Failure creates no extra reaction roll, and a threat never grants the player a defensive roll of its own: the **Response / TN** field is the difficulty of a suggested answering action, not a save.
- Resolve a cycle in the Player Rulebook §4 order. Every hit declared that cycle lands; excess damage past the last box is wasted.
- A creature action that can kill a player character must say so on the card, and the GM must announce it before the cycle in which it resolves (Player Rulebook §6).
- A hazard created in advance needs no roll; directly catching a creature with it does.
- A damaging hazard deals 1 damage to each exposed creature each cycle. Do not count entering and remaining twice in one cycle, and do not add damage for overlapping hazards — several at once still deal 1 in total.
- Use the four distance bands. Ordinary movement stays within Close / Room; list exceptional movement on the card.

## 5. Example: Bridge Brute

**Tier:** Standard  
**Description:** An unarmored toll collector with a heavy club.  
**Resistance:** [ ] [ ] — endurance and determination.  
**Senses:** ordinary sight and hearing. It watches the bridge mouth and nothing else; anyone approaching along the waterline below is out of its view until they climb up.  
**Noise it makes:** Quiet. The club on the deck plates carries, but only across the bridge.  
**Starting awareness:** Aware. It has been watching the approach since before the scene opened.

| Action / Warning | Reach | Suggested response | Unresolved consequence |
|---|---|---|---|
| Club Sweep — winds up a swing | Melee | Evade or interrupt, TN 15 | 1 damage |
| Drive Back — lowers its shoulder | Melee | Hold ground or sidestep, TN 15 | Pushed back within Close; announce any fall risk first |
| Bar the Crossing — plants its club across the path | Close | Maneuver past, TN 15 | Route stays blocked; a fitting complication follows |

**Strengths:** holds a narrow crossing, where only one character can reach it at a time.  
**Weaknesses:** a credible bargain buys passage without a fight — discoverable from anyone who has crossed before. It will not follow anyone off the bridge.  
**Creature conditions:** none.

**Behavior**  
**Goal:** collect a toll from everyone who crosses, and be seen doing it.  
**Approach:** plants itself at the bridge mouth, swings at whoever presses forward, and gives ground to nobody. Avoids flame barriers rather than charging through them.  
**Retreat:** leaves when the toll stops being worth the injuries, or when the crossing is no longer the only route.

**Defeat**  
**Normal:** yields, flees, or falls when the last box is removed, according to the declared action. Nothing on this card kills a player character; it is a beating, not a killing.  
**Special condition:** none.

Two hits defeat it — that is what Standard tier means, and no hit in VBG deals more than 1. A total of 13 against TN 15 still lands a declared attack, with a cost. Creating flames ahead of it does not guarantee entry; creating flames beneath it requires a roll. The [Player Rulebook](player-rulebook.md) §9 resolves a full cycle against this creature.

---

**Document set:** [Index](README.md) · [Player Rulebook](player-rulebook.md) · [GM Guide](gm-guide.md) · **Creature Blueprint** · [Item Glossary](item-glossary.md) · [Decision Log](decision-log.md)
