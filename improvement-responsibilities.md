# Improvement and responsibilities: Routine policyholder correspondence

**Status: Reviewed** (approved by the user, 2026-10-06). v1. The later sections ("Answers received after approval", "Follow-up answers") were approved by the user on 2026-10-06; items inside them keep their Proposed, Assumption and Unresolved labels. Sources: Reviewed workflow map and description, value thesis, operating model, adoption plan and success baseline; the course "who does what" boundary ([case-context.md](case-context.md)); your answers. Everything here is **Proposed** unless marked as from a Reviewed document. No numeric targets are on record, so I haven't invented any.

## Better Outcome (Proposed)
Routine letters reach policyholders sooner after an approved claim decision, because handlers start from a first draft in the approved template and spend their effort verifying details rather than recreating wording. The handler still verifies every detail and approves every letter.

**Caveat:** this assumes drafting is a meaningful part of the 2.4 business days. Where those days go isn't measured (map, Reviewed), so the improvement is a hypothesis, not evidence.

## Success signals
- Median business days from approval to send falls below the 2.4-day baseline (**no target set**).
- Median drafting time stays down (sampled 18 to 11 minutes in the pilot) and drafts need fewer wording revisions.
- Handlers return to the workflow week after week, including the 14 who were blocked by access.
- Handlers act on the AI's flags of missing or inconsistent information.
- Every sent letter shows handler approval.
- Complaints about how operators handle policies don't rise, and policyholder feedback shows no more frustration (Charter measures).

## Failure signals
- Drafting is faster but letters don't go out sooner.
- Handlers spend more time verifying or tracing details than before (increased effort).
- Errors found at review rise, or errors reach policyholders, shown by complaints.
- A letter is sent without handler approval, or automatically.
- The AI uses source information that isn't permitted, or real data is used before the data-handling findings (Q18).
- A conflict, legal or unusual case is drafted by AI instead of being referred.
- Handlers stop using the workflow, or access problems persist.

## Safeguards (from Reviewed documents unless marked)
- A handler verifies every detail and approves every letter before it is sent. AI prepares a first draft only.
- No letters are sent automatically without human approval (your exclusion, 2026-10-06).
- Conflict and legal cases stay out of scope. The legal specialist decides legal conflict cases.
- Use stays within the current pilot scope. A successful pilot doesn't authorise routine use. The Chief Claims Officer approves routine use and additional resources.
- Only permitted source information is used. What is permitted depends on Q18 (**unresolved**).
- Handlers report results weekly. A failed test leads to a blameless retrospective.
- Escalation follows the Operating Model. Policy, privacy or risk concerns go to the Responsible AI and Privacy Working Group.
- **Proposal:** use only the approved letter template. Who approves it is **unresolved**.

## Proposed responsibilities by step

| Step | Level | What AI does | Who reviews, approves or handles exceptions |
|---|---|---|---|
| **1. Gather information** | **Person completes** | Nothing in the First initiative. Finding details across systems is the Next opportunity. | Handler collects the details from authorised systems. If something is missing, the handler resolves it or refers the case. |
| **2a. Format into the template** | **AI completes** *(course example; Proposed for Northfield)* | Formats permitted source information into the approved letter template. Only appropriate if agreed rules permit it (Q18). | Handler reviews the result at step 3 in every case. |
| **2b. Draft the letter** | **AI supports with human review** | Drafts the letter and flags missing or inconsistent information. | Handler reviews the draft and the flags. The Workflow owner handles questions the handler can't resolve. |
| **3. Review the draft** | **Person completes** | Nothing. The AI's flags are input, not a check. | Handler verifies details against sources, and checks wording, tone and required statements. |
| **4. Approve or refer** | **Person completes** | Nothing. AI doesn't approve, send or decide whether a case is routine. | Handler approves the routine letter, or refers an unusual case. A specialist reviews referrals (**receiver unknown**). The legal specialist handles legal conflict cases. |

## Who coordinates (existing roles; assignments Proposed unless Reviewed)
- **Coordinates implementation:** AI Transformation Program Manager (you). *(Reviewed)*
- **Contributors:**
  - Claims handlers: draft review, verification, approval, weekly reports.
  - Claims Correspondence Operations Manager (Workflow owner): evidence, workflow changes, data-handling review. *(Reviewed)*
  - Enterprise Applications Administrator: access and configuration. *(Reviewed; the access fix is unconfirmed)*
  - Automation Solutions Architect: data handling, integrations. *(Reviewed)*
  - Claims Learning and Quality Manager: guidance and support. *(Proposal, unconfirmed)*
