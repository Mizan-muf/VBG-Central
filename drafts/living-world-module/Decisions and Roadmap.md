# Living World — decisions and roadmap

**Status:** planning record, not approved rules · **Revised:** 2026-09-24  
**Owns:** source audit, proposed changes, decision gates, work sequence, and release criteria.

> **Superseded in part (2026-09-24).** The VBG 2.2 baseline has since settled that **every hit deals exactly 1 damage, permanently**, and that weapons grant effects rather than damage ([Decision Log](../vbg-2.2/Decision%20Log.md) §2a). Every proposal below that assumes a 2-damage pattern needs rewriting as an *effect* — a condition it defeats, a defence it breaches, a band it reaches — before it can be commissioned. Gear acquisition is no longer a gap: see [Item Glossary](../vbg-2.2/Item%20Glossary.md) §2.


## 1. Confirmed scope

| Decision | User answer |
|---|---|
| Rules baseline | VBG 2.2 draft. |
| Setting | Port Vane. |
| Population and medium | 20–40 active players, mostly asynchronous Discord. |
| Staffing | 2–3 DMs or world stewards. |
| PvP | Opt-in; agreed stakes; staff handle lasting consequences. |
| Combat emphasis | Frequent combat with a tight, rich tactical system; novel-feeling movement requested. |
| Player-run PvE | Authorised players run monster encounters; some are also authorised to play their PC while running. |
| Deliverable | A separate living-world module plan, including deeper combat, player-to-player roleplay, and further systems. |

These answers authorise the plan's scope, not its proposed numbers or rule overrides. Existing source files remain authoritative until an adopted module explicitly replaces a named rule.

## 2. Whole-system audit and proposed baseline comparison

