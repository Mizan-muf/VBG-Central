# VBG 2.2 documentation restructuring plan

Status: implemented on 2026-09-20. The split preserves 2.2 as a working draft and does not make new mechanical decisions.

## 1. Target document structure

Keep the new rules together under `drafts/vbg-2.2/`. Split by reader and purpose, rather than creating a separate file for each subsystem.

| File | Purpose and authoritative content |
|---|---|
| `README.md` | Version status, reading order, document links, and authority conventions. |
| `Player Rulebook.md` | All shared rules needed to create a character and play: resolution, actions, threats, movement, abilities, harm, inventory, and progression. |
| `GM Guide.md` | Procedures and guidance for presenting scenes, adjudicating declared actions, setting difficulty, handling consequences, and resolving asynchronous posts. Links to shared mechanics instead of redefining them. |
| `Creature Blueprint.md` | Creature construction: tiers, card fields, strengths, weaknesses, special defeat conditions, regeneration requirements, and the worked creature example. |
| `Item Glossary.md` | Item-entry format and, once decided, equipment values, stacks, kit contents, consumable effects, and material quantities. Initially retain the existing checklist and label entries as pending. |
| `Decision Log.md` | Unresolved rules, decision status, and a concise record of changes. Separate settled rules from proposals and historical notes. |

Keep the quick reference, terminology list, and play examples inside the Player Rulebook. Separate files would create unnecessary navigation and more summaries to maintain at this size.

## 2. Player Rulebook outline

1. **Start here:** asynchronous RPG premise, player and GM roles, required materials, and how to use the book.
2. **Core resolution:** declare intent, decide whether a roll is needed, set TN, apply Stats and Traits, resolve outcomes and consequences. Briefly introduce Strain, Armor, and action types before using them in examples.
3. **Create a character:** allocate Stats; choose Major and Minor Traits; define a Domain; record 4 Strain, no Armor, and 4 slots; select at most two permitted items. Include a completed example. Link to progression for later upgrades.
4. **Play a scene:** the 24-hour cycle, Major/Minor/Free Actions, post format, movement and distance, incoming threats, missed posts, and shared creature Resistance/defeat rules.
5. **Use abilities:** Domain scope, scale and cost, action type, reach, duration, last-Strain timing, hazards, and targeted versus untargeted uses. Give hazard damage its own heading.
6. **Harm and recovery:** damage sequence, Armor, Downed and death, traumatic conditions, rest, medical aid, Strain Transfer, and Armor repair/scrap. Give Strain Transfer a short procedure and its own heading.
7. **Inventory and equipment:** slots, fractions, stacks, kits, containers, worn Armor, and equipment benefits. Link to specific item definitions in the Item Glossary.
8. **Progression:** PP awards, upgrade costs, and limits. Preserve pending award amounts and prerequisites as unresolved.
9. **Reference and examples:** concise terminology index, quick reference with links, sample player post, and a complete GM-to-player-to-resolution example.

Character creation may repeat starting values for usability. Identify the owning rule section through links and check those repeated values during review.

## 3. Source-to-destination map

Source: `drafts/VBG 2.2 Rulebook Draft.md` unless otherwise stated.

| Current content | Destination and treatment |
|---|---|
| §1 Core engine | Player Rulebook: core resolution. Move version-removal notes, such as Expertise, to the Decision Log. |
| §2 Stats and Traits | Player Rulebook: character creation. Move advancement prices to progression; retain links. |
| §2 Ability Domain selection | Player Rulebook: character creation. |
| §2 Ability operation, hazards, examples | Player Rulebook: abilities. Preserve examples alongside the relevant rule. |
| §3 Strain, Armor, harm and recovery | Player Rulebook: harm and recovery. Include starting values in the creation checklist. |
| §4 Inventory and equipment | Player Rulebook: inventory; starting choices also appear in character creation. Item-specific definitions belong in the Item Glossary. |
| §§5–6 Actions, asynchronous play, movement | Player Rulebook: play a scene. Put Free Actions beside Major and Minor Actions. |
| §7 Threats, Resistance, defeat and interaction with creature protections | Player Rulebook: shared threat/creature rules. Preserve rules players need to interpret their actions. |
| §7 Creature construction requirements | Creature Blueprint. Put encounter-running guidance in the GM Guide. |
| §8 Progression | Player Rulebook: progression. |
| §9 and inline unresolved notes | Decision Log, with short linked pending notices at affected rules. |
| Existing 2.2 Monster Creature Blueprint | Creature Blueprint: retain design-specific details and example; replace duplicated shared rules with linked summaries. |
| Existing 2.2 Item Glossary Backlog | Item Glossary: retain checklist status; do not invent equipment statistics during migration. |