- **Specialists:** Responsible AI and Privacy Working Group (policy, risk); legal specialist (legal cases only, out of scope). The Chief Claims Officer approves routine use and resources.

## Missing information and unconfirmed items
1. Which source information is "permitted" (Q18).
2. Who approves the letter template, and whether one exists for every routine letter type.
3. Referral rules, and who receives referrals.
4. Where the elapsed time goes within the 2.4 days. This decides whether the improvement is plausible.
5. The roles of compliance reviewers and team leaders (Q4).
6. Targets for approval-to-send days, drafting time and revisions.
7. Whether the Workflow owner agrees with these responsibilities.

## Answers received after approval (2026-10-06): Reviewed (approved by the user, 2026-10-06; as you report where marked)
Your answers to the missing items. They don't change the approved content above. Where they could, they are flagged below.

1. **Permitted sources (Q18), partly answered by you.** The AI may have read-only access to the policyholder's data, history, claims history and claim notes, from the source. This is your answer. The Automation Solutions Architect and the Claims Correspondence Operations Manager, who were assigned Q18, haven't confirmed it, so Q18 stays open for their confirmation.
2. **Templates.** Templates are predefined by use case, and the handler selects one before drafting. Who approves the templates is **still unanswered**.
3. **Unusual cases.** A case is unusual if the claim is very large, anomalous or suspected fraud, including when the handler senses fraud. How large counts as "big", and what counts as anomalous, aren't defined (the handler's judgement). Region differences: you withdrew that question. The course fact that referral processes vary by region stays on record.
4. **Where the time goes (your account, not measured).** Drafting is only one part. Handlers also cross-verify information against the databases and past records, go through fraud detection, then have the letter reviewed and wait for approval.
5. **Referrals.** After the handler finishes, the case goes to a specialist team: for example a medical specialist review team, or vehicle or home insurance teams.
6. **Targets:** to be decided later. Unresolved.
7. **Workflow owner:** you said "Flow agrees". I've read this as the Claims Correspondence Operations Manager. This is your report; I haven't heard from them.
8. **Q4** (roles of compliance reviewers and team leaders): not answered. Still open.

**Conflicts and gaps with Reviewed documents (for your decision)**
- **Fraud detection and a review-and-approval wait aren't in the Reviewed workflow map.** The map has the handler approving routine letters. "Get reviewed and wait for approval" suggests someone else's approval. If so, who approves, and does the handler still approve every letter?
- **Referral scope.** The map treats the specialist referral as for unusual cases. Your answer could also mean every letter goes to a specialist. Unclear.
- **Read-only access.** If the AI itself reads the source, that overlaps with the Next opportunity (policy lookup support), and step 1 in the responsibilities table would change. If the handler supplies the data, nothing changes.
- **Evidence.** If most of the 2.4 days is verification, fraud checks and waiting, faster drafting may not shorten it. The Better Outcome caveat stands.

## Follow-up answers (2026-10-06): Reviewed (approved by the user, 2026-10-06; as you report where marked)
These update the section above.
- **Fraud check and approval wait: removed at your request.** They are not added to the workflow map. This also withdraws the part of your earlier time account that named them. What's left of that account is that handlers cross-verify information against the databases and past records. Where the 2.4 days go is still **not measured**. The definition of an unusual case (large, anomalous or suspected fraud) stays, because it concerns when a handler refers a case, not a separate fraud-check step.
- **Data (Q18) still open.** Some data is permitted for AI read-only use now. You said the complete data policy covers more than data purposes, but the rest isn't stated. Which data is permitted beyond the list you gave, and what else the policy requires, are **Unresolved**. The Architect and the Workflow owner still need to confirm.
- **Compliance review (partly answers Q4).** Compliance reviewers review a checklist after the handler drafts the letter. This isn't in the Reviewed workflow map or the responsibilities table. Where it sits relative to the handler's approval, and whether it applies to every routine letter, are **Unresolved**.
- **Open:** whether the AI reads the source itself or works on data the handler supplies. Your answer suggests some read access exists, but not which.
