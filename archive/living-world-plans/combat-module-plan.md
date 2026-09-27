# Living World — Combat Module Plan

> **Archived 2026-09-27 — historical material, not current rules.** Setting references describe a removed setting. Use the repository’s `rules/` and `modules/` indexes for current material.

**Status:** design proposal, not playable or balanced rules · **Revised:** 2026-09-24  
**Owns:** the proposed optional combat module, its local overrides, development work, and acceptance tests.  

> **Superseded in part (2026-09-24).** The VBG 2.2 baseline has since settled that **every hit deals exactly 1 damage, permanently**, and that weapons grant effects rather than damage ([Decision Log](../../rules/decision-log.md) §2a). Every proposal below that assumes a 2-damage pattern needs rewriting as an *effect* — a condition it defeats, a defence it breaches, a band it reaches — before it can be commissioned. Gear acquisition is no longer a gap: see [Item Glossary](../../rules/item-glossary.md) §2.

**Confirmed brief:** VBG 2.2; Port Vane; 20–40 active players; mostly asynchronous; frequent combat; authorised player-run and simultaneous play-and-run monster fights; rich combat and novel-feeling precise movement; PvP by consent with agreed stakes and staff handling lasting consequences.

## 1. Design target and boundary

Combat is a principal activity of this server. Build a repeatable tactical engine for frequent fights: protecting someone, breaking containment, recovering evidence, escaping a debt collector, or holding a bridge. Depth comes from interacting movement routes, firing lanes, action commitments, weapon roles, counters, and objectives. Ordinary roleplay remains available between and alongside fights.

Use 2–5 characters per encounter for the first pilot. Six is a stress test, not a server population limit. Larger incidents divide into linked objectives, each with its own thread and facilitator; one character occupies one active threat scene. Campaign time and reconciliation belong to [Discord Operations Plan](discord-operations-plan.md).

[Encounter Running](encounter-running-plan.md) owns who may run these fights, including playing a PC while running. [Movement and Positioning](movement-and-positioning-plan.md) owns the proposed position-and-route battlefield. The same mechanical inputs must produce the same answer under different authorised runners.

This plan neither changes the base draft nor fills its pending entries by implication. An adopted module needs a versioned rules pack and explicit overrides. A scene names its version before rolls; characters never switch systems midway to improve an outcome.

| Preserve from [VBG 2.2](../../rules/player-rulebook.md) | Add or resolve locally before testing |
|---|---|
| d20 + Stat + at most one Major and one Minor Trait; four result bands | Consistent threat response, conditional action, and resolution order |
| Force, Finesse, Focus; existing progression limits | Tactical choices with opportunity costs; no extra ability scores |
| One Major, one Minor, movement; announced threats; creatures do not roll | Bounded responses, team setup, cover, escape, and objective procedures |
| Strain as both harm capacity and ability fuel; ability costs 0/1/2 | Explicit damage permissions, bodily harm categories, and treatment |
| Resistance as each creature's only defeat track | Distinct behaviors, discoverable protections, and multi-objective encounters |
| Reach / Close / Far / Distant as effect-range labels | C9 replaces estimated tactical distances with exact position, route, and attack-lane data; adds a paid Drive action |
| Scale distinct from damage; limited trait stacking | Reviewed Domain patterns, Domainless options, and equipment tags |

Draw inspiration from VBG-Z's telegraphed enemies, loadout choices, cover, and shared escalation. Do not import its incompatible free counters, Sprint action, monster Armor, infection, no-natural-recovery rule, or equipment numbers. [The baseline comparison](../../docs/baseline-comparison.md) records its unresolved contradictions. Published v1.4.2 traits and abilities supply concepts only: their d10 assumptions, extra starting Minor Trait, Miracle scale, and automatic critical recovery do not carry over.

## 2. Decision and override register

