# Responsible AI Operating Model: Routine policyholder correspondence

**Status: Reviewed** (approved by the user, 2026-10-04). v2, with your role, sponsor and data-handling corrections of 2026-10-04. Sources: Reviewed roadmap, Charter, success and baseline, evidence judgment and value thesis; program roles supplied by the course ([case-context.md](case-context.md)). Labels: **Course** = role and responsibility as the course states it; **Charter** = Reviewed; **Correction** = your decision of 2026-10-04; **Proposal** = suggested assignment; **Assumption** = not yet confirmed.

## 1. People and ownership

| Role | Job title | Owns or contributes | Source |
|---|---|---|---|
| Executive sponsor and functional leader | Chief Claims Officer | Sets priority, commits capacity, clears barriers; decides on additional manpower and material resources | Course; Correction |
| AI adoption lead and initiative lead | AI Transformation Program Manager (you) | Leads the initiative; coordinates review and approved action; approves the roadmap; reallocates assigned resources; starts bounded tests; runs blameless retrospectives on failed tests | Course; Correction; Charter |
| Workflow owner | Claims Correspondence Operations Manager | Reviews pilot evidence and recommends changes; tracks business days from approval to send against the 2.4-day baseline; reviews and changes data handling | Course; value thesis; Correction |
| Intended users | Claims handlers (40 in the pilot) | Test the workflow and report results; verify every detail, make changes and approve every letter before it is sent | Course; case |
| Technical administrator | Enterprise Applications Administrator | Approved access and configuration. **Proposal:** also maintains access and configuration after the pilot | Course; Proposal |
| Technical partner | Automation Solutions Architect | Integrations, automation and reliability; handles data handling for policyholder and claim data. **Proposal:** also owns reliability fixes after the pilot | Course; Correction; Proposal |
| Enablement partner | Claims Learning and Quality Manager | Guidance, learning and support. **Proposal:** owns handler guidance and ongoing support | Course; Proposal |
| Governance partner | Responsible AI and Privacy Working Group | Policy, risk and specialist review | Course |
| Specialist owner | Legal specialist | Decisions on legal conflict cases. Out of the pilot's scope | Charter |
| Other affected people | Compliance reviewers, team leaders, managers | Role in the letter process not yet recorded (Q4) | Context note |

## 2. Decision boundaries

| Role | Can decide | Needs input from | Approval required from |
|---|---|---|---|
| Claims handler | Changes to each draft; whether a letter is ready to send | Workflow owner on unclear cases | None. Handler approval is the required check on every letter |
| Workflow owner | What workflow changes to recommend; reviews and changes data handling | Handlers' test results; the Architect | You coordinate the change; the Chief Claims Officer if it needs capacity beyond your assigned resources |
| AI Transformation Program Manager (you) | Roadmap approvals; reallocating assigned resources; starting bounded tests within them; routing approved actions | Workflow owner's evidence; partners as needed | None within your assigned resources (Charter) |
| Chief Claims Officer | Priority; capacity; additional manpower and material resources; clearing barriers; approval of routine use (confirmed 2026-10-04) | You | — |
| Automation Solutions Architect | How data handling, integrations and reliability are carried out | You; Workflow owner | Workflow owner reviews and changes data handling |
| Responsible AI and Privacy Working Group | Policy, risk and specialist review findings | You | — |
| Legal specialist | Legal conflict cases | Handlers | — |

**Safeguards that don't change:** AI prepares a first draft only. A claims handler verifies every detail, makes any needed changes and approves every letter before it is sent. Conflict and legal cases stay out of scope (working assumption, Q5).

**Trial permission versus routine use**
- **Currently authorized:** a bounded trial within your assigned resources: AI first drafts of routine letters, used by the pilot handlers, with handler approval on every letter. Next step (value thesis, Reviewed): continue within the current pilot scope.
- **Not authorized:** routine repeat use, or any expansion beyond the pilot scope. A successful pilot doesn't authorize either.
- **Next decision:** whether to propose use beyond the pilot scope, once the business days from approval to send have been compared with the 2.4-day baseline.
- **Still needed before that decision:** evidence of business impact against the baseline; approval of routine use from the Chief Claims Officer (confirmed 2026-10-04); data-handling findings (Q18, assigned to the Automation Solutions Architect and the Claims Correspondence Operations Manager (2026-10-04)); confirmed support and maintenance owners (Proposals above); additional resources from the Chief Claims Officer if the scope grows.

## 3. Handoffs

| Handoff | Trigger | Inputs | Recipient | Next action |
|---|---|---|---|---|
| Draft to approval | AI prepares a first draft of a routine letter | Draft; claim and policy details | Claims handler | Verify every detail, edit, approve and send, or reject |
| Test results | Every week during the pilot (your decision, 2026-10-04) | Use, drafting time, wording revisions, issues found | Workflow owner | Review evidence against the baseline |
| Recommended change | Workflow owner's evidence review identifies a change | Evidence summary and recommendation | AI Transformation Program Manager (you) | Coordinate review with partners, then approve within your scope or route to the Chief Claims Officer |
| Questions and approved actions | A recommendation needs technical, enablement or governance input, or is approved | The question or approved action | Relevant partner (Enterprise Applications Administrator, Automation Solutions Architect, Claims Learning and Quality Manager, or Working Group) | Partner answers or carries out the action |
| Priorities and resources | Chief Claims Officer sets priority or commits capacity | Decision on priority or capacity | AI Transformation Program Manager (you) | Update the plan and inform the workflow owner |
| Monthly review | Each month (Charter) | Speed, cost, correctness (complaints) and frustration (feedback) | Chief Claims Officer | Review progress and act on roadblocks |

## 4. Escalation pathways

| Issue | Taken to | Who responds |
|---|---|---|
| A handler can't verify a detail, or a draft looks wrong | Workflow owner | Workflow owner; letter isn't sent until a handler approves it |
| Claim details conflict with policy terms | Out of pilot scope: handled in the current manual process | Handler; legal specialist for legal conflict cases |
| Access, configuration or system problem | You | Enterprise Applications Administrator |
| Integration, reliability or data-handling problem | You | Automation Solutions Architect; Workflow owner reviews and changes data handling |
| Guidance or training need | Workflow owner | Claims Learning and Quality Manager |
| Policy, privacy or risk concern | You | Responsible AI and Privacy Working Group |
| A test fails | You | Blameless retrospective with everyone accountable (Charter) |
| Barrier the team can't clear, or capacity needed | You | Chief Claims Officer |

## Remaining gaps
1. **Resolved 2026-10-04:** the Chief Claims Officer approves routine use (A9 confirmed by you).
2. **Resolved 2026-10-04:** claims handlers report test results every week.
3. **Unresolved:** the roles of compliance reviewers, team leaders and managers (Q4); data-handling findings (Q18): assigned to the Automation Solutions Architect and the Claims Correspondence Operations Manager (2026-10-04). They confirm whether the rules allow claim and policy data in the drafting tool, under what conditions, and what needs improving.

## Agreed conditions that trigger review
- A failed test's retrospective produces a fix that needs a decision outside your scope (Charter).
- Results are in for business days from approval to send against the 2.4-day baseline (value thesis).
- Anyone proposes use beyond the current pilot scope.

## Update 2026-10-06: Reviewed (approved by the user, 2026-10-06; as you report where marked)
Q18: you report that the Automation Solutions Architect and the other owners have confirmed which data handlers may copy into the AI (policyholder data, history, claims history and claim notes). I haven't changed the Reviewed text above.
