# Priority AI Workflow Design Spec: Routine policyholder correspondence

**Status: Reviewed** (approved by the user, 2026-10-06). v1. Recommendation: Proceed with conditions. Proceed doesn't authorise real use. Sources: Reviewed workflow map and description, improvement and responsibilities, value thesis, operating model, adoption plan and roadmap; the course workflow and boundary tables ([case-context.md](case-context.md)); your answers. Items from your later answers (section "Follow-up answers" in [improvement-responsibilities.md](improvement-responsibilities.md)) are **Proposed** and not reviewed. Your answers of 2026-10-06 on how data reaches the AI and on compliance review are included and are **Proposed**.

## Recommendation: Proceed, with conditions
See the check at the end. In short: the gaps that changed what the requirements must say are now closed, and the two that remain are conditions to meet, not reasons to hold back the requirements step. **Proceed would not authorise real use and doesn't replace testing and approvals.**

## 1. Purpose and better outcome
Routine letters reach policyholders sooner after an approved claim decision, because handlers start from a first draft in the approved template and spend their effort verifying details. The handler still verifies every detail and approves every letter. *(Proposed outcome, Reviewed 2026-10-06.)* **Hypothesis, not evidence:** where the 2.4 business days go is not measured.

## 2. Scope, trigger, inputs, end point
- **Included:** routine letters to policyholders after a claim decision is approved.
- **Excluded:** conflict and legal cases; unusual cases (very large, anomalous or suspected fraud), which are referred; replies to policyholder concerns and end-of-day updates; policy lookup support (Next); sending letters automatically without human approval. Pilot scope only: no expansion.
- **Trigger:** a claim decision is approved.
- **Inputs:** the approved decision, policy and customer details, case notes and required wording. **Sources (your account):** user profile database, past claims, past premiums, claim notes checked against policies, company policies. **How data reaches the AI (your answer, current practice):** the AI doesn't access the sources. The handler copies data into the AI for drafting. **Q18 confirmed (2026-10-06, as you report):** handlers copy the policyholder's data into the AI: policyholder data, history, claims history and claim notes. You say the Automation Solutions Architect and the other owners have confirmed this. I don't have their findings in writing. Conditions beyond the field list aren't stated.
- **End point:** the letter is sent.

## 3. Current workflow (Reviewed map)

| Step | Who | What happens | Friction and judgment |
|---|---|---|---|
| 1. Gather information | Handler | Collects the decision, policy and customer details, notes and required wording from authorised systems | Repeated switching and copying between systems. Finding details across databases is hard. |
| 2. Draft the letter | Handler | Selects (templates are predefined by use case) or recreates wording | Similar wording recreated across cases. Sampled median drafting time before the pilot: 18 minutes. |
| 3. Review the draft | Handler | Checks facts, tone and required statements | Details are hard to trace to sources. Judgment: are the facts, tone and statements right? |
| 4. Approve or refer | Handler | Approves the routine letter, or refers an unusual case to a specialist review team (medical, vehicle, home) | Referral processes vary by region (course). Judgment: is the case routine? Approve or refer? |

- **Handoffs:** handler to specialist team on referral. **Compliance reviewers** check a checklist after the handler drafts the letter. Your instruction: treat them as outside this design, and assume they review and pass letters quickly (**Assumption, untested**). Not in the Reviewed map.
- **Owner:** Claims Correspondence Operations Manager (you report they agree; not heard from them).
- **Elapsed time:** median 2.4 business days approval to send (Reviewed baseline). Not broken down by step.

## 4. Proposed responsibilities

| Step | Level | AI does | Who reviews, approves, handles exceptions |
|---|---|---|---|
| 1. Gather | Person completes | Nothing in First (finding details is Next) | Handler; resolves missing information or refers |
| 2a. Format into approved template | AI completes (course example) | Formats permitted source information into the approved template, if rules permit | Handler reviews at step 3 |
| 2b. Draft | AI supports with human review | Drafts and flags missing or inconsistent information | Handler; Workflow owner for unresolved questions |
| 3. Review | Person completes | Nothing. AI flags are input, not a check | Handler |
| 4. Approve or refer | Person completes | Nothing. AI doesn't approve, send or judge routine status | Handler; specialist teams for referrals; legal specialist for legal cases |
| *Compliance checklist* | *Outside this design (Assumption)* | *Nothing* | *Compliance reviewers; assumed to pass quickly* |

## 5. Affected users
Claims handlers (40 in the pilot); policyholders; compliance reviewers; specialist review teams; team leaders and managers (roles unresolved, Q4).

## 6. Coordination and decision authority
- **Coordinates implementation:** AI Transformation Program Manager (you).
- **Contributors:** Workflow owner (evidence, workflow changes, data-handling review); Enterprise Applications Administrator (access; the fix for the 14 blocked handlers is unconfirmed); Automation Solutions Architect (data handling, integrations); Claims Learning and Quality Manager (guidance; **Proposal**); Responsible AI and Privacy Working Group (policy, risk).
- **Decision authority:**
  - **Handler:** approve each letter or refer.
  - **You:** roadmap, bounded tests, reallocating assigned resources, Revise, Continue, Pause, Stop within scope.
  - **Chief Claims Officer:** additional resources and approval of routine use.
  - **Legal specialist:** legal conflict cases.