**C IDs below are proposed module decisions.** D IDs refer to the [base Decision Log](../../rules/decision-log.md); Q IDs refer to [revision review findings](../revision-notes/open-questions.md); P IDs refer to Port Vane questions (removed setting; historical reference). Resolve locally for the pilot, then reconcile with any later base revision. None is already approved.

| ID | Proposed choice | Existing gap or departure | Required before |
|---|---|---|---|
| C1 | Lock declarations; entry maneuvers, opening movement, setup, simultaneous main actions/threats, fallout, closing movement; reserve one Minor defense | Q1–Q3, Q27; D5. Defines action budgets and distinct position snapshots | Any combat pilot |
| C2 | Permission-based setup, cover, control, and explicit escape destinations | Q6–Q8, Q17; D4–D5. Adds bounded tactical effects | Tactical cards |
| C3 | Default 1 damage; explicit 2-damage patterns; one source of added damage; declared Armor coverage | Q4–Q5, Q9, Q25; D2/D4. Adds currently missing higher damage and gear acquisition interface | Gear and Domain tests |
| C4 | Field stabilization stops deterioration but does not restore combat actions; recovery has one logged boundary | D1; Q10–Q12, Q18. Downed treatment and hazard timing require local decisions | Any lasting harm |
| C5 | A Domainless character may replace the required Domain with a bounded training package; Domain patterns emit loudness events | P1; Q13–Q14; D3. Domainless creation explicitly departs from base §3 | Port Vane creation |
| C6 | Tier difficulty comes from objectives, reach, protections, and threat budget before inflated TNs or Resistance | Q5/Q8; creature blueprint extension | Tier II/III encounters |
| C7 | Consent and agreed stakes govern PvP; staff ratify lasting consequences; use a separately tested opposed procedure | Base supplies no PC-versus-PC combat procedure | Contested PvP |
| C8 | Publish one approved local equipment/technique catalog with costs, slots, permissions, and progression interfaces | D2–D4; Q4/Q14; P4/P5 | Persistent rewards |
| C9 | Position-and-route movement, independent firing lanes, 2 Pace split movement, Major Drive +2 Pace | Explicitly replaces core §4 estimated movement distances and no-Sprint restriction; ownership in Movement and Positioning | Any mapped fight |
| C10 | Deterministic monster policies and reusable packet rulings for authorised runners, including play-and-run | Local scoped delegation of Campaign Format §2; no self-awarded benefits | Player-run PvE |

## 3. Candidate cycle: decisions without reply chains

**C1 prototype:** keep the base player posting window of up to 24 hours. Aim for one complete declaration per player per cycle. The facilitator can resolve sooner once everyone has locked a post; arrival order grants no tactical advantage.

1. **Brief.** Publish opening positions, movement priority, monster routes, exact threat IDs/TNs, triggers, interruption conditions, and objective/failure conditions. Lock monster decisions before PC declarations; a play-and-run host then locks their own PC's post before others' dice.
2. **Declare and lock.** Name the Major's stage, Minor/defense trigger, pre-route, action position, post-route, threat answered, cost choice, and one fallback. Reserve resources against the same opening snapshot. No changed objectives, Traits, or branches after visible dice.
3. **Entry and opening movement.** Resolve entry Majors, then opening routes and crossing triggers under Movement. An entry Major consumes the actor's only Major. A unit Downed during traversal cannot act afterward.
4. **Setup.** Resolve setup from reached positions, then freeze the action snapshot. Setup cannot benefit from another same-cycle setup. State which permissions, lanes, and protection changed.
5. **Main actions and responses.** Validate range, target, and method against that snapshot; resolve legal actions and remaining threats simultaneously. An interruption cancels its named threat only. Ordinary damage does not retroactively cancel all of a creature's announced attacks.
6. **Fallout and closing movement.** Use Movement §4's single ordering rule for harm, control/features, forced movement, and closing routes; also record attention events. Publish the final snapshot and exact resource deltas. Newly attracted enemies get warnings and a response window before attacking.

