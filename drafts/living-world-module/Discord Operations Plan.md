# Living World — Discord operations plan

**Status:** design proposal, not a configured server · **Revised:** 2026-09-24  
**Owns:** channels, permissions, records, continuity, staffing, and onboarding.

## 1. Server structure

Use a small number of forums with one post per scene or record. Discord forums support tags, guidelines, and channel permissions, and require a Community-enabled server. Use ordinary text channels with scene threads if Community is unsuitable. Tags organise posts; they do not provide private access. [Discord's Forum Channels FAQ](https://support.discord.com/hc/en-us/articles/6208479917079-Forum-Channels-FAQ)

| Category | Proposed channels | Purpose |
|---|---|---|
| Start here | `start-here`, `rules-and-boundaries`, `announcements` | Reading order, rules version, conduct, current situation. |
| People | `introductions`, `characters` forum, `find-a-scene` | Character records, invitations, timezone and pace matching. |
| City | `city-bulletin`, `locations`, `street-scenes` forum | Ratified developments, location cards, player-led scenes. |
| Action | `combat-scenes` forum, `adjudicated-scenes` forum, `projects` forum | Runner-led PvE, staff-led investigations/events, and world-changing work. |
| Records | `scene-logs` forum, `requests-and-transfers` forum, `rules-rulings` | Closure summaries, pending changes, reusable rulings. |
| Community | `general`, `help-and-feedback`, optional voice room | Out-of-character conversation and support. |
| Staff | Private review queue, world notes, moderation reports | Hidden information, decisions, escalations, incident records. |

Suggested scene tags: `open`, `arranged`, `needs-dm`, `active`, `paused`, `awaiting-review`, `closed`; add location and scene-type tags only when useful. The header's fields remain authoritative if tags are stale. Put concealed-faction and private scenes in access-restricted channels; public titles must not reveal secret memberships.

Do not create a channel for every building. A location card and linked scenes establish a persistent place without splitting conversation across an empty map. Public faction information can share one directory; create private faction spaces only when actual play requires them.

## 2. Roles and authority

| Role | May do | Does not imply |
|---|---|---|
| Member / player | Open permitted scenes, propose projects, submit logs | Edit canonical rewards, sheets, NPC reactions, or faction standing. |
| Scene host | Maintain a scene header, invite participants, compile agreed summary | DM powers over opponents, NPCs, or world facts. |
| Encounter runner | Run approved packet families; apply their immediate tactical results | Own-PC participation without a play-and-run endorsement; new world powers or self-awarded rewards. |
| Play-and-run runner | Participate while applying a public deterministic packet | Hidden tactical information, discretionary own-PC benefits, or authority over PvP. |
| Encounter reviewer | Validate fixed packet claims when independently endorsed and uninvolved | General economy, standing, permanent harm, or own/shared-asset rewards. |
| DM / world steward | Resolve assigned scenes, ratify consequences, update assigned records | Approve benefits to their own PC without another reviewer. |
| Moderator | Handle conduct, privacy, participation disputes, channel order | Adjudicate mechanics unless also appointed a DM. |
| Administrator | Configure permissions and maintain access/backups | Override an agreed fiction or rule through undocumented edits. |

People may hold several roles. [Encounter Running](Encounter%20Running%20Plan.md) owns their precise scope and endorsement requirements. Staff and endorsed players may run an encounter they play in under that procedure; they cannot decide their own disputed benefit, reward, lasting injury, or faction outcome. Publish an independent reviewer and correction/appeal route. Resolve player conduct outside the fiction, without extra character harm as punishment.

## 3. Canonical records and review

Maintain these minimal records before choosing automation:

| Record | Minimum data |
|---|---|
| Character | ID, owner, approved version, traits/Domains, Strain/Armor/injuries, inventory, PP, memberships, current scene. |
| Scene | ID, rules version, cast, location, fictional time, opening snapshot, stakes/consent, state, conclusion link. |
| Encounter registration | Packet/instance ID, runner endorsements, reviewer, allowed party variant, location/time reservation, reward allowance, monster policy and map version. |
| World change | Event ID, source scene, decision, affected records, DM, effective fictional time. |
| Asset or exchange | Item/claim ID, owner, quantity/slots, reservation, debit/credit, approving actor and authority/endorsement. |
| Project / clock | Owner, scope, progress, evidence, next obstacle, completion condition. |

**Review path:** host submits agreed summary → queue checks completeness → assigned DM, or endorsed independent reviewer for fixed packet claims only, validates or returns the request with a reason → record the decision once → update affected records and publish only appropriate public information. New world rulings and mechanical exceptions stay with DMs.

Every self-run scene gets batch review, including personal scenes. Personal conclusions may guide later conversation under the [roleplay proposal](Player%20Roleplay%20Module%20Plan.md). Ordinary social scenes cannot grant resources or world changes. In authorised PvE, tactical state, expenditure, and approved recovery apply immediately under the packet; new rewards await independent validation, and lasting harm/broader consequences go to staff. This explicit delegation allows successive fights using the current resource snapshot without a live DM or a completed payout review. Staff silence never approves a claim.

Review summaries, not every line of ordinary dialogue. Read underlying posts for disputed claims, hidden-information questions, or an occasional consistency sample. Correct only affected consequences and inform participants; avoid rewriting an entire relationship because an unrelated requested reward failed review.

Keep an append-only decision history. Owners may correct presentation; mechanical changes require a recorded ruling. In a manual pilot, a staff-owned register plus scene links is sufficient. Export a dated snapshot weekly and before rules migrations; keep private records private in copies.

## 4. Time, parallel scenes, and absence

Three clocks serve different purposes: the real-world response window, a scene's fictional time, and the publication schedule for world updates. They are never interchangeable.

- **Concurrency proposal:** one mechanically consequential present-time scene per PC, plus up to two personal scenes whose chronology is declared. Do not commit the same resources to concurrent outcomes.
- Label social scenes earlier, current-compatible, or explicitly retrospective. They cannot invent earlier healing, equipment, information, or preparations to change an already declared consequential scene.
- Reserve the location/time and resources of unresolved consequential scenes. Before another scene could affect them, the DM either links the scenes under one event, sequences them, or moves the new scene elsewhere. Being first to post is not authority to settle the other's outcome.
- An unresolved battle can span several real-world world-update days. Unrelated locations can develop; its participants and contested area remain tied to their scene snapshot. Publication is not a city-wide time jump.
- Recovery follows elapsed safe fictional time and the approved harm rules. Starting more threads cannot create extra rests or Catch Your Breath uses. Long travel remains dependent on D5; no instantaneous transit through Discord channels.
- Keep the baseline up-to-24-hour threat posting window. Proposed personal-scene target: reply within 48 hours; after 72 hours without response, participants may close only to the last mutually established state under their agreed absence convention.
- Silence grants no consent, surrender, item transfer, permanent harm, or new declaration. Threat scenes use the baseline missed-post default and approved Downed procedure; a player may preauthorise a bounded fallback at entry.
- Announced leave closes or pauses personal scenes by agreement. A DM resolves a safe handoff for active threats where fiction allows; absence is not invulnerability and is not a real-time death timer.

## 5. Staffing and capacity

**Confirmed staffing:** 2–3 DMs/world stewards, with authorised players also running fights. Recruit and train a trial pool of 4–6 volunteer runners; their availability is a dependency, not an already confirmed resource. Trial 8–12 aggregate staff hours plus 8–12 distributed runner hours weekly. Keep these budgets separate.

| Workload example | Weekly staff time |
|---|---:|
| 24 routine closure reviews × 4 minutes | 96 minutes |
| 8 complex consequence/transaction reviews × 12 minutes | 96 minutes |
| 10 player-run encounter reviews × 8 minutes | 80 minutes |
| 1 staff-led threat scene × 3 resolutions × 20 minutes | 60 minutes |
| World update and coordination | 45 minutes |
| Onboarding, packet preparation, training, and rulings | 90 minutes |
| Moderation/overrun reserve | 90 minutes |
| **Illustrative staff total** | **557 minutes, about 9.3 hours** |

During training, open two player-run fights and one staff-led fight concurrently. Scale toward 4–6 concurrent runner-led fights and roughly 8–12 completions weekly as endorsement and review capacity allow. At four PCs per fight, that offers roughly 32–48 weekly participation slots; it is not a quota or guaranteed schedule. Keep one consequential scene per PC and normally one active fight per runner.

Ten runner-led fights at three cycles ×20 minutes require roughly 10 distributed runner hours, in addition to the staff estimate above. Each needs a named runner, a permitted handoff substitute, and an independent closure reviewer. A live staff DM or staff backup is not required for routine packet resolution. Staff-led bespoke encounters have their own primary/backup coverage. Social play and the [project capacity](World%20Systems%20Plan.md) continue alongside combat.

Review logs twice weekly and publish one concise world digest weekly. These are service schedules, not play windows. Each batch clears routine summaries first while complex requests receive an owner and next-update date. Treat an active scene's necessary ruling and a player conduct issue ahead of optional new content.

If requests exceed seven days or encounters repeatedly miss their agreed cadence, limit new work in the affected queue and publish capacity. A payout backlog does not erase existing costs or prohibit an otherwise legal new fight; a disputed injury/resource prerequisite does. Add endorsed runners/reviewers, simplify packets, or narrow active districts before expanding beyond capacity. Never silently approve backlogs.

## 6. Onboarding and re-entry

1. Read the short premise, authority split, boundaries, and current rules version.
2. Propose one character with a personal want, a useful skill, and a reason to care about a neighbourhood. Every new Port Vane PC begins a Stray.
3. DM approves the character against the tested trait/Domain/item list, including any adopted Domainless variant.
4. Offer three different invitations: a social gathering, an existing player's ambition, and an active local need. None requires combat or faction membership.
5. Pair the newcomer with a willing player contact and an open scene. The first scene can be entirely player-run.
6. Show how to close the scene and submit one summary. Ask for feedback after their first week.

For returning players, provide a short “what changed” digest, reconcile their last scene and records, and offer new connections. Do not charge fictional debts or consume medication just because the player was away.

## 7. Tooling sequence

**Manual pilot first:** templates, staff-owned register, timestamps, and links. No custom bot is required to test whether the game works.

Once procedures stabilise, consider tools for scene IDs, deadline reminders, dice audit trails, form submission, and read-only sheet summaries. Automate calculations and duplicate checks before automating rulings. A bot must not award standing, resolve consent, invent loot, or advance a world clock merely because messages arrived.

Before opening the server, test access with ordinary player, runner, reviewer, and staff views: public scenes are readable, concealed memberships remain private, canonical awards require the appropriate independent reviewer/DM authority, and a former participant does not retain unintended private access. Those checks validate this proposed layout; no live Discord changes are part of this planning task.
