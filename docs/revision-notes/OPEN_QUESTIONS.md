# VBG 2.2 — ambiguous and blocking items

**Status:** internal review note · **Raised:** 2026-09-20 · **Updated:** 2026-09-24 · **Not distribution material**

> ## Resolved 2026-09-24
>
> **Every blocking item in §1 is settled**, along with D1, D2, D4 in part, D5 in part, and the ambiguous items Q7–Q13 and Q17–Q19, Q26–Q30. The rulings live in the [VBG 2.2 Decision Log](../../drafts/vbg-2.2/Decision%20Log.md) §2a, which is now their owner, and the text is carried into the Player Rulebook, GM Guide, Creature Blueprint, and a fully written Item Glossary.
>
> The headline rulings:
>
> - **Every hit deals exactly 1 damage, permanently.** Weapons grant effects, never damage. Creature tiers measure how long a fight lasts, not how hard it hits. *(Q5, Q25)*
> - **Downed inflicts an Injury and starts a deadline. Death requires a stated killing or an announced lethal danger, and nothing else.** *(D1)*
> - **The cycle has an order** — movement, actions and threats together, conditionals, consequences. All hits land, excess is wasted, a character Downed in a cycle still acts. *(Q3)*
> - **A threat gets no defensive roll.** Address it, hold a conditional for it, or take it. One conditional per post, spending the Minor Action. *(Q1, Q2)*
> - **The Item Glossary is written in full**, with four acquisition paths and Common / Restricted / Rare value bands in place of currency. *(Q4, D2)*
> - **Escape has a procedure and a TN band.** *(Q6)*
>
> ## Carry-through pass, 2026-09-24
>
> **The rulings above had been recorded but not written.** A third audit found the Player Rulebook still at its 2026-09-20 text — no perception layer, no cycle order, no conditional-response rule, no Injury procedure, and a §6 line stating that a Downed character *"dies if struck again"*, the exact opposite of D1 — while the Item Glossary was still a checklist of empty boxes despite D2 claiming it was written in full.
>
> A decision recorded in a log and absent from the rules text is not a rule. The pass wrote all of them in and closed the remainder:
>
> - **D3 settled.** PP is awarded per session or arc, equally, 2–5 typically; +1 for a survived risk, an avoided fight, a discovery, or costly roleplay, +2 for an objective, +3 for a milestone. Not currency.
> - **D5a settled.** A Transition Scene runs as one to three legs, one obstacle and one roll each; Failure converts a leg into a threat scene.
> - **Q14 settled.** VBG 2.2 ships no trait catalog and does not adopt the v1.4.2 lists. Port Vane supplies its own original catalog.
> - **Q15 settled.** Non-threat play is deliberately freeform; only threat scenes use the cycle.
> - **Q16 settled.** All 6 points are spent, nothing below −1, and +2 / +2 / −1 is intended.
>
> **Nothing in VBG 2.2 is pending.** Only Q20 (licence and credit) and Q21 (filenames) remain, and both are repository decisions rather than rules. The tables below are kept as the record of what was asked; read the [Decision Log](../../drafts/vbg-2.2/Decision%20Log.md) for what is true.

A review of the VBG 2.2 document set for rules that cannot be applied as written. Every item below is a **candidate** entry for the [Decision Log](../../drafts/vbg-2.2/Decision%20Log.md), not a decision and not a rule. Promote the ones you accept; the Decision Log stays the single owner of unresolved rules.

Items already tracked as D1–D5 are listed in §5 and are not repeated here, except where a settled rule collides with one of them.

Severity:

- **Blocking** — a table hits this in ordinary play and cannot proceed without a ruling.
- **Ambiguous** — play proceeds, but two tables will reach different answers.
- **Editorial** — text or packaging, no mechanical effect.

> **Repository note (2026-09-23, closed 2026-09-24).** The three legacy files in `drafts/` were replaced with relocation notices before `drafts/` was ever committed, so no commit, stash, or reflog entry holds the pre-restructuring text. **It is not recoverable**, and the migration therefore cannot be checked against its source as [the restructuring plan](VBG_2.2_RESTRUCTURING_PLAN.md) §6 asks. This is recorded as a known gap rather than a pending task: the 2.2 set has since been rewritten from the Decision Log rather than from the legacy draft, so the legacy text is no longer the authority for anything. `drafts/` is committed from 2026-09-24 onward, which stops the same thing recurring.