For step 5, preserve a valid declared action if its actor is Downed by incoming harm in that same batch. **Last-Strain exception for a main-stage Major:** commit its full activation and declared Strain cost before remaining main-stage defenses; if it exhausts the actor, resolve the Major but cancel any still-unused reserved Minor defense and sustained effects. An earlier crossing defense already resolved in step 3 stays resolved. At other stages, an effect spending the last Strain completes and then causes Downed before later actions. A still-untriggered conditional spends nothing. Reserve expenditures legally at lock and never borrow future Strain; this exception does not let a unit Downed during opening movement act.

Lock each Minor to a named checkpoint: **before entry**, **before opening movement**, **before/after the actor's Major**, or **before closing movement**. All still spend the same one Minor; a reserved defense uses its printed trigger instead. This makes drawing a weapon or picking up a casualty before movement legal and auditable. Setup and entry Majors use the same budget as attacks. Each roll's cost/critical menu must come from its approved entry; own-PC creative exceptions require the Encounter Running review path.

Recheck resource affordability immediately before an effect begins, including after traversal harm or earlier defenses. If a reserved 2-Strain Major now has only 1 Strain available, use its legal locked affordable fallback or cancel its effect while retaining the spent action commitment. Never overdraw Strain or substitute a stronger free effect.

For a Major that both attacks and directly answers a threat, publish **one combined TN: the higher of the attack's adjusted TN and the threat's adjusted response TN**. Apply each relevant cover adjustment to its own requirement before choosing that maximum; use the declared method's applicable Stat/Traits and one allowed setup bonus. One outcome then governs the linked objective and threat. This explicitly resolves unequal attack/response difficulties; indirect attacks still do not supply defense.

If two valid attacks defeat the same target in the batch, both execute and pay their costs; excess damage is lost. A fallback is available only when its primary target is already invalid at that action's resolution snapshot, not because another simultaneous attack would have sufficed. This eliminates incentives to wait for everyone else's dice.

If an action cannot legally begin and has no legal locked fallback, its action commitment is spent but unactivated Strain/ammunition is not. Once begun, failure or simultaneous overkill gives no refund. A newly invalid monster target is not replaced unless its prepublished policy includes a replacement selector.

### Response budget

| Declaration | Commitment | What it can accomplish |
|---|---|---|
| Attack or maneuver that directly answers a named threat | Major; ordinary movement as allowed | One roll resolves its declared objective and that threat, if the method actually prevents it |
| Defend, protect, or escape as the main objective | Major | Resolve the declared protection; broader coverage requires a fitting approved effect |
| Reserve a mundane defensive response | Minor; one trigger and one target | One separate defense roll against one still-unanswered threat; no damage, counterattack, or free reposition beyond the declared route |
| Conditional 1–2 Strain Domain response | Reserve Major and its Strain; name trigger stage/window | Replaces the main action if triggered; only after that window closes may a locked alternative resolve at a stage allowed by its entry, never both |
| Attack and an unrelated incoming threat | Major plus reserved Minor defense, or accept the announced consequence | The attack does not provide automatic defense |
| Failed action or failed response | Existing commitment | Apply its consequence; never add a new reaction roll to undo failure |

An ordinary defense uses the threat's TN and result bands. Success with Cost prevents the threat and pays one fitting published cost; Failure applies the announced unresolved consequence. Do not automatically charge that same damage twice as both failure and an additional penalty. If the reserved trigger never occurs, its Minor stays spent; no late conversion into aiming or equipment handling.

A reserved Minor cannot retry a threat that the same PC already attempted to answer with their Major. It may cover a different named threat. A separately declared ally intervention still resolves on its own merits; a failed roll cannot retroactively recruit a new response.

A closing-movement trigger cannot be declared untriggered during main actions. A reserved Major remains unused until its named window resolves. If its fallback is not legal at or after that window, the unused Major is forfeited; no retroactive main action. Publish these windows on response-capable effects instead of allowing open-ended “if anything happens” declarations.

