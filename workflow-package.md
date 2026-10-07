# Workflow Package: Routine policyholder correspondence

**Status: Reviewed** (v2 approved by the user, 2026-10-07; v1 was Reviewed 2026-10-06). Revised 2026-10-07 to reflect your report that the workflow has moved from the pilot to two teams, has been introduced to them, and has been tested further with them. Suggestions and unconfirmed responsibilities keep their labels. For the two receiving teams. Sources: Reviewed handoff check, 30/60/90 adoption plan, Design Spec, requirements, test set, Operating Model, value thesis and your answers. **Suggested** and **unconfirmed** items are labelled. Section 6's introduction outline uses the format you chose (a combination of my suggestions) and the barrier you named (workflow fit).

## 1. Purpose and intended users
- **Who it is for:** claims handlers in the two receiving teams: similar teams in a different region and office. The teams aren't named, and that their flow matches the pilot's is an **Assumption**.
- **When to use it:** after a claim decision is approved, for a routine policyholder letter.
- **What it should improve:** letters reach policyholders sooner than the pilot's median of 2.4 business days after approval, while the handler still verifies every detail and approves every letter. The receiving teams' own baseline is **not recorded**.
- **Not for:** conflict, legal or unusual cases; replies to policyholder concerns; end-of-day updates; policy lookup; sending letters automatically without human approval.
- **Current scope (as reported 2026-10-07):** the workflow has moved from the pilot to two teams, which have been introduced to it, with the Chief Claims Officer's approval (date and form not recorded). **No wider use is approved**; expansion beyond two teams is the pending decision.

## 2. Instructions and resources
**Access:** ask the Enterprise Applications Administrator for access and configuration. In the pilot, 14 handlers were denied access; the fix is unconfirmed.

**Steps**
1. Confirm the case is routine (not conflict, legal, big, anomalous or suspected fraud). If not, refer it (section 3).
2. Gather the details from your authorised systems.
3. Copy only the permitted fields into the AI: the policyholder's data, history, claims history and claim notes.
4. Select the predefined template for the use case.
5. The AI formats the information into the template, drafts the letter and flags missing or inconsistent information.
6. Verify every detail against the sources, and check wording, tone and the template's required statements. Resolve each flag from the authorised source. Don't accept the AI's wording where the information is missing.
7. Approve the letter, one at a time, and send it, or refer the case.
8. Report results to the Workflow owner every week.

**Resources that exist:** the predefined templates (pilot); the five test cases as worked examples (section 5).

**Still needed**
- The template set for the receiving teams, and which letter types it covers (Workflow owner).
- Example drafts: the test record holds no draft text (you).
- A setup guide for access and configuration (Enterprise Applications Administrator).
- A one-page list of the permitted fields (Automation Solutions Architect; accepted as R6).
- Training material and a practice session (Claims Learning and Quality Manager, agreed as you report).
- Access for the receiving teams' handlers.

## 3. Checks and boundaries
**Human checks (required)**
- The handler verifies every detail and approves each letter before it is sent. AI flags don't replace the check.
- The AI never approves, sends or decides whether a case is routine, and it has no access to source systems.

**Limits on information:** only the permitted fields. No data from conflict, legal or unusual cases goes into the AI.

**Refer, don't draft:** a case that is very large, anomalous or suspected fraud goes to the specialist review team: medical, vehicle or home. Legal conflict cases go to the legal specialist. **The thresholds for "big" and "anomalous" aren't defined** (Workflow owner). Referral processes vary by region (course), so the receiving teams' routes and specialist teams may differ (**to confirm**).

**If a letter goes out with an error:** the policyholder flags it or it is escalated to the Workflow owner. The error is recorded and a corrected letter is sent (about 2 days, your estimate). **Who is accountable is unresolved.**

**Pause use** (you decide; the Responsible AI and Privacy Working Group for risk concerns) if a letter is sent without handler approval, or non-permitted data is used.

