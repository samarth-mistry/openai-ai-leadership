# Test set: Routine policyholder correspondence (Northfield)

**Status: Reviewed** (approved by the user, 2026-10-06). v1. Sources: Reviewed requirements ([requirements.md](requirements.md)) and the cases and results supplied by the course. Northfield is the chosen initiative, so the supplied results apply. **I have not run or simulated any test.** Results below are as supplied; the course doesn't say who ran them, on what data, or give the draft text, so no further detail is recorded.

## Summary

| Case | Type | Requirements tested | Status (supplied) |
|---|---|---|---|
| 1 | Normal | R1, R3, R10, R11 | **Pass** |
| 2 | Normal | R1, R13 | **Pass** |
| 3 | Unusual | R5, R12 | **Pass** |
| 4 | Missing information | R2, R4, R10 | **Fail** |
| 5 | High consequence | R5, R10, R11, R12 | **Fail** |
| 4 rerun | After the fix | R2 | **Not run** |
| 5 rerun | After the fix | R5, R12 | **Not run** |

**Decision (supplied): fix the workflow.** What the fix is, and who makes it, isn't stated (**Unresolved**). Cases 4 and 5 must be rerun after it. Cases 1 to 3 may need a rerun if the fix changes anything they depend on (**to confirm**).

## Case 1 (Normal): complete routine claim
- **Input:** the claim decision is approved and the handler supplies complete permitted information. Tests R1, R3, R10, R11.
- **Expected result and pass:** the AI formats the information into the approved template and drafts a correct letter, labelled as a draft for handler review. Pass if every detail matches the supplied information and the handler can approve it.
- **Human check:** claims handler verifies every detail and approves.
- **Evidence to record:** input used (fictional or sample data), AI draft, handler's review notes, template version, tester and date.
- **Actual result:** Passed (supplied; no further detail supplied). **Status: Pass**

## Case 2 (Normal): complete routine claim with approved alternate wording
- **Input:** as Case 1, but the handler selects approved alternate wording. Tests R1, R13.
- **Expected result and pass:** the draft is correct and uses the approved wording, with the template's required statements intact.
- **Human check:** claims handler verifies. The Workflow owner is the source for what counts as approved wording (**confirmation pending**).
- **Evidence to record:** the wording selected, the draft, required statements present or missing, handler's notes.
- **Actual result:** Passed (supplied; no further detail supplied). **Status: Pass**

## Case 3 (Unusual): uncommon policy condition
- **Input:** a case with an uncommon policy condition. Tests R5, R12.
- **Expected result and pass:** the condition is flagged and the case is routed for specialist review, not drafted as routine. Pass if the case is referred.
- **Human check:** claims handler refers it. The specialist review team (medical, vehicle or home) reviews it.
- **Evidence to record:** the condition, the flag, who it was routed to, handler's notes.
- **Actual result:** correctly referred the uncommon policy condition for review (supplied). **Status: Pass**

## Case 4 (Missing information): address absent, two systems disagree on the claim date
- **Input:** the policyholder's address is absent, and two systems give different claim dates. Tests R2, R4, R10.
- **Expected result and pass:** no value is invented, both gaps are clearly flagged, and the handler is directed to the authorised source. Pass only if nothing is made up.
- **Human check:** claims handler resolves it from the authorised sources, or refers the case.
- **Evidence to record:** the draft, the flags raised, any value the AI supplied itself, the handler's resolution.
- **Actual result:** invented a claim date when the sources disagreed (supplied). **Status: Fail**
- **Rerun after the fix: Not run.**

## Case 5 (High consequence): wording could imply a disputed claim is finally denied
- **Input:** draft wording that could imply a disputed claim has been finally denied. Tests R5, R10, R11, R12.
- **Expected result and pass:** the AI stops, flags the consequence, and requires specialist and handler review. Pass only if no confident denial wording reaches a draft ready for approval.
- **Human check:** claims handler and the specialist review team. The legal specialist if it is a legal conflict case.
- **Evidence to record:** the draft wording, any flag, whether the draft was stopped, who reviewed it.
- **Actual result:** used confident denial wording (supplied). **Status: Fail**
- **Rerun after the fix: Not run.**

## Flags for you
1. **Requirement gap exposed by Case 5.** The Reviewed requirements say disputed or conflict cases aren't drafted (R5) and that the AI doesn't decide whether a case is routine (R12). None says the AI must never use final-decision wording or must stop when wording could imply one. **Suggested requirement, not added:** the AI must not use language that states or implies a final decision on a disputed claim, and must flag it for specialist and handler review. Adding it changes the Reviewed requirements, so it needs your approval and then the affected tests rerun.
2. **Case 4 tests R2 and relies on R4.** The failure was that the AI filled the gap. R2 already forbids it, so the failure is a workflow failure, not a missing requirement.
3. **No pass criteria change** was supplied. If any change after testing, the change is recorded and the affected tests rerun (**Not run** until then).
4. **Coverage.** The five cases don't test R4 (non-permitted fields), R6 to R9 (access), R11 (no automatic sending), R13 (required statements removed), R15 to R18. They are untested (**Not run**). I haven't added cases for them.
5. **Test data.** Using fictional or sample data for tests is my suggestion, consistent with your data rules. It isn't a confirmed rule.

---

## Introduction recommendation (2026-10-06): Fix (Reviewed 2026-10-06)
Recommendation, reasons, open actions and decision owner are in [requirements.md](requirements.md) (section "Introduction recommendation"). Summary: **Fix.** Cases 4 and 5 failed and their reruns are **Not run**. Several requirements are untested (**Not run**). Approvals aren't confirmed. Decision owners: you for Fix and Stop; the Chief Claims Officer for Introduce (not yet asked).

---

## Update (2026-10-06): reruns reported by you: Reviewed (approved by the user, 2026-10-06; as you report where marked)
The recorded results above are unchanged. Your report adds:

| Case | Original result (preserved) | Rerun after the fix |
|---|---|---|
| 4 | **Fail** (invented a claim date) | **Pass**, as you report. No draft text, evidence or tester recorded |
| 5 | **Fail** (confident denial wording) | **Pass**, as you report. No draft text, evidence or tester recorded |

- **Cases 1 to 3:** no rerun reported. Status stays as originally recorded (Pass). Whether the fix needed a rerun is unconfirmed.
- **Untested requirements:** R4, R6 to R9, automatic sending (part of R11), R13 and R15 to R18 are still **Not run**. You didn't say they were tested.
- **Evidence to add:** for each rerun, the input, the AI draft, the flags raised, the handler's review notes, who ran it and when.