Multiple incoming threats remain distinct. One defense addresses one threat; withdrawing, suppressing a source, or creating a suitable barrier may answer more only when its scope is declared and approved. Creature cards must keep the number of independent threats within the party's practical response budget.

**Absence:** take cover or follow if possible, with no unapproved scarce expenditure; unavoidable announced consequences remain. An omitted Minor or movement means unused, not an extra prompt. A Downed absentee stays Downed and may be carried or treated; absence neither creates consent nor converts the posting window into a death timer.

## 4. Tactical choices and position

Start with the following universal intents; weapon and Domain patterns change how they work, not whether a character may try them. Add no stance subsystem until these choices produce useful tradeoffs.

| Major intent | Payoff to prototype | Opportunity cost or limit |
|---|---|---|
| Strike | Damage one reachable target | Does not protect against unrelated threats |
| Setup / expose | Reveal an opening or remove one named obstacle for an ally | Gives up direct damage; names beneficiary and expiry |
| Control / suppress | Deny a route, move a target, or interrupt a named attack | No default damage in addition; forced movement respects feasible routes |
| Guard / rescue | Cover an ally or move a casualty through a threatened route | Commits protection to a named target and position |
| Objective action | Open the floodgate, detach the sampler, restore the bridge crank | Advances the encounter without necessarily injuring an enemy |
| Withdraw / disengage | Reach a named refuge or leave the encounter by an established route | Uses Major; TN and success destination published before the roll |
| Treat / repair under pressure | Stabilize a casualty or restore one defined capability | Requires access, suitable resources, and a treatment or item entry |
| Drive | Gain the movement owner's +2 Pace | Commits the Major; no extra attack or automatic disengagement |

**Setup tokens:** prototype a single-use permission or advantage against a specific obstacle, expiring at the end of the next cycle. Examples: expose a seam that ordinary attacks can harm; hold a shutter so someone can pass. If a purely numerical benefit is needed, test +2 once; one token per roll, never combined with another setup bonus. Relevance of Major/Minor Traits still comes from the method, with facilitator veto before rolling.

**Minor choices:** draw, hand over, operate a simple control, maintain a Minor utility effect, prepare a cataloged item, or reserve defense. Avoid a universal free +1 Aim: it becomes obligatory while inflating every attack. A specific weapon may trade its Minor for reach or precision, with an explicit entry.

**Position is a resource:** Movement and Positioning owns map capacity, exact route costs, split movement, engagement, directional cover, carrying, elevation, forced movement, and escape. Changing firing angle can remove protection; changing a route can alter who reaches an objective. Use its action snapshot so a closing retreat never erases exposure while attacking.

**Control states:** test *Engaged* (named departure threat), *Pinned* (named contested route), *Exposed* (one stated protection removed), and *Disarmed* (named item inaccessible). Each application states source, affected capability, removal method, and expiry. A fresh application refreshes only a permitted duration; it never stacks an unspecified penalty or eliminates every possible response.

**Technique entries make depth repeatable:** publish shove, grapple/release, disarm/recover, suppress/cross, guard/intercept, aimed shot, and breach as explicit entries. Each needs action stage, eligible targets, reach, TN, full outcome bands, resource cost, one counter, duration, and interaction with cover/forced movement. A maneuver that grants control and damage must explicitly price both; descriptive flourish alone grants neither.

**Weapon differentiation:** make reach, useful lanes, handling, control access, reload cadence, and preparation distinguish weapon families before adding damage. Ensure every family has a useful matchup and a situation where changing method is sensible. Avoid one best attack, mandatory aim bonuses, indefinite denial loops, and reaction chains.

**Consequence menus:** each packet lists affordable Success-with-Cost options for its supported states and bounded critical benefits. A cost cannot secretly add a second creature attack, invent lasting harm, or grant free equipment. If no listed option handles the state, the packet needs revision or an independent exception ruling; the runner cannot downgrade a success to failure because its menu is incomplete.

## 5. Damage, equipment, and recovery

### C3: small numbers, distinct capabilities