## 7. Success and failure signals
- **Success:** approval-to-send days below 2.4 (no target); drafting time stays down (sampled 18 to 11 minutes) with fewer wording revisions; handlers return weekly, including the 14 who were blocked; handlers act on AI flags; every sent letter shows handler approval; complaints and frustration don't rise.
- **Failure:** drafting faster but letters not sooner; more time verifying or tracing; rising errors at review or complaints; a letter sent without handler approval or automatically; AI uses non-permitted data; a conflict or unusual case drafted instead of referred; handlers stop using it; access problems persist.

## 8. Safeguards and constraints
- Handler verifies every detail and approves every letter. AI prepares a first draft only.
- No automatic sending without human approval.
- Conflict, legal and unusual cases stay out. No expansion beyond the pilot. A successful pilot doesn't authorise routine use.
- Only permitted source information (Q18). Use only the approved template.
- Weekly reporting, escalation per the Operating Model, blameless retrospective on a failed test.

## 9. Confirmed information
Four-step current workflow; handler role; 2.4-day median; 18-to-11-minute sampled drafting time; 26 of 40 repeat use; Work Change evidence level; scope exclusions; roles and decision authority in the Operating Model; handler approval of every letter.

## 10. Assumptions, evidence gaps and evidence needed

| Gap | Label | Evidence needed |
|---|---|---|
| Drafting is a meaningful share of the 2.4 days | Assumption; **conflict with** your earlier, now partly withdrawn account | Timestamps for a sample of letters: approval, draft, review, send |
| Which fields handlers may copy into the AI (Q18) | **Confirmed**, as you report. The AI doesn't read sources; the handler pastes data in | Written findings from the Architect and Workflow owner, if you want them on file |
| Compliance review is quick and not a cause of delay | Assumption (your instruction for this case), untested | Timestamps showing any wait for compliance review |
| Who approves templates | **Answered (2026-10-06):** the workflow owner, the Claims Correspondence Operations Manager. You said "can be", so treat as Proposed until they confirm | The manager's confirmation, and which letter types have a template |
| What counts as "big" or "anomalous" | Unresolved | Workflow owner |
| Targets and pass criteria | Unresolved (decided later) | Your and the Chief Claims Officer's decision |
| Access fixed for the 14 | Unconfirmed | Administrator's confirmation |
| Workflow owner's agreement | Reported by you | Their own confirmation |

## 11. Human-owned consequential decision
**The handler's decision to approve and send each letter, or refer the case.** Above that, the Chief Claims Officer decides on routine use and expansion.

## Check against evidence and boundaries

| Check | Result |
|---|---|
| Scope stays within the pilot and your authority | Met |
| Handler approval of every letter preserved; no automatic sending | Met |
| Conflict and legal cases kept out | Met |
| Better outcome supported by evidence | **Partly.** Work Change shown (supplied); business impact and where the time goes unmeasured |
| Data permitted for AI defined | **Met**, as you report (Q18 confirmed) |
| Human review steps complete | **Met for this scope**, with compliance review assumed outside the design and quick |
| Template control defined | **Met, Proposed** (workflow owner approves; their confirmation pending) |
| Pass criteria defined | **Gap** (targets decided later) |
| Access for all pilot handlers | **Unconfirmed** |

**Test status:** no design tests have been run, so all are **Not run**. The pilot figures are supplied course results, preserved as given. I haven't simulated any results. If pass criteria are set or changed after testing, the affected tests must be rerun (**Not run** until then).

## Reasons, and what would change the decision
- **Revise, not Stop:** the evidence supports Work Change, the boundaries hold, and nothing contradicts pursuing the design.
- **Proceed, not Revise (updated 2026-10-06):** the gaps that changed what the requirements must say are closed. The AI doesn't read sources, so step 1 stays with the handler. Compliance review is outside the design and assumed quick. Q18 is confirmed as you report. The template approver is the workflow owner (Proposed).
- **Conditions that must be met, and that Proceed doesn't waive:**
  1. **Pass criteria:** set at least provisional criteria in the requirements step. Targets are still to be decided later. Rerun any affected tests if they change after testing.
  2. **Access:** confirm the fix for the 14 blocked handlers.
  3. **Template approval:** the Claims Correspondence Operations Manager confirms they approve templates.
  4. **Compliance assumption:** check with timestamps that compliance review isn't adding delay.
- **Proceed means moving into requirements and testing.** It doesn't authorise real use, expansion or routine use, and it doesn't replace testing and approvals.
- **Later decision (Continue or Expand):** approval-to-send days against 2.4, with the Chief Claims Officer's approval for routine use.
