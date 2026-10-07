# AI Strategy Brief: Northfield Mutual routine policyholder correspondence

**Status: Reviewed** (approved by the user, 2026-10-07), including the update below. v1. Northfield Mutual is a fictional insurer (about 2,000 employees). Sources: the eight Reviewed artifacts listed in section 4, the Reviewed [material-gaps-audit.md](material-gaps-audit.md), and the stakeholder and ask you confirmed on 2026-10-07. Nothing here is new evidence. Labels: **Reviewed** = from a Reviewed artifact; **As reported** = your word, no evidence or document on record; **Proposed**, **Assumption**, **Unresolved**.

## Update (2026-10-07, as you report)
- The workflow has **moved from the pilot** and is being given to **two teams**. I've read "the other team, not the pilot" as the two receiving teams. They **have been introduced** to it.
- It has been **tested further with the two teams**. The cases, results and dates **aren't stated**, so no pass or fail is recorded and the Not run tests stay Not run until you supply results.
- No usage, drafting-time or approval-to-send data from the two teams is on record. The evidence level is unchanged: **Work Change** from the pilot; no Business Impact evidence.
- The Reviewed Operating Model and Value Thesis say to continue within the pilot scope. This move was approved by the Chief Claims Officer as reported. It is not recorded in the roadmap, the 30/60/90 plan or the Operating Model (audit gaps 3 and 4).
- Names of the two teams, the introduction format actually used, and dates are **not recorded**.

**Stakeholder and decision owner:** Chief Claims Officer. **The ask:** a decision to expand beyond the two other teams. How many more teams, which ones, and by when are **unknown**.

## 1. Leadership recommendation

**What should happen next (Proposed; your decision, audit gap 1):** continue within the scope already approved, measure whether letters go out sooner, and ask the Chief Claims Officer to agree the conditions under which expansion beyond two teams would be approved, rather than to approve expansion now. The Reviewed Value Thesis already says the next step is to continue within the current scope and measure the outcome. I proposed this framing because the evidence doesn't yet support expansion. Tell me if you want the ask framed differently.

**Business result and why now:** routine letters reach policyholders sooner after an approved claim decision (median today: **2.4 business days**), with the handler still verifying every detail and approving every letter. Why now: this is the current business priority in the Reviewed Charter and roadmap, the pilot is running, and the Chief Claims Officer has approved routine use and two other teams, **as reported**. I have no recorded deadline or cost of delay.

**Evidence and confidence**

| Level | What the evidence shows | Confidence (Proposed) |
|---|---|---|
| First Use | 14 of 40 pilot handlers hadn't used it; they were denied access (as reported; fix unconfirmed). None yet for the receiving teams | Not available for the receiving teams |
| Repeat Use | 26 of 40 handlers used it more than once (course) | Moderate for the pilot |
| **Work Change** (current level) | Sampled median drafting time fell from 18 to 11 minutes; reviewed drafts needed fewer wording revisions, number not stated (course) | Moderate: sampled, not independently checked |
| Business Impact | **None.** Approval-to-send days against 2.4 are unmeasured, and where the 2.4 days go is unmeasured. No baselines for cost, complaints or frustration | **Low: no evidence** |

The pilot shows that drafting got faster. It doesn't show that letters reach policyholders sooner.

**Conditions and boundaries (Reviewed unless marked)**
- A handler verifies every detail and approves every letter before it is sent. No automatic sending.
- Conflict, legal and unusual cases stay out. So do replies to policyholder concerns, end-of-day updates and policy lookup.
- Handlers copy only the permitted data in (confirmed as reported; written findings not on record). The AI never reads source systems.
- A successful pilot, and a reviewed handoff package, do not authorise introduction or expansion. Expand needs business impact shown against the baseline, the Chief Claims Officer's approval, confirmed support owners, and extra resources if needed.