- Keep an ordinary hit at **1 damage**. Prototype **2 damage** only on an explicit weapon pattern, Domain pattern, or creature weakness. Do not add all three together; pilot cap is 2 per target per action.
- Reserve new 3+ damage, repeated attack pulses, and armor-bypass patterns for later review. Existing baseline hazards still apply their stated per-cycle damage; this defers added effects, not that rule. Starting characters have 4 Strain; stronger effects can remove response opportunities abruptly.
- A heavy weapon's 2-damage pattern must pay a meaningful commitment: setup, limited ammunition, bracing that spends Minor, or difficult handling. A label such as “rifle” is not enough to claim it.
- A discovered weakness may grant +1 damage up to the same cap or permit injury through a protection. Do not automatically require TN 20 for every called shot: access, precision, and pressure determine the TN.
- Prototype critical benefits as position, a setup token, or an objective opportunity. No automatic extra damage, free attack, or Strain recovery; D4 remains unresolved until a bounded local menu is adopted.
- Distinguish ability activation cost, Success-with-Cost payment, and incoming damage in every ledger. Armor pays physical harm only; it cannot pay activation or generic exertion.
- Before the pilot, define Armor coverage explicitly under Q9. Proposed default: impact, cuts, and projectiles are physical; thermal, corrosive, electrical, and mental attacks state their coverage or bypass on their entry. No spontaneous “magic ignores Armor” ruling.
- Creature protection remains a condition on its Resistance track. Do not give Carrion a second Armor track or produce player armor scrap from their Resistance.

Catalog weapon families by tactical job: compact sidearm, close control weapon, reach weapon, precise long weapon, heavy breaching weapon, restraint tool. Each entry needs range, hands/handling, slots, damage, action costs, uses, noise, and one limitation. Ammunition accounting should begin with explicitly defined magazine/use units; compare it with round counting before committing to either.

Armor requires an acquisition path in [World Systems](world-systems-plan.md): approved purchase, issued equipment, salvage conversion, or a logged loan. Pilot equipment is a test fixture, not an implicit character reward. Keep base repair and scrap boundaries until a local D2 replacement is approved; no inexhaustible loan-and-return repair loop.

### C4: injury and rescue as playable consequences

Retain Strain rather than introducing separate stamina and hit points in the first build. Measure whether Domain users become too fragile before splitting that central resource.

Prototype **stabilization** as a Major Action with a suitable treatment resource and access to the casualty; roll only when uncertain. Success, including with cost, stops the deterioration deadline but leaves the character Downed. Strain Transfer may stabilize and restore Strain within its existing 1:1 limit, but does not itself clear Downed; resuming combat requires a separately defined recovery procedure. This is a proposed D1/Q10 ruling, not existing base text.

Write treatment entries for three traumatic injuries: damaged limb, contaminated wound, and Domain burnout. Each needs a concrete restriction, field mitigation, definitive treatment, cost/time, and staff confirmation where lasting. Do not import numerical penalty stacks or “lose Strain every post.” Temporary control states clear by their own rules, never by inventing medical costs.

Use the base in-fiction rescue deadline, announced when Downed. Base second-hit death remains a major server lethality decision: either explicitly retain it in approved PvE stakes or adopt a stated override; this plan does not silently soften or broaden it. PvP cannot cause death or permanent injury beyond its agreement and staff review.

Track hazards once per source per cycle. Test at most one damaging exposure from overlapping copies of the same effect; distinct hazards need published combined consequences and a fair response. Catch Your Breath occurs once after a threat ends within the same logged scene, not once per wave, new thread, or moderator change. Preserve safe Full Rest; no unannounced VBG-Z recovery override.

## 6. Domains, loudness, and Domainless roles

**C5 Domain pattern template:** scope; legal effects; reach; Minor/Standard/Major scale; action; Strain; damage/control; duration and maintenance; loudness event; interruption; limits; counterplay. Retain creative uses inside approved scope, but pre-approve common attacks, rescues, and control effects so each post does not renegotiate the whole Domain.