Review all three existing 2.2 documents before cutting text: the blueprint contains details not present in the main draft, including regeneration requirements and action-card fields.

## 4. Editorial fixes

- Use the same section pattern where useful: purpose, rule/procedure, exceptions, example, related links.
- State the roll trigger once in full. Ability rules must refer to uncertainty or forcing an outcome, rather than implying every declared ability use requires a roll.
- Split dense paragraphs into steps or short rule groups, especially Strain Transfer and ability maintenance.
- Use explicit labels: Major Trait, Major-scale ability, Major Action; do the same for Minor.
- Define the relationship between post, turn, round, cycle, and scene. If equating terms would decide timing behavior, record the question instead of silently changing it.
- Define or flag Transition Scene; do not invent travel mechanics to fill the gap.
- Keep mechanical exceptions next to their parent rule. Move historical comparisons and discussion status out of instructional prose.
- Preserve local pending notices for incomplete procedures such as stabilization; moving the detail to the Decision Log must not imply those procedures are playable and complete.
- Use descriptive headings and relative section links. Mark every document as part of the 2.2 working draft.
- Treat examples and quick references as summaries of linked rules. They must not introduce costs, bonuses, or exceptions.

## 5. Decision handling

Give each unresolved issue an ID, current settled constraints, exact unanswered question, affected sections, and status. Record decisions only when made.

Initial issues:

- Downed stabilization, permitted actions, and traumatic-injury treatment/removal.
- Item definitions, healing consumables, stacks, kit contents, repair material units, and scrap crafting.
- PP award amounts and additional prerequisites.
- Difficulty examples, acceptable costs, and critical benefits.
- Timing terminology and Transition Scene definition where the current text is insufficient.

The existing `REFINEMENT_BACKLOG.md` predates several settled 2.2 choices. Label it as historical planning and point readers to the new Decision Log; preserve its historical content. Keep `BASELINE_COMPARISON.md` scoped to its existing v1.4.2/VBG-Z comparison.

## 6. Implementation order

1. **Inventory the source rules.** Create a temporary migration checklist covering each rule, table, example, number, exception, and unresolved note in the three 2.2 source files. Record its destination and authority owner.
2. **Create the destination structure.** Add the index and five documents with version status and headings. Move content before rewriting it so omissions are easy to detect.
3. **Rebuild the Player Rulebook.** Follow the outline above; consolidate character creation and the scene procedure, then edit ability and recovery sections.
4. **Complete supporting documents.** Separate GM adjudication guidance from creature construction. Transfer the equipment checklist and decisions without resolving them by assumption.
5. **Add reader aids.** Write the character example, post template, and complete resolution example using settled rules. Add the terminology index and quick reference.
6. **Review and switch navigation.** Verify content coverage and links, then update the repository README. Replace the three old draft entry points with short relocation notices linking to the new documents; retain source history in Git. Update internal references and the historical backlog notice together.
7. **Record completion.** Summarize editorial changes and remaining decisions in the Decision Log. Keep publication status separate from completion of the restructuring.

## 7. Completion checks

- Every source rule has a destination; no rule disappears during deduplication.
- Roll formula, TNs, outcome margins, starting values, ability costs, damage, recovery, action allowance, distances, inventory fractions, PP prices, and caps match the source.
- A new player can create a character and submit a valid post from the Player Rulebook without consulting the GM Guide or Creature Blueprint. Item-specific details may require the Item Glossary and remain explicitly pending where undefined.
- A GM can follow one resolution cycle without reconciling competing versions of a rule.
- The jar/flame examples, willing-recipient healing, last-Strain use, hazard damage timing, and creature defeat retain their original behavior.
- A sample resolution shows TN, modifiers, margin, outcome, player-chosen cost or advantage where relevant, incoming-threat handling, and resulting resource changes.
- Pending decisions remain visible, and no proposed item or procedure is presented as settled.
- All relative file and heading links resolve, including the old entry-point notices.
- Base v1.4.2 and VBG-Z mechanics remain unchanged. The restructure does not imply module compatibility or publish 2.2.