The [2.2 index](../vbg-2.2/README.md), Player Rulebook, GM Guide, Creature Blueprint, Item Glossary, and Decision Log form the active baseline. [Review findings](../../docs/revision-notes/OPEN_QUESTIONS.md) expose additional candidate Q items; they are not settled rules. [Port Vane's questions](../port-vane/Open%20Questions.md) use P IDs. Published base v1.4.2 and VBG-Z 2.0 are historical design inputs, not mechanically compatible catalogs.

| Subject | VBG 2.2 baseline / gap | Proposed module treatment | Owner |
|---|---|---|---|
| Resolution | d20 + Stat + one relevant Major/Minor; four margin bands | Preserve for ordinary resolution. Any setup bonus is an explicit extension; opposed PvP is a separate tested override. | Combat C1/C2/C7 |
| Creation | Three Stats; one Major, one Minor, one mandatory Domain; 4 Strain, no Armor, 4 slots, at most two items | Preserve except proposed Domainless substitution. Review legacy traits before use. | Combat C5/C8; adapter |
| Traits and progression | +2/+1 relevance; existing PP prices/caps; D3 award rate missing | Preserve prices/caps; propose activity-independent awards and audited evidence. | World Systems §6 |
| Actions and threats | Major + Minor + movement; 24-hour cycle; creatures do not roll; Q1–Q3 unresolved | Entry/opening movement/setup/main/fallout/closing stages; exact threat policies and fallback/resource handling. | Combat C1/C2/C10 |
| Non-threat play | No formal procedure, Q15 | Voluntary social beats, agreements, and logged closure; no forced PC beliefs. | Player Roleplay |
| Abilities | Open scope; 0/1/2 activation costs; scale does not itself grant damage | Reviewed effect patterns and explicit damage; loudness reports. No automatic legacy powers. | Combat C3/C5 |
| Harm | Default 1 damage; physical Armor first, then Strain; Q5/Q9 gaps | Bounded 2-damage entries and defined coverage; keep shared Strain resource. | Combat C3 |
| Downed / recovery | At zero Strain; subsequent hit kills; D1 incomplete; safe rest restores Strain | Explicit treatment, last-Strain and transfer timing; resolve PvE lethality choice before consequential play. | Combat C4 |
| Equipment / inventory | 4–6 slots, fractions, Armor 1 slot; D2 catalog pending | Small approved catalog, ownership/acquisition record, exact stacks/uses. No infinite storage carried into a scene. | Combat C8; World Systems §5 |
| Creatures | Resistance-only defeat track; discoverable conditions | Objective-based Carrion cards and threat budgets; preserve a single defeat track. | Combat C6 |
| Time and travel | Fictional bands; Close accompanying movement; no Sprint; D5 incomplete | Keep band labels but replace tactical geometry with exact positions/routes/lanes, 2 Pace, and Major Drive +2. Persistent chronology remains separate. | Combat C9; Movement; Operations §4 |
| GM authority | GM adjudicates outcomes; Port Vane reserves world response to DMs | Explicit scoped delegation to authorised runners, including play-and-run; immediate packet state and independent reward review. Staff retain broader world authority. | Encounter Running; Operations §§2–5 |
| Persistent world | No complete shared economy, project, faction, or continuity engine | Add projects, local clocks, obligations, access, and world-change records. | World Systems |

Do not import VBG-Z recovery restrictions, infection, free counters, or item values wholesale. Do not import the base v1.4.2 d10 engine or unreviewed catalogs. Its [historical comparison](../../docs/revision-notes/BASELINE_COMPARISON.md) remains about those versions; this table records this module's proposed differences.

## 3. Decisions to settle during implementation

| ID | Recommendation | What must be decided / dependency |
|---|---|---|
| L1 — authority | Delegate approved PvE packets to endorsed runners; keep broader world response with staff | Implement Encounter Running's runner-only/play-and-run/reviewer permissions, preauthorised outcomes, immediate costs, and independent reward validation. |
| L2 — tactical depth | Combat C1–C10, exact staged timing, interacting weapon/maneuver roles, and objective fights | Settle Q1–Q3 together, then D5/Q6/Q12/Q27; independently reproduce movement, conditional costs, setup, threat targeting, and invalid-target outcomes. |
| L3 — harm | Keep Strain and reachable treatment; telegraph danger | Explicitly retain or override PvE second-hit death. Adopt D1/Q10/Q11 and Armor Q9 rulings before character stakes. PvP remains consent-bound. |
| L4 — Domains | Curated effects plus bounded creative uses | P1/Q13/Q14/Q25; source list unavailable; commission a replacement if it cannot be obtained. |
| L5 — Domainless PCs | Launch with tested training packages | Decide compensation, later awakening, PP costs, and conversion. Never grant both starting options for free. |
| L6 — economy | Small catalog, abstract payout bands, repayable individual obligations within ongoing dependence | D2/Q4/P5; define stabiliser/burnout demand, rewards, restricted project funds, and transaction authority. Complete freedom from Ledger debt would depart from Factions §2 and needs a separate setting ruling. |
| L7 — factions | Narrative standing; institutional rank separate from PP | P2–P4/P7; pilot Cult as staff-run antagonist, pending explicit option policy. Clarify the setting's conflicting affiliation/registration uses of “Stray in uniform.” |
| L8 — advancement | Trial 2–3 PP per two-week review period | D3; test speed, mixed-experience play, evidence standards, alt handling, and absence. |
| L9 — continuity | One consequential scene plus limited social concurrency | D5/Q12; adopt snapshot, reservation, review, and absence rules from Operations. |
| L10 — PvP / social contests | Agreements for social choices; separately tested opposed combat | D4/Q15 and Combat C7; settle ties, multi-PC exchanges, withdrawal, and adjudication before competitive play. |
| L11 — movement model | Prototype positions/routes/independent firing lanes as the novel-feeling approach | C9 overrides baseline estimated distances and no-Sprint rule. Test Pace, occupancy, cover, area scope, vertical routes, and forced movement; the user has not approved these numbers. |
| L12 — frequent player-run combat | Reusable local packets and a pool of endorsed runners | C10; recruit actual capacity, test play-and-run conflicts, open-information policy, finite reward allowance, and review throughput before scaling. |

Remaining choices have concrete recommendations above. They do not block completion of this plan; they block adoption of the affected rules. Keep unready options outside the pilot instead of filling gaps through silent table custom.

## 4. Work packages

| Stage | Deliverables | Completion gate |
|---|---|---|
| **A. Freeze the pilot contract** | Baseline snapshot; accepted L/C choices; numbered local overrides; minimal glossary; content boundaries and authority sheet | Two DMs can identify the owner and status of every pilot rule. |
| **B. Player-led social slice** | Two-page player guide; opening/closure templates; three location cards; invitations; character approval checklist; staff review register | Players complete ordinary scenes without a live DM; logs preserve agency and separate world requests. Mechanical rewards remain disabled until their rules exist. |
| **C. Tactical and runner slice** | Staged combat and movement references; position/route/lane template; seven maneuver entries; six weapon/tool profiles; three Armor profiles; three treatments; six Domain patterns; four Domainless packages; five reusable packets; runner/reviewer endorsement exercises | All relevant timing, movement, damage, rescue, item, cost, and delegated-authority questions have local answers; pass Combat §10 and Movement/Encounter Running gates. |
| **D. Persistent-world slice** | Project/clock cards; starting supply and payout table; stabiliser/debt specification; transaction register; PP review process; starter Port Vane situation | One event can affect several scenes without duplicate rewards, incompatible chronology, or unauthorised discoveries. |
| **E. Closed integrated pilot** | 8–12 players; 2–3 DMs; trained volunteer runners; two connected neighbourhoods; frequent combat connected to social/project/economic play | Run 2–4 weeks or longer if necessary; include independent and play-and-run fights and meet the checks below across two successive review periods. |
| **F. Expand to target size** | Revised guides, tested runner/reviewer permissions, handoff coverage, packet library, public changelog | Expand toward 20–40 active players and the Operations fight-frequency target while runner availability, review latency, and staff workload stay within budget. |
| **G. Broaden the world** | Additional districts, professions, crafting, civic events, larger crises | Each addition has demand, an owner, tested costs, and capacity. Travel, Cult PCs, and Tier IV require separate decisions. |

These are dependency stages, not promised delivery dates. B and C can develop in parallel after A; D needs the relevant catalogs and authority rules. Controlled mechanical tests can use pregenerated fixtures; persistent characters need the actual approved creation rules. Do not treat fixture gear or test wins as campaign property or history.

## 5. Integrated playtest checks

| Question | Evidence / initial target |
|---|---|
| Do players initiate play? | At least 70% of pilot scenes originate from player invitations or ambitions rather than direct staff dispatch. This is a server metric, never a player quota. |
| Can a newcomer join? | An available invitation and first scene within 72 hours of character approval; investigate barriers instead of penalising pace. |
| Is ordinary RP independent? | Test friendship, disagreement, refusal, missed posts, and closure; no live DM required for personal decisions. |
| Does canon stay consistent? | Each immediate packet result has an authorised runner/source event; each wider world change has an approving DM and effective fictional time; no pending reward used elsewhere. |
| Can economic play be audited? | Test duplicate salvage claims, simultaneous transfers, item loans, absent owners, broken Armor, and attempted thread-based recovery. Reject duplicates without blocking unrelated play. |
| Does combat add choices? | Meet Combat §10 targets for clarification, 2–4-cycle ordinary encounters, useful non-attack actions, and Domainless contribution. Test new/veteran mixed groups. |
| Is movement both distinctive and exact? | Two runners produce identical positions, legal lanes, costs, and triggers. Test alternative routes, directional cover, narrow crossings, capacity, carries, areas, and forced movement. |
| Can players run fights without live staff? | Complete ordinary approved packets in runner-only and play-and-run modes; apply immediate expenditure/recovery, then independently validate rewards. No self-awards or hidden-information advantage. |
| Does frequent combat remain sustainable? | Measure runner hours separately; simulate repeated fights, reward exhaustion, disputed injury, reviewer backlog, and host handoff. Clean state can enter the next scene while payouts wait. |
| Is consent robust? | Test withdrawal, faction rivalry, indirect sabotage, surrender, and multiple affected PCs. No default loss because someone refuses a new stake. |
| Do quieter players advance? | Compare equally meaningful social, practical, and combat contributions; identical review criteria and no per-post multiplier. |
| Can staff sustain it? | Median routine closure review ≤4 minutes; world requests normally resolved within seven days; aggregate work within the staffing budget. Track long-tail disputes separately. |
| Does the city remember play? | At least one local condition changes through collective noncombat action; its effect appears in later scenes and a world digest. |

The combat plan's 12 controlled encounters can include fast facilitated tests as well as asynchronous runs, but at least four must use real asynchronous posting, four must be authorised player-run, and two of those must include runner-PC participation. These subsets may overlap. Do not infer queue performance from simulated dice alone. Record failures and revise the responsible rule; a missed target is information, not a reason to reward more posting.

## 6. Publishable module checklist

- A named version with exact baseline and setting dependencies; clearly labelled optional components.
- Player guide, roleplay procedure, combat and movement rules, runner permissions/packet library, world procedures, GM operations, approved catalogs, and quick references that introduce no new rules.
- Local override comparison reconciled against the latest accepted core decisions; no contradictions concealed by linking to pending text.
- Character/resource migration instructions and a changelog; active scenes keep their declared version unless all affected parties and the DM agree to a correction.
- Public scenario material separated from staff secrets; tested access and reliable copies of canonical records.
- Author credit, feedback route, and a distribution/licensing decision, as already flagged by source review Q20. No assumption that consulting another game's reference text authorises reproducing its wording.

This task produces the design package. Final rules, full catalogs, demonstrated balance, and a live Discord deployment are subsequent work packages, not completed artifacts of this plan.