Port Vane says Loud Domains “hit harder”; base 2.2 says scale does not determine damage. Resolve that deliberately: selected Loud patterns may explicitly deal 2 damage under C3, while other Loud patterns emphasize control or area. Quiet patterns earn useful perception, access, precision, and concealment; they are not universally ineffective versions of combat powers. Every targeted damaging use, including a 0-Strain one, still costs a Major and a roll.

Combat emits **loudness events** to the shared system owned by [World Systems](world-systems-plan.md): location, acting character, pattern, intensity/reach, event time, and source scene. That system decides accumulation, thresholds, decay, and cross-scene effects. Do not create an independent combat clock. Distinguish supernatural Stigma draw from ordinary gunfire; a pistol does not become a Domain beacon merely because it is noisy.

Carrion cards state their response to a visible Domain flare: next-cycle target preference, movement toward its source, or an announced escalation. The card cannot silently invent an immediate unavoidable extra hit. Sustained Major effects continue to consume Major each cycle under base rules; no free second barrier via a conditional.

**Domainless creation is an explicit local override.** Replace the mandatory starting Domain with one reviewed training package of equal design budget; keep starting Strain, traits, slots, and PP limits unless separately changed. Prototype medic, controller, scout, and engineer packages with one small reliable permission and two demanding techniques tied to mundane tools, preparation, or exertion. No free bonus Domain later without a stated conversion rule.

Domainless characters need decisive tasks: safely handle a bridge crank while a flare draws Carrion away; identify seams; evacuate civilians; stabilize an ally; place a restraint; secure evidence; operate equipment inside known limits. Techniques cannot grant arbitrary world facts, bypass staff authority, create infinite supplies, or duplicate every Domain. Strays may begin Domainless; joining the Marshals is an earned affiliation, not a starting membership exception.

Review legacy traits that imply extra gear, armor, movement, carrying capacity, or compulsion. Their descriptions do not grant those mechanics automatically. Avoid adding classes or a second XP currency: any purchasable techniques must map to the progression system owned by World Systems and D3.

## 7. Encounters that scale across the city

**C6:** define win conditions, loss conditions, escape routes, and enemy goals before Resistance. Every encounter should offer at least one meaningful choice besides maximizing damage. Surrender, bargaining, containment, evidence recovery, and evacuation may end violence without clearing every box.

| Port Vane threat | Depth comes from | Pilot constraint |
|---|---|---|
| Tier I Shiverers | Pack routes, light, civilians, limited time to secure a door | Begin with base Minor Resistance; group narration, but explicit threats and targets |
| Tier II Carapace-Render | Discoverable plating condition, coordinated opening, Stigma draw, salvage timing | Begin within base 2–4 Resistance range; tune after 2-damage tests, never assume it is balanced |
| Tier III Cairn-Titan | Separate evacuation, power isolation, breach, and Heart-Cairn objectives; Dead Static disrupts coordination | Staff event with linked small scenes; one event state owner; do not run 20 turns in one thread |
| Human opposition | Motive, cover, morale, surrender, evidence, witnesses | Clear retreat threshold and proportionate consequences |
| Tier IV Cold Silents | Investigation and negotiated stakes before violence | Defer until P6 metaplot authority is resolved; no secret invulnerability surprise |

Add to the creature card: objective pressure, maximum simultaneous threats, Stigma response, environmental interactions, escape consequences, and salvage authority. Components may unlock the main creature's vulnerability but do not secretly introduce another full health pool.

Every threat also specifies its stage, movement, reach/lane, one trigger, cancellation, and one targeting policy: **actor-locked** (named target within printed tracking limits), **position-locked** (named area), **crossing-triggered** (first qualifying traverse in movement priority), or **ordered selector** (public priority and tie-break). A crossing threat resolves once and consumes its allocated threat; it is not another attack at main stage. No post-roll retargeting or improvised extra reaction.

