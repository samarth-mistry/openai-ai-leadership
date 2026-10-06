# Requirements: Routine policyholder correspondence (First opportunity)

**Status: Reviewed** (approved by the user, 2026-10-06), including the suggested rows, which you accepted. v1. Sources: Reviewed Design Spec, Operating Model, adoption plan and requirements context, and your answers. Each row is labelled **Agreed** (from a Reviewed document or your answers) or **Accepted** (my suggestion, which you accepted on 2026-10-06). No test cases yet.

**Safeguards matched to risk (Proposed):** the data is personal and claims data (high sensitivity). A sent letter can't be unsent, and a correction takes about 2 days (your estimate). Before sending, errors are easy to fix. Data copied into the AI can't easily be taken back. So the rules lean on mandatory human verification before sending, tight limits on what is copied in, and clear escalation.

| ID | Condition | Expected behaviour | Human check | Explicit limit | Label |
|---|---|---|---|---|---|
| **Required actions** | | | | | |
| R1 | A claim decision is approved and the case is routine | The AI formats the information the handler supplies into the approved template for the use case, and drafts the letter | The handler selects the template by use case before drafting | Must not use a template that isn't approved, and must not add details not in the supplied information | Agreed |
| R2 | The supplied information is missing or inconsistent | The AI flags the gap in the draft | The handler resolves it from authorised systems, or refers the case | Must not fill the gap by guessing or inventing | Agreed (flag); Accepted (no guessing) |
| R3 | A draft is produced | The draft is labelled as a draft for handler review | The handler | Must not present AI output as final or ready to send | Accepted |
| **Permitted and prohibited information** | | | | | |
| R4 | A handler copies data into the AI | Only the permitted fields are copied: the policyholder's data, history, claims history and claim notes (Q18 confirmed, as you report) | The handler picks the data. The Automation Solutions Architect and the Workflow owner own the rule | Must not copy any other data. The AI must not read the source systems | Agreed |
| R5 | A case is conflict, legal or unusual | No data from the case is copied into the AI and no AI draft is made | The handler refers it | Must not use the workflow for these cases | Agreed (scope) |
| R6 | Handlers start or continue using the workflow | Handlers get a short list of the permitted fields | Claims Learning and Quality Manager (**Proposal, unconfirmed**) | Must not rely on handlers' memory alone | Accepted |
| R7 | Before any use beyond the pilot | The Architect confirms in writing which fields are permitted and where copied data is stored and who can see it | Automation Solutions Architect; Workflow owner | Must not expand use without it | Accepted |
| **Access and permissions** | | | | | |
| R8 | A pilot handler needs the workflow | Access and configuration are granted to all 40 pilot handlers | Enterprise Applications Administrator approves; you coordinate | Must not grant access outside the pilot without approval. The fix for the 14 blocked handlers is unconfirmed | Agreed (role); fix unconfirmed |
| R9 | The AI is in use | The AI has no access to source systems and no ability to send letters | Enterprise Applications Administrator | Must not be given either | Agreed |
| **Human review** | | | | | |
| R10 | A draft is ready | The handler verifies every detail against the sources, and checks wording, tone and the template's required statements | The handler | AI flags must not replace the check. The letter can't be approved without it | Agreed |
| R11 | The handler has verified the draft | The handler approves the letter before it is sent, one letter at a time | The handler | Must not send automatically or without approval. no batch approval (accepted) | Agreed; Accepted (no batch) |
| R12 | A case is big, anomalous or suspected fraud | The handler refers it to the specialist review team (medical, vehicle or home) | Specialist team. Legal specialist for legal conflict cases | The AI must not decide whether a case is routine. Thresholds for "big" and "anomalous" are not defined | Agreed; thresholds Unresolved |
| R13 | A letter is drafted | It includes the template's required statements | Workflow owner owns the statements and approves templates (**as you report; unconfirmed by them**). The handler checks they are present | The AI must not alter or remove required statements | Agreed (Proposed owner) |
| **Limits on use** | | | | | |
| R14 | Any use of the workflow | Use stays to routine letters after an approved decision, within the current pilot | You (bounded tests). Chief Claims Officer approves routine use and extra resources | Excluded: replies to concerns, end-of-day updates, policy lookup, conflict, legal and unusual cases. A successful pilot doesn't authorise expansion | Agreed |
| R15 | Each week of the pilot | Handlers report use, drafting time, wording revisions and issues to the Workflow owner | Workflow owner | Must not skip reports | Agreed |
| R16 | A letter goes out with an error | The error is recorded with its failure mode, and a corrected letter is sent | The policyholder flags it or it is escalated to the Workflow owner. **Accountability: Unresolved** | Must not be closed without a retrospective if it was a failed test | Agreed (blameless retrospective); Accepted (record each error) |
| R17 | A letter is sent without handler approval, or non-permitted data was used | Use is paused until the condition is resolved | You decide. Responsible AI and Privacy Working Group for risk concerns | Must not resume without your decision | Agreed (Pause criteria, adoption plan) |
| R18 | A template or the workflow changes | The change is reviewed before use | Workflow owner; Chief Claims Officer if capacity or resources are needed | Must not change templates informally | Accepted |

