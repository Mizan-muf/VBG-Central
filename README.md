# Very Basic RPG (VBG)

VBG is an asynchronous, fiction-first tabletop RPG. **VBG 2.2 is the current core ruleset**, promoted from draft on 2026-09-27.

## Start playing

1. Read the [Player Rulebook](rules/player-rulebook.md) to create a character and play.
2. Use the [GM Guide](rules/gm-guide.md) to run scenes.
3. Reference the [Creature Blueprint](rules/creature-blueprint.md) and [Item Glossary](rules/item-glossary.md).

The [core index](rules/README.md) defines rule authority. The [Decision Log](rules/decision-log.md) records settled decisions and future changes. No setting or combat module is required.

## Repository layout

| Folder | Contents | Status |
|---|---|---|
| [rules/](rules/README.md) | VBG 2.2 core and decision record | Current rules; no tracked rules decisions pending |
| [modules/](modules/README.md) | Arcana Deck, Charge Combat, and legacy VBG-Z | Optional; each module states its own status |
| [docs/](docs/README.md) | Release notes and rules comparisons | Supporting records |
| [archive/](archive/README.md) | VBG 1.4.2, earlier audits, and retired planning | Historical; not current rules |

**Arcana Deck is retained**, including its Domain decks and artwork. Arcana Deck and Charge Combat remain untested and are separate combat packages. Their proposals do not become core rules through this reorganization.

Port Vane and its setting integration have been removed. Historical notes may mention the retired setting, but create no dependency on it.

## Maintaining the rules

- Keep the core genre-neutral and give each rule one owning document.
- Modules state their overrides explicitly and link to the core for inherited rules.
- Use kebab-case document filenames and `README.md` folder indexes.
- Record changes in the Decision Log and [release notes](docs/release-notes.md); update the [comparison](docs/baseline-comparison.md) when module overrides change.

The core is out of draft. This editorial release does not claim proven balance or completed playtesting; see the release notes for scope and remaining editorial matters.