**Escalation:** access problems to you, then the Enterprise Applications Administrator; data handling to you, then the Architect; unclear details to the Workflow owner; policy or privacy concerns to you, then the Working Group; capacity or barriers to the Chief Claims Officer.

## 4. Ownership and support

| Role | Responsibility | Status |
|---|---|---|
| Claims Correspondence Operations Manager | Owns the workflow; approves templates; owns required statements; receives escalated errors; recommends changes | Reviewed role; their own confirmation is as you report |
| You (AI Transformation Program Manager) | Coordinate; approve the roadmap; start bounded tests; Revise, Continue, Pause, Stop within scope | Reviewed |
| Chief Claims Officer | Approves routine use and extra resources | Approved for two teams, as you report |
| Enterprise Applications Administrator | Access and configuration, including after launch | Agreed, as you report |
| Automation Solutions Architect | Data handling; reliability fixes | Agreed, as you report |
| Claims Learning and Quality Manager | Guidance and support | Agreed, as you report |
| Responsible AI and Privacy Working Group | Policy, risk and specialist review | Reviewed role |

- **Who helps users:** the Claims Learning and Quality Manager for guidance; the Workflow owner for unclear cases. **Support channel and response time are not defined** (**Suggested:** the Workflow owner defines them).
- **Who approves changes:** the Workflow owner, and the Chief Claims Officer if capacity or resources are needed (R18).
- **Receiving teams' own workflow owners and local support:** not named (**unconfirmed**).

## 5. Evidence and current status
- **Pilot:** 26 of 40 handlers used the workflow more than once; sampled median drafting time fell from 18 to 11 minutes; reviewed drafts needed fewer wording revisions. Evidence level: **Work Change**.
- **Business impact:** **not measured**. Whether letters go out sooner than 2.4 business days is the next evidence.

| Test | Result |
|---|---|
| Case 1 (routine claim) | Pass |
| Case 2 (approved alternate wording) | Pass |
| Case 3 (uncommon policy condition, referred) | Pass |
| Case 4 (missing and conflicting information) | Fail (invented a claim date), then rerun Pass **as you report** |
| Case 5 (wording implying a final denial) | Fail (confident denial wording), then rerun Pass **as you report** |
| Non-permitted data, access, automatic sending, required statements, escalation and reporting | **Not run** |

- **Known limitations:** no draft text or evidence recorded for the results; the Case 4 and 5 reruns are unevidenced; untested requirements; no pass criteria or targets; compliance review assumed quick.
- **Open actions:** name the receiving teams; set targets and provisional pass criteria; run or waive the untested requirements; decide on the final-decision wording requirement; set the thresholds for "big" and "anomalous"; settle error accountability; agree how approvals are logged; get the Architect's written findings; measure approval-to-send days; set the plan start date.
- **Further testing with the two teams (as reported 2026-10-07):** the cases, results, testers and dates are **not stated**. No pass or fail is recorded, and the Not run tests above stay Not run until results are supplied.
- **Decisions and approvals:** all project documents are Reviewed (2026-10-06). Recommendation recorded: Fix, then your report that the reruns passed. The Chief Claims Officer's approval of routine use and two other teams is as you report; its date and form aren't recorded. **Expansion beyond two teams is not approved.**

## 6. Introduction and ongoing review
**Reported 2026-10-07:** the two teams have been introduced to the workflow. The format actually used, dates and attendance are **not recorded**. The outline below was the suggested plan. Keep it as the reference, and update it with what was actually done.