## 1. Blocking

| ID | Item | Where it bites | What a ruling must state |
|---|---|---|---|
| Q1 | **Conditional responses have no rules.** The post format includes "any conditional response" ([Player Rulebook §4](../../drafts/vbg-2.2/Player%20Rulebook.md), §9 quick reference, and the sample post), but nothing defines what one costs. | Every threat scene. In the sample post, Vey's conditional — a flame barrier — is a second ability use, so as written it would need a second Major Action and more Strain than the post accounts for. | Whether a triggered conditional costs an action, costs Strain, requires a roll, and whether it draws against the current cycle or the next one. |
| Q2 | **Whether responding to a threat consumes the Major Action.** Creature cards prescribe a "Response / TN" as though the player rolls ([Creature Blueprint §3.1](../../drafts/vbg-2.2/Creature%20Blueprint.md)), but the Player Rulebook only lets one roll cover an action and a threat "when the action addresses it." | Every threat scene. Determines whether a character can act and defend in the same cycle, or must spend the whole cycle defending. | Whether an unaddressed threat simply applies its consequence with no roll, or whether the player always gets a defensive roll. |
| Q3 | **No resolution order inside a cycle.** All posts resolve together, with no sequencing rule. | Any group fight. Two players hit a Standard creature with 2 Resistance in one cycle; the second hit has no target. Same problem when a character is Downed by a threat in the cycle they also declared an action. | Whether simultaneous actions all take effect, whether excess damage is wasted or redirected, and whether a character Downed during a cycle still resolves their declared action. |
| Q4 | **Armor has no acquisition path.** Characters start with none, starting gear cannot include Armor, and no PP upgrade grants it. There are no purchase, loot, or economy rules anywhere in 2.2. | The entire Armor subsystem — absorption, repair, material units, scrap — is unreachable in play. | How a character first obtains Armor. Overlaps D2, but D2 only covers what items *are*, not how they are acquired. |
| Q5 | **Nothing in the settled rules deals more than 1 damage.** A hit deals 1 unless a rule says otherwise; abilities explicitly decouple scale from damage ("costs measure scale, not damage"); weapons are pending under D2. | All combat until the Item Glossary lands. A Boss at 5+ Resistance takes five successful hits, and a 2-Strain Major-scale ability hits as hard as a punch. | Whether >1 damage is intended to come only from items, or whether ability scale, Critical Success, or creature weaknesses can also produce it. The Creature Blueprint already references "one specified 2-damage hit" with no rule that produces one. |
| Q6 | **Escape has no distance or difficulty.** Escape costs a Major Action dedicated to getting away; the [GM Guide §4](../../drafts/vbg-2.2/GM%20Guide.md) then forbids the obvious fix — "do not treat escape as a fixed movement multiplier" — without supplying an alternative. | Any flight or pursuit. A successful escape has no defined destination band. | What a successful escape achieves: a band change, removal from the scene, or a GM-set fictional position, and what TN applies. |
| Q25 | **The worked example never pays for its own ability.** Vey's Strain moves 4 → 3, which covers only the Success-with-Cost payment; the flame burst's own cost is never stated ([Player Rulebook §9](../../drafts/vbg-2.2/Player%20Rulebook.md)). | Every ability attack. The example balances only if a targeted burst is Minor scale (0 Strain), but §5 describes a substantial effect on one target as Standard scale (1 Strain), which would give 4 → 2. | What a targeted single-creature ability costs, after which the example needs correcting. Narrower than Q5: this asks the cost, not the damage. |

## 2. Ambiguous