For regular play-and-run packets, make monster priorities, vulnerabilities, and phase transitions public. Difficulty comes from solving them under pressure. Reserve genuinely hidden-information encounters for staff or a nonparticipating runner separately endorsed for those packets. Grow the catalog through different objectives, terrain, mixed creature roles, and reinforcement patterns rather than more identical health pools.

Initial threat-budget hypothesis: at most one ordinary targeted threat per participating PC per cycle; a group threat consumes comparable response capacity rather than being a free extra. Tier II begins below that ceiling; Tier III splits pressure among objectives. Test overwhelm as a telegraphed situation requiring retreat, not an arbitrary action-count increase when staff see good rolls.

At startup, +4 vs TN 15 gives 30% Failure, 20% Success with Cost, 30% Clean, 20% Critical. At +8 it gives 10% / 20% / 30% / 40%. At +5 vs TN 20 it gives 50% / 20% / 30% / 0%. These exact d20 counts show why raising every veteran encounter to TN 20 can erase useful choices for newer characters. Scale objectives, reach, and preparation requirements before escalating TNs.

## 8. PvP within agreed stakes

**C7:** distinguish choreographed conflict, consensual sparring, and contested consequential combat. Any may use the tactical vocabulary, but agreed outcomes need no competitive dice. Consent to an argument, faction rivalry, or ordinary roleplay is not consent to attack, theft, forced capture, or power-based coercion.

Before contested play, record participants, win condition, permitted harm/loss, time window, escape/surrender terms, and staff adjudicator for lasting stakes. Failure never expands those permissions. Consent withdrawal pauses resolution; staff settle or rewind pending consequences under the RP procedure.

The NPC threat engine cannot simply designate one PC as a creature. Prototype **one opposed contest per disputed exchange**: both commit method and relevant bonus before dice; higher total wins its declared limited intent, tie preserves the contested state. Use the predeclared stakes rather than applying both VBG result-band tables independently. A roll can never determine another player's beliefs or consent.

This opposed procedure is a separate explicit override requiring tests for initiative, exchanges involving three or more PCs, defensive commitments, margin effects, stalemates, and unequal progression. Until it passes, offer choreographed bouts with agreed results or staff adjudication; no unsupervised lethal mechanical PvP. Do not publish invented balanced duel rules alongside a still-unresolved PvE defense economy.

## 9. Worked prototype cycle

**Illustration of C1–C6 only.** At a Flats service gate, three characters must open an evacuation route. They begin at legal action positions and declare no movement, isolating action/cost resolution. Movement's own example demonstrates changing positions. Test fixtures have no permanent ownership or rewards.

- Carapace-Render: 4 Resistance; small attacks cannot penetrate intact plating. An accessible seam can be levered open with a setup Major, TN 15, allowing one allied attack this cycle to harm it. A hit through that seam may interrupt its charging posture when declared.
- Threat A: the Render charges Mara; unanswered = 1 physical damage. Interrupt it through the seam, TN 15, or use another fitting defense. Threat B: a Shiverer lunges at Ivo; unanswered = 1 physical damage; evade TN 15. Each has one announced threat.
- Objective: Ivo can release the gate with a Major, TN 10. Success opens the evacuation route. Ordinary fixture tools occupy the declared starting loadouts; no item damage bonus applies.

| Character | Declaration and roll | Resolution |
|---|---|---|
| Mara, Domainless engineer; 4 Strain | Major: lever the seam for Vey; 12 + 4 = 16 vs 15. Minor: draw rope. No reserved defense | Clean setup grants Vey permission to harm the plated target. Mara relies on Vey answering Threat A |
| Vey, Flame Domain; 4 Strain | Major: Standard-scale focused burst through the opened seam, 1 activation Strain, 1 damage, interrupt Threat A; 9 + 4 = 13 vs 15. Proposed cost: 1 exertion Strain. Minor unused | Success with Cost: one Resistance removed, charge interrupted. Strain 4 → 2: 1 activation + 1 cost. Setup consumed |
| Ivo, medic; 4 Strain | Major: release gate; 10 + 2 = 12 vs 10. Minor: reserve evasion of Threat B; 12 + 4 = 16 vs 15 | Gate opens; separate reserved defense succeeds. No counterattack, no free ability, no Strain lost |

