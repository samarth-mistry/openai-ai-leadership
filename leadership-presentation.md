# Leadership roadmap presentation: routine policyholder correspondence

**Status: Draft v1 for your review, not Reviewed.** Built only from the Reviewed [ai-strategy-brief.md](ai-strategy-brief.md) (Reviewed 2026-10-07) and the artifacts it cites. **Audience and decision owner:** Chief Claims Officer (confirmed 2026-10-07). **Decision:** whether to expand beyond the two other teams, framed in the Brief as agreeing the conditions for expansion rather than approving it now. No timing, ROI, approval or ownership has been added. Items marked **as reported** rest on your word with no document or evidence on record.

**Emphasis for this audience:** the Chief Claims Officer decides resources, capacity and routine use, so the deck leads with the result and the decision, keeps the evidence honest about what is not yet shown, and ends with one clear ask.

---

## Slide 1: Faster routine letters, with handlers still in control
**Content**
- **Priority:** routine policyholder correspondence in claims operations.
- **Intended outcome:** routine letters reach policyholders sooner after an approved claim decision. Median today: **2.4 business days**.
- **Condition that does not change:** a claims handler verifies every detail and approves every letter before it is sent.
- **Why now:**
  - It is the current business priority.
  - The workflow has moved from the pilot to two teams, with your approval (**as reported**).
  - No deadline or cost of delay is on record.

**Speaker notes:** Open with the result we want and the control we keep. Be clear that the 2.4 days is today's measured median and that the goal is to reduce it. Don't claim urgency beyond the priority and the current rollout.

**Sources:** [ai-strategy-brief.md](ai-strategy-brief.md) section 1; [roadmap.md](roadmap.md); [success-baseline.md](success-baseline.md); [leadership-charter.md](leadership-charter.md).

---

## Slide 2: Six-month roadmap: First, Next, Later
**Content**

| Stage | Opportunity | Why here | Dependencies | Reconsider when |
|---|---|---|---|---|
| **First** (develop now) | Routine policyholder correspondence | Current priority; baseline 2.4 days; pilot shows Work Change | Data-handling findings; access for all handlers; business-impact measurement | A failed test needs a decision outside scope; business-day results are in; use beyond current scope is proposed |
| **Next** (possible follow-on) | Policy lookup support | Handlers check details across several systems; finding details is where they still struggle (**as reported**) | Trusted sources; access to the systems; agreed review requirements; which systems (open) | Dependencies and evidence are confirmed |
| **Later** (future option) | Complex claim recommendations | Conflicts and legal cases need the legal specialist; no frequency or cost data | A specialist owner agrees; approved controls for a bounded test | Stronger evidence; specialist owner agrees; controls approved |

- **Timing within the six months is unresolved** for all three stages. Owners for Next and Later are unresolved.

**Speaker notes:** The order is a reasoned proposal, not a ranking from data: it comes from the course example and your choice. Say plainly that dates and Next and Later owners aren't set. Flag that the roadmap still describes First as a bounded pilot and hasn't been updated for the move to two teams.

**Sources:** [roadmap.md](roadmap.md); [ai-strategy-brief.md](ai-strategy-brief.md) section 2; [material-gaps-audit.md](material-gaps-audit.md) gap 4.

---

## Slide 3: First opportunity: what changes, and who does what
**Content**
- **Today:** the handler gathers details from authorised systems, selects or recreates wording, reviews the draft, and approves the letter or refers an unusual case.
- **Change:** the handler copies the permitted data into the AI. The AI formats it into the approved template, drafts the letter, and flags missing or inconsistent information.

| Step | Level | Who |
|---|---|---|
| Gather information | Person completes | Handler |
| Format into approved template | AI completes | Handler reviews at the next step |
| Draft and flag gaps | AI supports with human review | Handler |
| Review the draft | Person completes | Handler |
| Approve or refer | Person completes | Handler; specialist review teams; legal specialist for legal cases |

- **The AI never** reads source systems, approves, sends, or decides whether a case is routine. **Out of scope:** conflict, legal and unusual cases; replies to concerns; end-of-day updates; policy lookup; automatic sending.

**Speaker notes:** The AI does the formatting and first draft. People do everything that needs judgement. Emphasise that the handler's approval is required on every letter.

**Sources:** [workflow-map.md](workflow-map.md); [improvement-responsibilities.md](improvement-responsibilities.md); [design-spec.md](design-spec.md); [requirements.md](requirements.md).

---