| ID | Item | Where it bites | What a ruling must state |
|---|---|---|---|
| Q7 | **Who judges Trait relevance.** "Add one relevant Major Trait (+2) and one relevant Minor Trait (+1) at most" never says who decides relevance. The GM Guide covers TN vetoes but not this. | Every single roll — the most frequent judgment in the game. | Whether the player asserts relevance subject to GM veto, matching the TN-proposal pattern, or the GM approves it up front. |
| Q8 | **"Base combat" at TN 10 versus "Standard combat" at TN 15.** The TN table gives combat two entries with near-synonymous labels; the GM Guide's difficulty guidance does not mention combat at all. | Every combat TN call. | What distinguishes base from standard combat, or drop one label. |
| Q9 | **Physical versus non-physical damage is undefined.** Armor "absorbs physical damage" only. Nothing defines non-physical damage or says whether open-ended Domain effects — fire, force, cold — count as physical. | Constantly, because Domains are open-ended by design. Decides whether Armor is useful against the game's most common attack type. | Either that all damage is physical unless stated, or a definition of the non-physical category and what interacts with it. |
| Q10 | **Strain Transfer may pre-empt the pending stabilization rules.** Strain Transfer is settled and restores Strain 1:1. A Downed character is at 0 Strain. | A healer appears to be able to restore a Downed character to consciousness with a settled rule, which would make the D1 stabilization procedure largely moot before it is written. | Whether Strain Transfer can target a Downed character at all, and if so whether it ends the Downed state or only stops the clock. Resolve alongside D1. |
| Q11 | **The missed-post default cannot apply to a Downed character.** "If a player misses the window, their character takes cover or follows the group where possible." | Any cycle in which a Downed player also misses their posting window — a realistic pairing. | What happens to a Downed character whose player misses the window, given the in-fiction treatment deadline is still running. |
| Q12 | **"Once per scene" recovery with scene boundaries undefined.** Catch Your Breath recovers 1 Strain "after a threat ends, once per scene"; the scene/cycle relationship is pending under D5. | Multi-wave fights and long dungeon sequences. | Depends on D5. Flagging it so the D5 ruling explicitly covers recovery frequency, not just timing terminology. |
| Q13 | **No GM guidance for character-creation approval.** The GM Guide covers scenes, adjudication, threats, movement, Downed characters, creatures, and authority — but never Domain approval, despite "GM-approved" appearing throughout the Player Rulebook. | Every new character. The only constraint given is "cannot produce miraculous or unlimited effects." | What makes a Domain scope acceptable, with accepted and rejected examples. Likely a new GM Guide section rather than a Decision Log entry. |
| ~~Q14~~ | ~~**2.2 has no trait catalog.**~~ **Settled 2026-09-24:** 2.2 ships none and does not adopt the v1.4.2 lists; traits stay fiction-first, and a module supplies its own. [Port Vane Traits](../../drafts/port-vane/Traits.md) is the worked example. | — | — |
| ~~Q15~~ | ~~**Only threat play has a procedure.**~~ **Settled 2026-09-24:** non-threat play is deliberately freeform — §2 resolution, no cycle, no action economy. Long travel is the one exception and uses a Transition Scene. | — | — |
| ~~Q16~~ | ~~**Stat allocation edge cases.**~~ **Settled 2026-09-24:** all 6 points are spent, no Stat drops below −1 to fund another, and +2 / +2 / −1 is legal and intended. | — | — |
| Q17 | **Sustained effects and the single Major Action.** Maintaining a sustained effect "needs the same action type each later cycle." | A character maintaining one Major-scale effect has no Major Action left, so a second is impossible. Derivable but never stated. | State the limit explicitly, or allow maintenance to drop to a Minor or Free Action. |
| Q18 | **Overlapping hazards.** "Entering and remaining in the same hazard do not cause separate damage twice in that cycle" covers one hazard only. | Two players creating overlapping hazards, a common Domain combination. | Whether two distinct overlapping hazards deal 1 damage each or 1 total. |
| Q26 | **Two different TN-veto standards.** The Player Rulebook lets the GM veto "a difficulty that is too low" (§2); the GM Guide says to reject a proposed TN "only when it does not fit the fiction" (§2). | Every player-proposed TN. The second wording also covers an inflated TN; the first does not. | One standard, owned by the Player Rulebook, with the GM Guide pointing to it instead of restating it. |
| Q27 | **Partial posts have no rule.** The missed-window default covers silence only ([Player Rulebook §4](../../drafts/vbg-2.2/Player%20Rulebook.md)). | Any cycle where a post declares a Major Action but omits the Minor Action or movement. | Whether omitted parts are forfeited, defaulted like a missed post, or queried before resolution. |

## 3. Editorial

