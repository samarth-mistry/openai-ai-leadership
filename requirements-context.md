# Requirements context: Routine policyholder correspondence

**Status: Reviewed** (approved by the user, 2026-10-06). v1. Sources: Reviewed Design Spec and Operating Model, and your answers of 2026-10-06. No requirements drafted yet.

## Required behaviour
- **AI:** formats permitted source information into the approved letter template, drafts the letter, and flags missing or inconsistent information.
- **Handler:** picks the data and copies it into the AI (your answer, current practice), verifies every detail, checks wording and tone, approves the letter or refers the case.
- **AI never:** reads source systems, approves, sends, or decides whether a case is routine. No automatic sending without human approval.
- **Out of scope:** conflict, legal and unusual cases (large, anomalous, suspected fraud).

## Risks
- **Sensitive information:** policyholder data, history, claims history and claim notes (personal and claims data). Details are not repeated here.
- **What could go wrong (Proposed, none observed):** a wrong or missing detail; wording not from the approved template; a handler copying in more data than permitted; a letter sent without approval; an out-of-scope case drafted instead of referred.
- **Correctability before sending:** easy, because the handler reviews and approves every letter.
- **Correctability after sending:** the policyholder flags the error, or it is escalated to the workflow owner. Correction takes about 2 days (**your estimate; I read "mark 2 days" as the time to correct. Not measured.**). Handlers are held responsible for corrected letters (**you aren't sure**).
- **Data copied into the AI:** handlers choose the data. You say there are no conditions on storage or visibility. Once data is copied in, it can't easily be taken back (**Proposed concern**).

## Decision authority
- **Handler:** approves each letter or refers it.
- **Specialist review teams (medical, vehicle, home):** receive referrals. **Legal specialist:** legal conflict cases.
- **Workflow owner (Claims Correspondence Operations Manager):** approves templates and owns the required statements, which belong to the templates (**Proposed: your belief, not confirmed by them**). Receives escalated errors. Recommends workflow changes.
- **You:** bounded tests, roadmap changes, Revise, Continue, Pause, Stop within scope.
- **Chief Claims Officer:** resources and routine use.
- **Compliance reviewers:** outside this design, assumed to pass letters quickly (Assumption).

## Flags: your reply "yes, confirm" (2026-10-06)
1. **Storage and visibility:** read as yes, the full data policy covers it. The Automation Solutions Architect's confirmation isn't on record, so the risk stays noted until they confirm.
2. **Error ownership:** **still open.** Your reply didn't say whether the handler or the workflow owner is accountable for a wrong letter that was sent.
3. **Correction time:** confirmed. "About 2 days" is the time to send a corrected letter. Still your estimate, not measured.
4. **Required statements:** confirmed by you that the workflow owner owns them (as you report; the manager's own confirmation isn't on record).