**Material open questions**
1. How the ask is framed, and what criteria would justify expansion (no targets or pass criteria exist).
2. Whether the untested requirements are run or waived, and the evidence for the reruns.
3. The Chief Claims Officer's approval: date, form, and their agreement to the Charter's sponsor commitments.
4. Where First sits in the roadmap and plan now that two receiving teams are in play, and the plan start date.
5. Ownership, capacity and support for the receiving teams; five blocking gaps in the handoff check.
6. Regional fit: flow, templates, referral routes and data rules assumed to match.
7. Error accountability, the "big" and "anomalous" thresholds, and the Architect's written findings.

**Decision, support or resource requested:** the decision named above, from the Chief Claims Officer. **No additional resources are stated** in any Reviewed artifact. Support from the Enterprise Applications Administrator, Automation Solutions Architect and Claims Learning and Quality Manager is **as reported** and unconfirmed by them.

## 2. Six-month roadmap (Reviewed 2026-10-03; unchanged)
**Timing within the six months is Unresolved for all three stages.** No dates are given. Owners for Next and Later are Unresolved. No impact-versus-effort comparison is on record; the order of Next and Later comes from the course example and your choice.

| Stage | Opportunity | Why placed here | Dependencies | Reconsideration trigger |
|---|---|---|---|---|
| **First: develop now** | Routine policyholder correspondence | Current business priority (Charter). Baseline 2.4 days; pilot Work Change | Data-handling findings (confirmed as reported); access for all handlers; business-impact measurement | Failed test needing a decision outside your scope; business-day results in; any proposal beyond the current scope (Operating Model) |
| **Next: possible follow-on** | Policy lookup support | Handlers check details across several systems. You report that finding details is where handlers still struggle. No time figures recorded | Trusted sources, access to the systems handlers check, agreed review requirements; which systems (Q2) is open | Its dependencies and evidence are confirmed |
| **Later: future option** | Complex claim recommendations | Conflicts and legal cases need the legal specialist. No data on how often they occur or cost | A specialist owner agrees to take part; approved controls for a bounded test | Stronger evidence of frequency and cost, a specialist owner agreeing, and controls approved |

**Conflict, not resolved:** the roadmap's First stage is a bounded pilot, but you report the workflow has moved from the pilot to two teams. The roadmap hasn't been updated (audit gap 4).

## 3. First opportunity: routine policyholder correspondence

**Opportunity statement (Reviewed):** in routine policyholder correspondence, reduce repetitive drafting and rework so policyholders receive correct updates faster and with less frustration, while retaining claims handler verification of details and approval before each letter is sent.

**Workflow change**
- **Today (Reviewed map):** the handler gathers details from authorised systems, selects or recreates wording, reviews the draft, and approves the letter or refers an unusual case.
- **Proposed change:** the handler copies permitted data into the AI. The AI formats it into the approved template, drafts the letter, and flags missing or inconsistent information. The handler verifies, approves or refers.

**AI and human responsibilities (Reviewed)**

| Step | Level | Who |
|---|---|---|
| Gather information | Person completes | Handler |
| Format into approved template | AI completes | Handler reviews at the next step |
| Draft and flag gaps | AI supports with human review | Handler; Workflow owner for unresolved questions |
| Review the draft | Person completes | Handler |
| Approve or refer | Person completes | Handler; specialist review teams (medical, vehicle, home); legal specialist for legal cases |

**30/60/90 adoption plan (Reviewed; for the pilot handlers; start date Unresolved)**
- **30 days:** confirm the cause of the access denials and restore access for the 14; keep weekly reporting; start recording approval-to-send days; get the data-handling findings.
- **60 days:** review repeat use, drafting time, revisions and the first approval-to-send data; reinforce what works; adjust support.
- **90 days:** review sustained use and the full comparison with 2.4 days; take it to the Chief Claims Officer's monthly review; decide Continue, Revise, Pause, Stop or propose Expand.
- **Receiving teams:** the Package gives a Suggested days 1 to 90 introduction (walkthrough, one-page guide, practice session). Stage (Not Started) and barrier (workflow fit) are Assumptions.

**Requirements and test evidence (Reviewed; 18 requirements, R1 to R18)**