## Slide 4: What the evidence shows, and what it doesn't
**Content**
- **Baseline:** median 2.4 business days from approval to send.
- **Evidence level: Work Change.** In the pilot, 26 of 40 handlers used the workflow more than once, sampled median drafting time fell from 18 to 11 minutes, and drafts needed fewer wording revisions (how many fewer isn't stated).
- **Business impact: no evidence yet.** Whether letters go out sooner than 2.4 days is unmeasured, and so is where those days go.
- **Confidence (Proposed):** moderate for Work Change (sampled); low for Business Impact.

| Test | Result |
|---|---|
| Cases 1 to 3 (routine, approved alternate wording, referred unusual case) | Pass |
| Case 4 (missing and conflicting information) | Fail (invented a claim date); rerun Pass **as reported** |
| Case 5 (wording implying a final denial) | Fail (confident denial wording); rerun Pass **as reported** |
| Non-permitted data, access, automatic sending, required statements, escalation, reporting | **Not run** |

- **Latest decision and status:**
  - Recorded recommendation: **Fix**. The conditions for Introduce aren't shown as met.
  - Reported since: moved from the pilot to two teams; introduced; tested further (results not stated).
  - **Not approved:** expansion beyond two teams.
- **Limitations:** no draft text or evidence recorded for the reruns; no results from the two teams; no targets or pass criteria; the Package and the Reviewed recommendation conflict on approval status.

**Speaker notes:** Lead with what's solid and what isn't. The pilot shows drafting got faster. It doesn't show letters go out sooner. Name the failed tests and the Not run tests. Don't present the reruns as proven.

**Sources:** [value-thesis.md](value-thesis.md); [success-baseline.md](success-baseline.md); [evidence-judgment.md](evidence-judgment.md); [test-set.md](test-set.md); [requirements.md](requirements.md) (recommendation section); [ai-strategy-brief.md](ai-strategy-brief.md) update.

---

## Slide 5: How adoption, ownership and review work
**Content**
- **30/60/90 (pilot handlers; start date unresolved):**
  - 30: restore access for the 14 blocked handlers, keep weekly reporting, start recording approval-to-send days, get data-handling findings.
  - 60: review repeat use, drafting time, revisions and first approval-to-send data; adjust support.
  - 90: review sustained use and the comparison with 2.4 days; decide Continue, Revise, Pause, Stop, or propose Expand.
- **Owners:** Claims Correspondence Operations Manager (workflow owner); you as AI Transformation Program Manager (coordinate); Chief Claims Officer (resources and routine use); Automation Solutions Architect (data handling); Enterprise Applications Administrator and Claims Learning and Quality Manager (access, guidance). Support roles **as reported**.
- **Safeguards:** handler verifies and approves every letter; permitted data only; pause use if a letter is sent without approval or non-permitted data is used.
- **Support:** no channel or response time defined. Receiving teams' own owners not named.
- **Review points:** weekly handler reports to the workflow owner; monthly review by the Chief Claims Officer of speed, cost, correctness and frustration.

**Speaker notes:** The 30/60/90 plan was written for the pilot handlers. The two teams have been introduced (as reported), but no dates or plan for them are recorded. Say what is agreed and what's unconfirmed.

**Sources:** [adoption-plan.md](adoption-plan.md); [operating-model.md](operating-model.md); [workflow-package.md](workflow-package.md); [leadership-charter.md](leadership-charter.md).

---

## Slide 6: Open items, what we're asking for, and what happens next
**Content**
- **Material open items:**
  1. How the ask is framed, and what would justify expansion (no targets or pass criteria).
  2. Untested requirements: run or waive; rerun evidence.
  3. Your approval: date, form, and your agreement to the sponsor commitments.
  4. First's place in the roadmap and plan, and the start date.
  5. Ownership, capacity and support for the receiving teams; five blocking handoff gaps.
  6. Regional fit: flow, templates, referral routes and data rules assumed to match.
  7. Error accountability, "big" and "anomalous" thresholds, the Architect's written findings.
- **Requested:** a decision from you (next slide). **Resources:** none stated in any reviewed artifact. **Support:** the three support roles need to confirm their roles.
- **Next actions if you agree (Proposed, from the audit):** record your approval; set provisional criteria; measure approval-to-send days against 2.4; update the roadmap and the 30/60/90 plan for the two teams; settle ownership and support for them.

**Speaker notes:** Don't hide the open items. Show that each has an owner or a proposed way to close it. State that no extra resources are requested because none are recorded, not because none are needed.

**Sources:** [material-gaps-audit.md](material-gaps-audit.md); [ai-strategy-brief.md](ai-strategy-brief.md) section 1; [handoff-check.md](handoff-check.md).

---

## Slide 7: Decision requested
**Content**
- **Decision owner:** Chief Claims Officer.
- **The question:** expand beyond the two other teams?
- **Proposed framing (Brief):** don't approve expansion now. Agree the conditions under which it would be approved.
- **Conditions already on record for Expand:**
  - Business impact shown against the 2.4-day baseline.
  - Your approval.
  - Support and maintenance owners confirmed.
  - Extra resources agreed, if needed.
- **To close first (Proposed):** provisional criteria; untested requirements run or waived; rerun and two-team test evidence.
- **Not known:** how many more teams, which ones, and by when.

**Speaker notes:** Make one ask and ask for a yes or no on the conditions. If the answer is to expand now, record that as your decision against the evidence shown, and flag the open items.

**Sources:** [ai-strategy-brief.md](ai-strategy-brief.md) sections 1 and 3; [adoption-plan.md](adoption-plan.md) (decision definitions); [value-thesis.md](value-thesis.md).

---

## Notes for you
- **Not strengthened:** no ROI, cost, deadline, or approval date appears. "As reported" items are labelled on the slides.
- **Conflicts shown, not resolved:** roadmap versus the move to two teams; the Reviewed Fix recommendation versus the Package's approval status.
- **If you have the results of the two-team testing**, slide 4 can be updated and the evidence claim revisited.