**Introduction outline** (suggestions, for you to accept or change)
- **Audience and stage:** claims handlers in the two receiving teams, **Not Started (Assumption; you named the barrier but didn't confirm the stage)**.
- **Primary barrier: workflow fit (your expectation, not evidence).** The risk is that the receiving teams' templates, systems or referral routes differ from the pilot's, so the workflow doesn't match how they work.
- **Format:** a combination of a live walkthrough, a one-page guide and a hands-on practice session (your choice, "for now").

| When (from a start date that is **unresolved**) | What happens | Who (**unconfirmed unless marked**) |
|---|---|---|
| **Before the walkthrough** | Compare the receiving team's current flow with the four steps. Note differences in templates, systems and referral routes. Fix or approve the templates and routes the team will use | Workflow owner approves; you coordinate; the receiving team's lead supplies the flow (**not named**) |
| **Days 1 to 30** | **Live walkthrough** of the eight steps, using the team's own letter types with sample or fictional data. **One-page guide** covering the steps, permitted fields, limits and where to refer cases. Access and configuration for each handler | Claims Learning and Quality Manager (agreed, as you report); Enterprise Applications Administrator (access); Architect (permitted-field list) |
| **Days 30 to 60** | **Hands-on practice session** on sample letters, including a missing-information case, a conflicting-information case, an unusual case and a wording-risk case like the test cases. Handlers report where the workflow doesn't fit | Claims Learning and Quality Manager; handlers report to the Workflow owner |
| **Days 60 to 90** | Review fit and results. Adjust templates and routes. Retest anything changed | Workflow owner; you decide within scope |

- **How the team gets help:** the Claims Learning and Quality Manager for guidance; the Workflow owner for unclear cases. **The support channel isn't defined (Suggested above).**
- **How feedback is gathered:** the weekly handler report. **Suggested:** add a standing question to it, "where didn't the workflow fit your letters or process?".
- **Evidence of fit:** none yet. The Not run tests and the weekly reports are the first evidence.

**Evidence to review**

| Level | Measures | Status |
|---|---|---|
| **First Use** (people try it) | Handlers who have used it at least once; access problems raised and closed | **Not recorded** for the receiving teams (introduced as reported; no usage data supplied) |
| **Repeat Use** (people return) | Handlers using it more than once, by week | Pilot: 26 of 40. **Not yet available** for the receiving teams |
| **Work Change** | Median drafting time; wording revisions | Pilot: 18 to 11 minutes (sampled). **Not yet available** for the receiving teams |
| **Business Impact** | Business days from approval to send against 2.4; complaints (correctness); policyholder feedback (frustration); cost | **Not available.** Baselines for the receiving teams, and for cost, complaints and frustration, aren't recorded |

**Quality and safeguards across all four levels:** every sent letter shows handler approval (the Workflow owner checks the weekly reports); wording revisions and errors caught at review are recorded; no permitted-data breaches; conflict and unusual cases referred, not drafted. Usage alone is never counted as business impact.

**Who reviews and the review points**
- **Weekly:** handlers report to the Workflow owner.
- **Monthly:** the Chief Claims Officer reviews speed, cost, correctness and frustration.
- **30, 60 and 90 days:** the adoption plan's checkpoints for the pilot handlers. **The start date for the receiving teams is unresolved.**
- **Decisions:** Revise, Pause, Stop, Continue, Expand. You decide within scope; the Chief Claims Officer decides on resources and further expansion.

**Maintenance, and when to change or retest:** retest the affected cases when a template, the workflow or the permitted data rules change; when a pass criterion changes; when a new failure appears; and for each receiving team's region if its referral rules differ. The Workflow owner approves changes.

## Handoff check status (2026-10-07)
From [handoff-check.md](handoff-check.md) (Reviewed). Only what your report changes:

| Gap | Status after your report |
|---|---|
| 2 Start timing | Moot as a plan: the teams are reported as introduced. The actual order (access, walkthrough, practice) is **not recorded** |
| 3 Approval status | Now stated in section 1 and 5: moved from the pilot to two teams, as reported. Untested requirements still Not run |
| 1 Tool and access route; 5 Receiving-team owner; 6 Support route | **Still open.** Nothing supplied |
| 4, 7 to 12 | **Still open** |