## Missing information and authority to confirm
- **Workflow owner (Claims Correspondence Operations Manager):** confirm they approve templates and own the required statements (R13); confirm the thresholds for "big" and "anomalous" (R12).
- **Automation Solutions Architect:** the permitted fields and the storage and visibility of copied data in writing (R4, R7). You say storage and visibility are covered by the full data policy; their confirmation isn't on record.
- **Enterprise Applications Administrator:** confirm access for the 14 blocked handlers (R8).
- **Error accountability (R16):** the handler or the workflow owner. Unresolved.
- **Not recorded:** how approvals are logged, and whether the drafts are kept.
- **Compliance review:** outside this design and assumed quick. No requirement written.

---

## Introduction recommendation (2026-10-06): Reviewed (approved by the user, 2026-10-06)
The Reviewed requirements above are unchanged. This section was added after the test set ([test-set.md](test-set.md), then Draft v1, now Reviewed).

### Recommendation: **Fix**
Address the gaps and retest before any introduction. **Introduce** is not supported yet. **Stop** is not supported either.

### Check against the three conditions for Introduce
| Condition | Result |
|---|---|
| All required tests pass | **No.** Case 4 failed (invented a claim date when sources disagreed) and Case 5 failed (confident denial wording). Reruns of both are **Not run**. The five cases don't test non-permitted data (R4), access (R6 to R9), automatic sending (part of R11), removal of required statements (R13) or escalation and reporting (R15 to R18). Those are **Not run**. |
| Supporting evidence available | **Partly.** Work Change is supported (supplied pilot figures: drafting time 18 to 11 minutes, 26 of 40 repeat use). Business impact isn't measured (approval-to-send days against 2.4). The test results are supplied without draft text or detail. The Architect's written findings aren't on record. |
| Required approvals confirmed | **No.** See the list below. |

### Why Fix, not Stop
- Cases 1 to 3 passed, including a correct referral of an unusual case.
- The failures are specific: filling a gap, and confident wording on a disputed claim. Neither shows the approach can't work.
- The safeguards hold: handler verification of every letter, no automatic sending, and conflict and legal cases kept out.
- No constraint on record rules the approach out.

### Why not Introduce
Two required tests failed, the required retests and several tests are Not run, and the approvals below aren't confirmed. Missing evidence isn't counted as a pass.