| Test | Result |
|---|---|
| Case 1 routine claim | Pass |
| Case 2 approved alternate wording | Pass |
| Case 3 uncommon policy condition, referred | Pass |
| Case 4 missing and conflicting information | **Fail** (invented a claim date); rerun **Pass, as reported** |
| Case 5 wording implying a final denial | **Fail** (confident denial wording); rerun **Pass, as reported** |
| Non-permitted data, access, automatic sending, required statements, escalation and reporting | **Not run** |

No draft text or evidence is recorded for these results. Pass criteria and targets don't exist. The final-decision wording requirement (proposed after Case 5) isn't recorded as approved.

**Ownership**
- **Workflow owner:** Claims Correspondence Operations Manager (owns the workflow; approves templates and required statements, as you report).
- **Coordinator:** you, the AI Transformation Program Manager.
- **Executive sponsor:** Chief Claims Officer.
- **Data handling:** Automation Solutions Architect.
- Receiving teams' own owners: not named.

**Safeguards:** as in section 1. Pause use (you decide) if a letter is sent without handler approval, or non-permitted data is used. Errors are recorded and a corrected letter sent (about 2 days, your estimate); who is accountable is **Unresolved**.

**Support and maintenance**
- **Roles (Proposed in the Operating Model; "agreed, as you report" in the Package):** Enterprise Applications Administrator for access and configuration; Automation Solutions Architect for reliability fixes; Claims Learning and Quality Manager for guidance and support; Workflow owner approves template and workflow changes.
- **Not defined:** support channel, response time, local owners for the receiving teams.
- **Retest** when a template, the workflow or the permitted-data rules change, when a pass criterion changes, when a new failure appears, and per region if referral rules differ.

**Latest decision and approval status**
- **Recorded recommendation (Reviewed):** Fix. The conditions for Introduce are not shown as met: required tests are Not run and approvals are as reported.
- **As reported:** the Case 4 and 5 reruns passed; the Chief Claims Officer approved routine use and two other teams; the owners confirmed; the workflow has been introduced to the two teams and tested further with them (results not stated).
- **Not approved:** expansion beyond two teams.
- **Conflict, not resolved:** the Package says two teams are approved while the Reviewed recommendation says Introduce isn't yet supported (audit gap 2). The Package was revised and Reviewed on 2026-10-07 (v2), but five blocking gaps from the Reviewed handoff check remain open (audit gap 5).

## 4. Supporting decisions

| # | Component | Current version | Status |
|---|---|---|---|
| 1 | AI Leadership Charter | [leadership-charter.md](leadership-charter.md) | Reviewed 2026-10-03. Still says the Chief Claims Officer's agreement to the sponsor commitments is unconfirmed |
| 2 | AI Strategy and Roadmap | [roadmap.md](roadmap.md) | Reviewed 2026-10-03 |
| 3 | Value Thesis and Evidence Plan | [value-thesis.md](value-thesis.md) | Reviewed 2026-10-04 |
| 4 | Responsible AI Operating Model | [operating-model.md](operating-model.md) | Reviewed 2026-10-04, with a 2026-10-06 update |
| 5 | 30/60/90 AI Adoption Plan | [adoption-plan.md](adoption-plan.md) | Reviewed 2026-10-05 |
| 6 | Priority AI Workflow Design Spec | [design-spec.md](design-spec.md) | Reviewed 2026-10-06 (Proceed with conditions) |
| 7 | AI Workflow Requirements and Test Case Set | [requirements.md](requirements.md), [test-set.md](test-set.md) | Reviewed 2026-10-06 |
| 8 | AI Workflow Package | [workflow-package.md](workflow-package.md) | Reviewed 2026-10-07 (v2; v1 was Reviewed 2026-10-06); handoff check in [handoff-check.md](handoff-check.md) |

Also: [material-gaps-audit.md](material-gaps-audit.md) (Reviewed 2026-10-07), [README.md](README.md) (full file map). The detailed source artifacts are unchanged.
