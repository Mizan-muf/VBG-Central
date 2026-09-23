# VBG Living World Module — design plan

**Status:** proposal, not playable rules · **Revised:** 2026-09-24  
**Owns:** scope, package structure, reading order, and authority for this planning set.

## 1. Direction

Build a persistent ensemble campaign where players initiate relationships, disputes, investigations, businesses, neighbourhood projects, and fights. The city remembers what happens. Characters need neither a standing party nor a dispatched mission to participate.

**Confirmed by the user:** VBG 2.2 baseline; Port Vane setting; 20–40 active players; primarily asynchronous Discord play; 2–3 DMs/world stewards; frequent combat; authorised player-run monster encounters, including authorised people playing while running; tight, rich combat and a novel-feeling movement system; opt-in PvP with agreed stakes and staff handling lasting consequences; a separate module folder.

**Design recommendation:** make tactical combat a central, repeatable activity. Use named positions, exact movement routes, separate firing lanes, and staged resolution to make positioning consequential and consistent across runners. Relationships and world consequences connect frequent fights to city life; ordinary conversation stays easy to start.

Players should be able to say “we are opening a clinic,” “we need to find who closed the bridge,” or “we are organising the tenants” and start recruiting other PCs immediately. Staff adjudicate the city's response. An incursion is one source of play among many.

## 2. Read the plan

| Document | Owns |
|---|---|
| [Player Roleplay Module Plan](Player%20Roleplay%20Module%20Plan.md) | Player-led scene procedure, relationships, consent, interpersonal conflict, and scene records. |
| [Combat Module Plan](Combat%20Module%20Plan.md) | Optional tactical combat design, action resolution, harm, encounter construction, and combat playtests. |
| [Movement and Positioning Plan](Movement%20and%20Positioning%20Plan.md) | Novel-feeling position-and-route prototype: exact movement, firing lanes, cover, engagement, and map snapshots. |
| [Encounter Running Plan](Encounter%20Running%20Plan.md) | Authorised player-run and play-and-run PvE; packets, monster policies, rewards, and independent review. |
| [World Systems Plan](World%20Systems%20Plan.md) | Projects, world developments, economy, progression, and additional systems. |
| [Discord Operations Plan](Discord%20Operations%20Plan.md) | Server layout, permissions, canonical records, chronology, staff workload, and onboarding. |
| [Port Vane Integration](Port%20Vane%20Integration.md) | Setting bindings, source constraints, starter situation, and setting-specific dependencies. |
| [Decisions and Roadmap](Decisions%20and%20Roadmap.md) | Baseline audit, proposed override register, work order, unresolved choices, and launch gates. |

Start with this index, combat, movement, and encounter running. Then read roleplay and world systems for life between fights. Use the roadmap to commission the actual rules and playtest packets.

## 3. Package boundaries

| Component | Dependency | Intended use |
|---|---|---|
| Living-world framework | VBG 2.2 + approved setting | Shared continuity, projects, progression, economy, and operations. |
| Player roleplay module | VBG 2.2; living-world records for persistent consequences | Usable on its own for PC scenes; required for this server. |
| Tactical combat module | VBG 2.2 + its own approved equipment/creature additions | Optional in VBG generally; intended default for this server's consequential combat after testing. |
| Player-run encounter framework | Tactical combat + movement + approved packets | Core server capability; separate runner-only, play-and-run, and review endorsements. |
| Port Vane adapter | Port Vane setting + living-world framework | Domains, Carrion, faction memberships, local economy, and starting situations. |

Keep these as distinct documents now; give each a rules document and reference sheets when implemented. A server fixes one combat rules version at scene opening. Players do not switch between basic and tactical combat to obtain better rewards or recovery. Abstract an uncontested outcome through ordinary adjudication; specify any alternate resolution method before stakes are accepted.

> ### Baseline moved — 2026-09-24
>
> **This planning set has not been revised against the current baseline.** It was written while several core items were open, and those items are now settled. The plans below still describe them as pending, which is stale, not authoritative:
>
> | Referenced here as open | Now |
> |---|---|
> | **D2** — item catalog pending | Written in full. Four acquisition paths, three value bands, no currency, no damage values. |
> | **D3** — award rate missing | Settled: per session or arc, equally, 2–5 typically. The trial rate proposed in World Systems §6 is close to it and no longer needs to be invented. |
> | **D5a** — Transition Scene | Settled: one to three legs, one obstacle and one roll each. |
> | **Q13 / Q14** — Domain approval, trait catalog | Both settled. Approval has a four-test standard in GM Guide §3; VBG ships no catalog and Port Vane supplies an original one. |
> | **Q15** — non-threat procedure | Settled as **deliberately freeform**. The Player Roleplay Module Plan is therefore a proposed *addition* to a settled freeform default, not a candidate answer to an open question. |
> | **Port Vane: Cult as staff-run antagonist** (Decisions and Roadmap L7) | Superseded. **No faction is an antagonist**; every faction and the Stray path are playable, and the Carrion are the only threat. |
>
> Also note that VBG 2.2 now owns a full perception layer — engagement, cover, awareness, light, a 0–6 Noise Clock, moving unseen, and pursuit. The Movement and Positioning Plan should be re-read as an extension of that layer rather than a replacement for its absence.
>
> Reconcile these before commissioning any rules pack from this set.

## 4. Authority and status

- The [VBG 2.2 set](../vbg-2.2/README.md) remains the baseline. **It no longer has pending entries**; see the note above.
- [Port Vane](../port-vane/README.md) owns established setting facts. Its DM-only world-response rule receives a scoped local extension through Encounter Running: authorised runners resolve approved PvE packets; staff retain broader world authority.
- This folder proposes extensions and explicit local overrides. None is approved, balanced, or retroactively inserted into either source set.
- In an adopted release, an explicitly listed module override governs its named subject; everything else stays with its existing owner. Record that release's baseline snapshot and exact changes.
- Use one rules owner per subject. Examples, character sheets, bots, and quick references link to the owner; they cannot introduce mechanics.
- A world steward is an authorised DM for world rulings. An encounter runner receives only their recorded packet permissions, including play-and-run where endorsed. An ordinary scene host or moderator receives neither merely from their title.

## 5. Target experience

| Layer | What players do | What persists |
|---|---|---|
| Personal | Talk, help, bargain, disagree, form commitments | Relationships, promises, character decisions |
| Neighbourhood | Recruit a crew, maintain a place, investigate, organise protection | Projects, local conditions, contacts, shared assets |
| City | Intervene in faction plans, expose evidence, respond to crises | Ratified consequences, institutional responses, public history |

Launch across a few active places with many ways to interact. Broaden the map when play needs it. Keep recurring locations useful between emergencies; players can stay, build, recover, and pursue ambitions without returning to a hub or waiting for a quest window.

The proposed operating limits and numerical trials in these documents are hypotheses. The roadmap defines how to test them before treating the module as ready to run.