### Open actions
| # | Action | Owner | Status |
|---|---|---|---|
| 1 | Fix the workflow for Case 4 (no invented values) and Case 5 (no final-denial wording). What the fix is, and who makes it, isn't stated | **Unresolved** (you coordinate) | Open |
| 2 | Decide whether to add the suggested requirement: the AI must not state or imply a final decision on a disputed claim, and must flag it | You | Open |
| 3 | Rerun Cases 4 and 5. Decide whether Cases 1 to 3 need a rerun | You, with the Workflow owner | **Not run** |
| 4 | Add and run tests for the untested requirements, or record why they aren't needed before introduction | You | Open |
| 5 | Set at least provisional pass criteria. If they change after testing, rerun the affected tests | You and the Chief Claims Officer | Open |
| 6 | Measure approval-to-send days against the 2.4-day baseline | Workflow owner | Open |
| 7 | Confirm templates and required statements, and the thresholds for "big" and "anomalous" | Workflow owner | Unconfirmed |
| 8 | Written findings on permitted fields, and storage and visibility | Automation Solutions Architect | Unconfirmed |
| 9 | Confirm the access fix for the 14 blocked handlers | Enterprise Applications Administrator | Unconfirmed |
| 10 | Decide who is accountable for a sent error | You, with the Workflow owner | Unresolved |
| 11 | Review and approve the test set | You | **Done: Reviewed 2026-10-06** |
| 12 | Approval of routine use | Chief Claims Officer | **Not yet requested** |
| 13 | **Suggested:** tell pilot handlers about both failure modes so they check for invented dates and denial wording until the fix is retested | You | Not started |

### Decision owner (from the Reviewed Operating Model)
- **Fix:** you, within your authority.
- **Introduce (routine use):** the Chief Claims Officer, on your recommendation. They haven't been asked.
- **Stop:** you, within the pilot scope.
- **Until then:** the pilot continues within its current scope. This recommendation doesn't authorise routine use or expansion.

---

## Update (2026-10-06): your report on reruns, confirmations and the introduction decision: Reviewed (approved by the user, 2026-10-06; as you report where marked)
The Reviewed text above is unchanged.

**Reported by you**
- Cases 4 and 5 were rerun after the fix and passed (details in [test-set.md](test-set.md); no evidence recorded). Actions 1 and 3 are done, as you report.
- You have confirmed with "a number of owners and other participants, the architect, and all". You didn't name them. I've read this as covering actions 7 and 8 (Workflow owner's confirmations; the Architect's findings, still not in writing). It doesn't clearly cover action 9 (access for the 14), action 10 (error accountability) or action 12 (Chief Claims Officer approval).
- You say the decision on the final working requirements is yours, they are ready for shipping, and you want to introduce them to other teams too. I've recorded this as your **stated decision**, not as an approval.

**Check against the Reviewed documents (conflicts flagged, not resolved)**
1. **Who approves introduction.** The Reviewed Operating Model says the Chief Claims Officer approves routine use, and anything beyond the pilot scope triggers a review. You approve the roadmap and bounded tests. No Chief Claims Officer approval is on record.
2. **Other teams is an Expand decision.** The Reviewed adoption plan says Expand needs business impact shown against the 2.4-day baseline, the Chief Claims Officer's approval, confirmed support and maintenance owners, and extra resources if needed. None of these is on record, and support and maintenance is not yet done in the brief.
3. **Tests.** Cases 1 to 5 now pass, as reported. The untested requirements are still **Not run**. Introduction requires all required tests to pass, so either run them or record that they aren't required.
4. **Suggested requirement.** The final-decision wording requirement, proposed after Case 5, is not recorded as approved. Tell me if "ready for shipping" includes adding it.

**Updated recommendation:** the Cases 4 and 5 gap is closed, as reported. **Introduce** for routine use by the current pilot teams is the next decision, but not yet supported, because the Chief Claims Officer's approval isn't on record and the untested requirements are Not run. **Expand to other teams is not yet supported.**

### Further update (2026-10-06): Reviewed (approved by the user, 2026-10-06; as you report where marked)
You say the Chief Claims Officer has approved routine use and the introduction to two other teams (similar teams in a different region and office). Action 12 is done, as reported. The approval covers two teams only. Support and maintenance owners are reported as agreed (action unchanged for the three confirmations, which I haven't received from them). Business impact is still unmeasured, and the untested requirements are still **Not run**.