Final snapshot: evacuation route open; Render 3/4 Resistance; Shiverer unharmed; Mara 4, Vey 2, Ivo 4 Strain. Vey's pattern emits its agreed loudness event; the Render's next announced behavior prioritizes that flare. No extra untelegraphed attack occurs. The group can now evacuate, continue fighting for salvage, or attempt containment.

If Vey had failed, Mara would suffer the announced 1 damage without a new defense roll. In a separate counterfactual, Vey starts at 1 Strain and rolls a Clean Success: the 1-Strain activation resolves the burst, then leaves Vey Downed. The original Success-with-Cost result would need a different agreed cost because another exertion Strain is unaffordable.

## 10. Build order and acceptance gates

1. **Timing and movement prototype:** settle C1/C2/C9, write the staged procedure and declaration/map templates, and independently resolve identical sample posts with two facilitators. Pass: identical legal actions, threat outcomes, resources, position IDs, and lanes in every case.
2. **Content slice:** build six weapon/tool profiles, three Armor profiles with access paths, three treatment entries, six Domain patterns across Loud/Quiet roles, and four Domainless packages. Each entry includes cost, counterplay, limits, and owning rule reference; no rewards enter the live economy yet.
3. **Encounter slice:** build bridge evacuation, Tier I containment, Tier II salvage, human standoff, and pursuit/rescue. Each tests a different objective; each contains an achievable non-slaughter endpoint and declared retreat stakes.
4. **Controlled pilot:** run at least 12 encounters across new, advanced, and mixed groups; include all-Domainless, all-Domain, and mixed teams, and at least four authorised player-run encounters, two of them play-and-run. Log declaration count, clarification count, time, runner/staff effort separately, selected intents, harm, ability spending, and objective contribution.
5. **Edge-case gate:** check last-Strain casting, Strain Transfer on Downed, simultaneous kills, missing/partial posts, two threats on one PC, overlapping hazards, sustained effects, failed setup, invalid fallback, and an escape route closing. Pass: every case has one reproducible ruling without a new reply chain.
6. **PvP gate:** separately test consent withdrawal, unequal progression, draws, multi-party interference, and surrender. Persistent PvP stays unavailable until the RP agreement and C7 procedure cover each case.
7. **Release gate:** publish local overrides, character migration rules, card catalog, facilitator quick reference, and version pinning. Staff ratify pilot rewards only through the normal world ledger; a balance revision never silently rewrites completed scenes.

Pilot targets, not claims of proven balance:

- At least 80% of cycles resolve from one declaration per player; median at most one clarification across the whole group per cycle; at most two rolls per ordinary player post.
- Ordinary 3–5 player encounters finish in 2–4 cycles; median facilitator resolution effort at most 20 minutes per cycle. Repeatedly longer fights trigger fewer threats or shorter objectives before faster posting demands.
- In objective encounters, at least one third of Major declarations are useful setup, control, rescue, or objective actions. No universal attack pattern exceeds half of all Major choices across differing scenarios.
- Every tested Domainless role makes a decisive contribution in at least two distinct encounter types without needing an improvised permission unavailable to comparable characters.
- Every traumatic injury has an attainable treatment path; no character dies solely because their player missed a real-world deadline. Every resource delta and lasting consequence reconciles to the scene log.
- Compare Domain and Domainless survival, objective contribution, resource consumption, and player-reported choices. Investigate any repeated failure pattern; do not claim parity from one successful encounter or average damage alone.

**Release blocker:** timing, position/route geometry, damage, treatment, Domainless creation, equipment access, and delegated encounter authority must be locally resolved and tested together. More weapon entries cannot compensate for an ambiguous action economy.
