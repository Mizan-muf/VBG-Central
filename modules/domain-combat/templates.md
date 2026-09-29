# Domain Combat record templates

[Domain Combat](README.md) · [Starter sets](domains/README.md) · [Shadows journey](journeys/shadows.md)

**Status:** reusable formats for the standalone draft. [Domain Combat](README.md) owns the mechanics; these templates organize their records. They add no permissions, prices, action allowances, or numerical balance rules.

Replace bracketed prompts. Use **None** for a known absence, **Not applicable** for an irrelevant field, and **Unresolved** for an undecided rule or value. An unresolved cost is not zero. Shared information may be stated once for a catalogue, provided each entry clearly inherits it. Link each acquired record to its advancement entry; keep proposals separate from current permissions.

## Choose the record

| What the player wants | Record |
|---|---|
| An independent subject of influence | [Domain](#domain) |
| A linked new Aspect | [Branch](#branch) |
| One changed permission on the same Aspect | [Domain addition](#domain-addition) |
| A repeatable application or improvement of owned permissions | [Technique](#technique) / [technique improvement](#technique-improvement) |
| An application attempted in the current scene | [Quick improvisation declaration](#improvised-declaration) |
| An effortless, inconsequential application | [Minor Effect](#minor-effect) |
| Development requirements, approval, purchases, and PP balance | [Advancement ledger](#advancement-ledger) |

A branch grants permissions; a technique uses them. Domain mixing uses the normal technique record with each Expression's source identified. A new name, Form, or mastery benefit cannot supply a missing permission.

## Domain

The static Domain record describes its current permissions. Use these fields in this order for every Domain. Keep the fields even when a value is None or Unresolved. Record techniques, purchases, and advancement history separately.

A starting Domain has one Aspect, two Expressions, and one Anchor. Later additions update the relevant field; the format stays the same. The four Anchor entries describe one connection.

- **Name:** [Domain name.]
- **Origin:** Internal Energy.
- **Aspect:** [Precisely what it influences.]
- **Expressions:**
  - [Operation]: [What it does to this Aspect.]
  - [Operation]: [What it does to this Aspect.]
- **Anchor:**
  - Establish: [How influence begins.]
  - Reach: [Where influence can remain controlled.]
  - Maintain: [What keeps the connection active.]
  - Break: [What ends the connection.]
- **Boundary:** [Explicit exclusions, or None beyond the stated permissions.]
- **Tolerance:** [What the user's body can endure; ordinary unless explicitly changed.]
- **Persistence:** [What happens to the effect when control ends.]
- **Mark:** [Bodily location, appearance, and response when the Anchor engages.]

Boundary does not need invented restrictions to fill space. Tolerance grants only what is explicitly written. Persistence describes the effect, not a payment rule. A mark is descriptive and grants no additional ability or weak point.

## Branch

A branch uses the same nine core fields, in the same order, plus its Parent. Restate its permissions rather than writing “same as parent.” Origin remains Internal Energy; start with one Aspect, two Expressions, and one Anchor. Use the advancement ledger for proposals, approval, and purchases.

**[Branch name]**

- **Name:** [Branch name.]
- **Origin:** Internal Energy.
- **Aspect:** [The linked subject this branch influences.]
- **Expressions:**
  - [First operation]: [Meaning for this branch's Aspect.]
  - [Second operation]: [Meaning for this branch's Aspect.]
- **Anchor:**
  - Establish: [How this branch begins influence.]
  - Reach: [Its own control range.]
  - Maintain: [Its own continuing conditions.]
  - Break: [What ends this connection.]
- **Boundary:** [This branch's restrictions.]
- **Tolerance:** [Ordinary bodily tolerance or an explicit approved difference.]
- **Persistence:** [What happens to the effect when control ends.]
- **Mark:** [Site, pattern, and activation; any visual relationship to the parent.]
- **Parent:** [Parent Domain or branch.]

Parent identifies the source Domain or branch; it grants no inherited permissions. Mastered techniques using the branch are separate purchases.

## Domain addition

Use for one permission change to a Domain or a Branch. If it introduces a new Aspect, use a Branch or new Domain instead.

**[Addition name]**

- **Status:** [Proposed / approved for purchase / acquired]
- **Applies to:** [Domain / Branch: name.]
- **Kind:** [Expression growth / Anchor growth / tolerance growth / boundary change]
- **Desired capability:** [What the player wants to do.]
- **Before:** [Exact existing permission or restriction.]
- **After:** [Exact replacement or added permission.]
- **Still applies:** [Unchanged restrictions, including other Anchor conditions.]
- **Learning requirement:** [Agreed experiment, study, discovery, or demonstration.]
- **Mark change:** [Optional cosmetic development, or None.]
- **Acquisition:** [GM approval, agreed PP price, payment status, and ledger entry.]
- **Technique impact:** [What becomes available to improvise; which recorded techniques need separate improvement.]

**Example — Long Reach:** Target: Shadows. Kind: Anchor growth. Before: continuous surface control within Close / Room. After: within Far / Hallway. Still applies: own cast shadow, visible light source, continuous surface connection, all other boundaries. Learning: demonstrate a stable connected extension across a courtyard. PP: unresolved; proposal only. Existing Mastered ranges and branch Anchors remain unchanged. See the [full journey](journeys/shadows.md#2-buy-reach-when-reach-is-the-missing-permission).

## Technique

Use this for a permanent Mastered record or a proposed recipe. An improvised version has no mastery benefit. State one Form, Flow, Shape, Size, and Range; list every Expression application actually used. Use the [keyword options](README.md#keyword-groups); a Shape, Size, or Range label still needs concrete dimensions and delivery.

**[Technique name]**

- **Type / status:** [Improvised recipe or Mastered; proposed / approved / acquired.]
- **Access:** [Required Domains, branches, and specific additions.]
- **Keywords:** [Expressions] : [Form] : [Flow] : [Shape] : [Size] : [Range]
- **Method:** [What the user does; how every Expression contributes to one effect.]
- **Dimensions and delivery:** [Actual dimensions, path, target or area, and any movement distance.]
- **Anchor use:** [How each required Anchor is established and maintained in this method.]
- **Base output:** [Recorded result and limits; mark undecided numerical values Unresolved.]
- **Mastery benefit:** [Specific approved improvement and its conditions; None for improvisation.]
- **Conditions:** [When the output applies; relevant cover, resistance, or exposure.]
- **Requirements:** [Equipment, medium, posture, prior setup, or stored effect.]
- **Action demand:** [Activation, steering, maintenance, and release as applicable.]
- **Expression applications:** [Number, with source and operation for each application.]
- **Base Energy:** [Improvised cost / Mastered cost, calculated from applications.]
- **Other Energy costs:** [Upkeep as N Energy/min, preparation, storage, release, exceptional costs; Unresolved where undecided.]
- **Interruption:** [What spoils execution or ends the effect; what happens to stored effects if relevant.]
- **Aftermath:** [What remains, expires, or returns to normal.]
- **Acquisition:** [Starting Mastered choice 1 or 2, or GM approval, agreed PP price, payment status, and ledger entry; no PP for improvisation.]

For **N** Expression applications, improvised base Energy is **N**; mastered base Energy is **max(1, ceil(N / 2))**. Count repeated applications, not only distinct names. List each source for mixed techniques, such as `Flame—Generate + Air—Compress + Air—Redirect`.

For **Sustain**, specify the **Energy/min** upkeep rate, continuing attention, and Anchor conditions. Generated material with Sustain persists only while that upkeep is paid. For **Accumulate**, also specify the receptacle, capacity, retention conditions, and release method in Requirements, Interruption, and Aftermath. Mark undecided values explicitly. Base execution cost does not settle accumulation, upkeep, or release payments.

### Technique improvement

Change an already Mastered technique's recorded output or execution. Buy a missing Domain permission separately before relying on it here.

**[Improvement name]**

- **Status:** [Proposed / approved for purchase / acquired]
- **Target:** [Existing Mastered technique.]
- **Before → after:** [One specific change to output, benefit, dimensions, or execution.]
- **Permission / method:** [Why owned Domain permissions support the change.]
- **Requirements:** [Any prior addition, branch, or agreed fictional preparation.]
- **Cost and action impact:** [Recount Expression applications if changed; record other affected costs or demands.]
- **Still applies:** [Unchanged requirements, limits, interruption, and aftermath.]
- **Acquisition:** [GM approval, agreed PP price, payment status, and ledger entry.]

After any acquired addition or improvement, update the owning Domain or technique record so the current ability can be read in one place. Preserve the before/after entry as advancement history. An addition does not automatically upgrade recorded techniques or related branches.

## Improvised declaration

This is the quick format for the current exchange. The player supplies intent, method, keywords, and setup; the GM clarifies output, action demand, costs, and risk with the player before rolling.

- **Intent:** [The result I am trying to achieve now.]
- **Method / permissions:** [How I do it, with the source of each Expression.]
- **Keywords:** [Expressions] : [Form] : [Flow] : [Shape] : [Size] : [Range]
- **Setup / limits:** [Valid Anchors, equipment, dimensions, path, and conditions.]
- **Agreed output / action / cost:** [Expected effect; action and movement; N Expression applications = N base Energy; other expenditure.]
- **Risk / interruption / aftermath:** [What can spoil the attempt; consequences and persistence.]

Improvisation costs no PP and grants no mastery benefit. A successful use does not permanently enlarge the Domain or automatically master the technique.

For a chat declaration, use this compact version:

> I want [intent], using [source Expressions and method].
>
> **Keywords:** [Expressions : Form : Flow : Shape : Size : Range].
>
> **Setup/limits:** [Anchors, equipment, dimensions, path].
>
> **Agree before roll:** [output; action/movement; base/other Energy; risk, interruption, aftermath].

## Minor Effect

Use only when the application meets the module's [Minor Effect limits](README.md#minor-effects). Free Energy does not mean a free action.

**[Minor Effect name]**

- **Status:** [Proposed / GM-approved]
- **Access / method:** [Owned permissions and how they produce the effect.]
- **Anchor / scope:** [Connection, small extent, and continuing conditions.]
- **Output:** [An effortless result without meaningful attack, protection, healing, or Energy recovery.]
- **Action demand:** [What the user must do in the current situation.]
- **Cost:** No PP to define; no tracked Energy.
- **Interruption / aftermath:** [What ends it and what remains.]
- **Limit:** [When a more consequential use requires normal technique resolution.]

Minor Effects cannot store power or accumulate material for a larger effect. Repetition does not make a substantial task free.

## Advancement ledger

Use one ledger per character. Track proposed developments separately from actual PP movements. This is optional bookkeeping, not a level system or a new PP award schedule.

**[Character] — advancement ledger**

- **Campaign / player:** [Names.]
- **Opening PP balance:** [Confirmed unspent PP when this ledger begins.]
- **Current PP balance:** [Opening balance + PP received − PP spent.]
- **Starting Mastered choices:** [1: technique link; 2: technique link. Each costs 0 PP.]

### Development tracker

Repeat this entry for each proposed development.

- **Development ID:** [D1]
- **Development / target record:** [Type, desired capability, and record link.]
- **Scene evidence / requirements met:** [Study, discovery, or demonstration.]
- **Requirements remaining:** [Unmet conditions or None.]
- **Agreed PP price:** [Value or Unresolved.]
- **GM approval:** [Pending / approved, date.]
- **Acquisition / transaction:** [Not acquired / acquired, transaction ID.]

### PP transactions

Repeat this entry for each award or purchase.

- **Transaction ID:** [T1]
- **Date / session:** [When.]
- **Award or acquired development:** [Award reason or development ID.]
- **PP received:** [Amount or 0.]
- **PP spent:** [Amount or 0.]
- **Balance after:** [Previous balance + received − spent.]
- **Evidence / record:** [GM confirmation or acquired record link.]

### Keeping the ledger

- Track new Domains, branches, additions, Mastered techniques, and technique improvements. Record each purchase separately, even when several happen in one session.
- Agree on permissions, requirements, and PP price before commitment. Approval and a fictional breakthrough do not themselves spend PP or complete acquisition.
- Add a purchase transaction only after approval, fulfilled requirements, and payment. Link it to the development entry and update the current ability record.
- Keep unresolved prices in the tracker; never enter them as zero-cost purchases. Record actual awards without assuming the core game's award rates apply to this standalone draft.
- Record the two free starting Mastered choices as acquired at 0 PP. Starting Domain allocation remains unresolved; do not assume Domains or branches are free.
- Keep improvements' before/after records. Ordinary improvisation and Minor Effects need no purchase transaction.