| ID | Item | Fix |
|---|---|---|
| Q19 | **"Declared Action" is capitalized like a defined term** in the Major Action table but is never defined; §2 uses "declare the action" in lower case. | Define it in Player Rulebook §1 or lower-case it. |
| Q20 | **No licence, author credit, or contact.** The repository has no `LICENSE`, and no document names an author or a way to report a rules problem. | Required before any genuine public distribution. Decide a licence — a Creative Commons licence is common for tabletop rules, though I would not assume which one fits your intent — and add a credit line to the index. |
| Q21 | **Filenames contain spaces**, so every link needs `%20` encoding. | Optional. Kebab-case would be cleaner, but renaming breaks any links already shared. |
| Q28 | **"side-initiative" appears once and is never defined** ([Decision Log §1](../../drafts/vbg-2.2/Decision%20Log.md)). It is absent from the Player Rulebook key terms, against the convention E4 sets. | Delete the phrase, or define it in Player Rulebook §1. |
| Q29 | **"Condition", "Weakness", and "vulnerability" overlap.** Player Conditions are injuries; creature conditions are defeat requirements; GM Guide §6 says "vulnerabilities" where the card field is "Weaknesses". | Use one name per concept. Keep the card field "Weaknesses", and qualify creature conditions wherever both meanings appear. |
| Q30 | **The Bridge Brute does not follow its own template.** It uses singular "Strength:" / "Weakness:" and a single Behavior sentence, against the plural fields and the Goal / Approach / Retreat split in [Creature Blueprint §3.2 and §3.4](../../drafts/vbg-2.2/Creature%20Blueprint.md). | Match the example to the template fields, since it is the only worked card in the set. |

## 4. Outside 2.2, blocked on it

| ID | Item | Detail |
|---|---|---|
| Q22 | **VBG-Z has unresolved internal contradictions.** | [BASELINE_COMPARISON.md](BASELINE_COMPARISON.md) lists ten, including Strain capacity, stat cap, whether natural recovery is overridden, Noise Clock start value, called shots, Armor wording, and firearm data. Blocking only if VBG-Z is distributed; 2.2 does not touch them. |
| Q23 | **The West Marches module is partly unblocked.** | [West_Marches_Checklist.md](../../to%20do/West_Marches_Checklist.md) line 14 deferred the resolution engine, health overrides, death and rescue procedures, and a Hub economy. The 2026-09-24 rulings supply all four: the cycle, the Downed and death procedure, and the Item Glossary's acquisition paths and value bands. Party size and absent-player handling remain module questions. Note that Port Vane runs a player-centric campaign instead, so this module may not be wanted. |
| Q24 | **What 2.2 *is* relative to the v1.5 plan is unstated.** | [REFINEMENT_BACKLOG.md](REFINEMENT_BACKLOG.md) §1 asks whether the base game should adopt d20 at all and proposes a `VBG v1.5 design decisions.md`. VBG 2.2 answers that question in practice by settling on `1d20 + Stat`, but nothing records whether 2.2 *is* the v1.5 revision, supersedes the backlog, or runs in parallel. |

## 5. Already tracked

These remain open in the [Decision Log §2](../../drafts/vbg-2.2/Decision%20Log.md) and are not duplicated above:

- ~~**D1**~~ — settled 2026-09-24.
- ~~**D2**~~ — settled 2026-09-24; the Item Glossary was written in the carry-through pass the same day.
- ~~**D3**~~ — settled 2026-09-24 in the carry-through pass. PP awards have a scale.
- ~~**D4**~~ — settled 2026-09-24. A Critical Success may not add damage.
- ~~**D5**~~ — settled 2026-09-24. Scene and cycle are defined; there is no round or turn.
- ~~**D5a**~~ — settled 2026-09-24 in the carry-through pass. Transition Scene has a procedure.

**The Decision Log's pending list is empty.**

## 6. Suggested order

> Superseded by the 2026-09-24 rulings; kept as the record of how the work was sequenced.

Q1, Q2, and Q3 are the tightest knot: all three concern what one cycle actually contains, and answering them separately risks contradiction. Settle them together, then D5, since the timing vocabulary depends on the same model.

Q5 and Q4 then unblock D2, because the damage ceiling and the acquisition path determine what item statistics need to exist. Settle Q25 with Q5: both ask what an ability's numbers are, and the worked example cannot be corrected until they exist.

Everything else can be resolved independently. The repository note above is not a rules question and can be settled at any time, but it stops being fixable once `drafts/` is committed.
