# Very Basic RPG (VBG)

VBG is an asynchronous, fiction-first tabletop RPG. This repository preserves the base game and publishes setting modules that intentionally modify its rules.

## Contents

| Material | Version | Status |
|---|---|---|
| [VBG 2.2 document set](drafts/vbg-2.2/README.md) — player rules, GM guidance, creature blueprint, item glossary, and decisions | 2.2 | Working draft; complete, nothing pending |
| [Port Vane](drafts/port-vane/README.md) — setting module for VBG 2.2: a rotting fortress-city in 2013 where Domains are a licensed industry | — | Working draft; playable |
| [Base rules](base%20rules/Very%20Basic%20RPG%20%28VBG%29.md) — the core game | 1.4.2 | Published baseline; unedited |
| [Base traits and abilities](base%20rules/) — major traits, minor traits, abilities, and creature blueprint | 1.4.2 | Published baseline; unedited |
| [VBG-Z](Zombie%20Module/) — survival-horror module | 2.0 | Published module; unedited |

### Working notes

These are internal records, not distribution material.

- [Open questions](docs/revision-notes/OPEN_QUESTIONS.md) — ambiguous and blocking rules in the 2.2 draft, as candidate Decision Log entries.
- [Baseline comparison](docs/revision-notes/BASELINE_COMPARISON.md) — mechanical changes from v1.4.2 to VBG-Z 2.0, and the source conflicts still open in VBG-Z.
- [Refinement backlog](docs/revision-notes/REFINEMENT_BACKLOG.md) — base-game design questions that predate the 2.2 draft.
- [VBG 2.2 restructuring plan](docs/revision-notes/VBG_2.2_RESTRUCTURING_PLAN.md) — the document split implemented on 2026-09-20.

## Where to start

- **Playing VBG 2.2:** read the [Player Rulebook](drafts/vbg-2.2/Player%20Rulebook.md). It is complete enough to create a character and post a turn.
- **Running VBG 2.2:** read the Player Rulebook, then the [GM Guide](drafts/vbg-2.2/GM%20Guide.md).
- **Playing in Port Vane:** read the [Campaign Format](drafts/port-vane/Campaign%20Format.md) first, then the rest of that set in its stated order.
- **Checking what is settled:** read the [Decision Log](drafts/vbg-2.2/Decision%20Log.md).

## Repository conventions

- Keep the base rules genre-neutral.
- Put module-specific overrides in the module folder; label every override explicitly.
- Update the baseline comparison whenever a module changes a core rule.
- Give every rule exactly one owning document, and link to the owner rather than copying the rule.
- Do not silently overwrite source material; record an approved revision in Git history.

## Current status

The base rules and VBG-Z remain an unedited baseline. VBG 2.2 is the active draft revision: it does not replace v1.4.2, does not change VBG-Z, and does not imply compatibility between them.

As of **2026-09-24**, the VBG 2.2 [Decision Log](drafts/vbg-2.2/Decision%20Log.md) has an empty pending list — every rule it tracks is written into the document that owns it. Two repository decisions remain outstanding and are not rules questions: a **licence and author credit**, and whether to rename files out of spaces. Both are recorded as Q20 and Q21 in the [open questions](docs/revision-notes/OPEN_QUESTIONS.md).

[Port Vane](drafts/port-vane/README.md) is the first setting module. It scaffolds on 2.2 rather than forking it: it adds Domain loudness as a noise trigger, a Burnout track, and its own catalogs and gear entries, and reads every other mechanic from the base set.
