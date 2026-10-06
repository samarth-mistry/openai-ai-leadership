# AI Strategy Brief: Northfield Mutual (AI Leadership course, OpenAI Academy)

This folder is a working space, not software. It holds the **AI Strategy Brief** being built one course activity at a time, using the fictional **Northfield Mutual** case. Nothing here needs building, linting or testing. Last updated 2026-10-07.

**Rules the work follows** (set in [CLAUDE.md](CLAUDE.md)): use only project material and what the user approves; no web search or general knowledge; never invent evidence, policies, approvals, owners, dates or results; label items **Assumption**, **Proposed** or **Unresolved**; carry reviewed decisions forward and flag conflicts; do one course step at a time; nothing is **Reviewed** until the user explicitly approves it.

## 1. What we discussed
- **The case:** Northfield Mutual is a fictional insurer with about 2,000 employees. Claims handlers recreate similar wording and check details across several systems when writing routine policyholder letters. AI may draft; a handler verifies every detail and approves every letter before it is sent.
- **The goal:** a six-month roadmap (First, Next, Later), the First opportunity developed into a priority AI initiative, and a final sponsor recommendation.
- **Key decisions along the way:**
  - You play the **AI Transformation Program Manager**, not the claims operations director (corrected 2026-10-04). The **Chief Claims Officer** is the executive sponsor.
  - **First:** routine policyholder correspondence. **Next:** policy lookup support. **Later:** complex claim recommendations.
  - **Baseline:** a median of 2.4 business days from approval to sending. Pilot: 26 of 40 handlers repeated use, and sampled drafting time fell from 18 to 11 minutes (evidence level **Work Change**, not yet business impact).
  - Your earlier time estimates ("almost a day", then about 2 hours) were withdrawn.
  - Adoption: 14 handlers were blocked by access; replies to concerns, end-of-day updates and conflict cases stay out of the pilot.
  - Design: the AI never reads source systems, the handler copies in only permitted data, and nothing is sent automatically.
  - Tests: Cases 1 to 3 passed; Cases 4 and 5 failed, then passed on rerun **as you report**. Recommendation: **Fix**, then your report that the Chief Claims Officer approved routine use and two other teams.

## 2. What we have done
Twenty-seven activities, from project set-up to the handoff check, all marked Reviewed (listed in section 3). The roadmap, value thesis, operating model, adoption plan, design spec, requirements, test set, handoff check and Workflow Package are complete. **Not done yet:** support and maintenance, and the final recommendation for sponsors and partners.

## 3. Activities in sequence
Dates are from the files' own status lines. "Created" is the file-system date; some files were rewritten later, so it can be later than the first draft.

| # | Course activity | File | Created | Reviewed |
|---|---|---|---|---|
| 1 | Project set-up (`/init`) | [CLAUDE.md](CLAUDE.md) | 2026-09-23 | n/a (instructions) |
| 2 | Case context and your answers; later the pilot results, program roles, current workflow and "who does what" boundary | [case-context.md](case-context.md) | 2026-10-04 | With the context note, 2026-09-27 |
| 3 | Context note | [context-note.md](context-note.md) | 2026-09-27 | 2026-09-27 |
| 4 | Charter judgments | [charter-judgments.md](charter-judgments.md) | 2026-09-29 | 2026-10-03 |
| 5 | AI Leadership Charter | [leadership-charter.md](leadership-charter.md) | 2026-09-29 | 2026-10-03 |
| 6 | Opportunity statements (all three) | [opportunity-statement.md](opportunity-statement.md) | 2026-10-03 | 2026-10-03 |
| 7 | Roadmap inputs check | [roadmap-inputs.md](roadmap-inputs.md) | 2026-09-29 | 2026-10-03 |
| 8 | Assumptions standing in for parked questions | [working-assumptions.md](working-assumptions.md) | 2026-10-03 | 2026-10-06 |
| 9 | Six-month AI Strategy and Roadmap | [roadmap.md](roadmap.md) | 2026-10-04 | 2026-10-03 |
| 10 | Success and baseline | [success-baseline.md](success-baseline.md) | 2026-10-04 | 2026-10-04 |
| 11 | Evidence judgment | [evidence-judgment.md](evidence-judgment.md) | 2026-10-04 | 2026-10-04 |
| 12 | Value Thesis and Evidence Plan | [value-thesis.md](value-thesis.md) | 2026-10-04 | 2026-10-04 |
| 13 | Responsible AI Operating Model | [operating-model.md](operating-model.md) | 2026-10-04 | 2026-10-04 |
| 14 | Adoption context | [adoption-context.md](adoption-context.md) | 2026-10-05 | 2026-10-05 |
| 15 | Support recommendation | [support-recommendation.md](support-recommendation.md) | 2026-10-05 | 2026-10-05 |
| 16 | 30/60/90 AI Adoption Plan | [adoption-plan.md](adoption-plan.md) | 2026-10-05 | 2026-10-05 |
| 17 | Current workflow description | [workflow-description.md](workflow-description.md) | 2026-10-06 | 2026-10-06 |
| 18 | Current workflow map | [workflow-map.md](workflow-map.md) | 2026-10-06 | 2026-10-06 |
| 19 | Improvement and responsibilities | [improvement-responsibilities.md](improvement-responsibilities.md) | 2026-10-06 | 2026-10-06 |
| 20 | Priority AI Workflow Design Spec | [design-spec.md](design-spec.md) | 2026-10-06 | 2026-10-06 |
| 21 | Requirements context | [requirements-context.md](requirements-context.md) | 2026-10-06 | 2026-10-06 |
| 22 | Observable requirements (R1 to R18) | [requirements.md](requirements.md) | 2026-10-06 | 2026-10-06 |
| 23 | Test set (five cases) | [test-set.md](test-set.md) | 2026-10-06 | 2026-10-06 |
| 24 | Recommend Introduce, Fix or Stop (Fix) | section in [requirements.md](requirements.md) | 2026-10-06 | 2026-10-06 |
| 25 | Handoff gap check | [handoff-gaps.md](handoff-gaps.md) | 2026-10-06 | 2026-10-06 |
| 26 | Workflow Package | [workflow-package.md](workflow-package.md) | 2026-10-06 | 2026-10-06 |
| 27 | Handoff check of the Workflow Package | [handoff-check.md](handoff-check.md) | 2026-10-07 | 2026-10-07 |
| 28 | This summary | README.md | 2026-10-07 | n/a |
| — | **Support and maintenance** | not started | | |
| — | **Final recommendation to sponsors and partners** | not started | | |

## 4. Entity table
People, groups and things in the Northfield case, with where each comes from.

| Entity | Role in the brief | Source | Confirmed? |
|---|---|---|---|
| Northfield Mutual | Fictional insurer, about 2,000 employees | Case | Yes |
| You, AI Transformation Program Manager | Lead and coordinate; approve the roadmap; start bounded tests; decide Revise, Continue, Pause, Stop within scope | Course; your correction 2026-10-04 | Yes |
| Chief Claims Officer | Executive sponsor; resources; approval of routine use (approved routine use and two other teams, **as you report**) | Course | Role yes; approval as reported |
| Claims Correspondence Operations Manager | Workflow owner; approves templates and required statements; reviews data handling | Course; your answers | Role yes; agreement as reported |
| Claims handlers (40 in the pilot) | Intended users; verify and approve every letter | Course | Yes |
| Enterprise Applications Administrator | Access and configuration | Course | Role yes; support role as reported |
| Automation Solutions Architect | Data handling; reliability fixes | Course; your correction | Role yes; agreement as reported |
| Claims Learning and Quality Manager | Guidance, training and support | Course | Role yes; agreement as reported |
| Responsible AI and Privacy Working Group | Policy, risk, specialist review | Course | Yes |
| Legal specialist | Legal conflict cases (out of the pilot) | Your answers | Yes |
| Specialist review teams (medical, vehicle, home) | Receive referrals of unusual cases | Your answers | As reported |
| Compliance reviewers | Check a checklist after drafting; treated as outside the design, assumed quick | Your answers | **Assumption** |
| Team leaders and managers | Roles not recorded (Q4) | Case | **Unresolved** |
| Policyholders | Receive the letters | Case | Yes |
| Two receiving teams | Similar teams in a different region and office | Your answers | **Not named** |

| Information entity | What it is | Status |
|---|---|---|
| Routine letter | Letter sent after an approved claim decision | In scope |
| Approved template | Predefined by use case; handler selects; Workflow owner approves | As reported |
| Permitted data | Policyholder data, history, claims history and claim notes, copied in by the handler | Confirmed as you report; written findings not on record |
| Baseline | 2.4 business days, approval to send | Reviewed |
| Out-of-scope cases | Conflict, legal, unusual (big, anomalous, suspected fraud), replies to concerns, end-of-day updates, policy lookup, automatic sending | Reviewed |

## 5. Memory files
Outside this folder, in `~/.claude/projects/-Users-tech-Desktop-Samarth-openai-ai-leadership/memory/`. They let a new session pick up where the last one stopped.

| File | Created | Purpose |
|---|---|---|
| `MEMORY.md` | 2026-10-03 | One-line index loaded at the start of each session |
| `brief-progress.md` | about 2026-10-03; updated through 2026-10-06 | Current step, file map and open conflicts. Edits re-create the file, so its file-system date shows 2026-10-06 |

The conversation transcripts (`*.jsonl`, six sessions since 2026-09-23) sit in the folder above the memory directory.

## 6. What each file is for (high level)
- **Foundations (1 to 3):** project rules, the case, and what is known and unknown.
- **Leadership (4 to 5):** your role, how you lead, what you can decide and what needs a sponsor or specialist.
- **Opportunities and roadmap (6 to 9):** what to work on, evidence, constraints, and the First, Next and Later order. `working-assumptions.md` holds stand-ins for questions you parked.
- **Value and governance (10 to 13):** what success looks like, how strong the evidence is, the value thesis, and who owns, reviews and approves what.
- **Adoption (14 to 16):** who needs support, the main barrier, and a 30/60/90 plan.
- **Workflow design (17 to 20):** how the work runs today, the improvement, AI and human responsibilities, and the Design Spec.
- **Requirements and testing (21 to 24):** what the workflow must do, tests, and the Fix recommendation.
- **Handoff (25 to 27):** what the receiving teams still need, the package to give them, and a check of the package from their side (12 gaps, 5 blocking).

## 7. Still open
- **To draft:** support and maintenance; the final recommendation.
- **Handoff check gaps:** five blocking gaps (tool and access route, start conditions, approval status line, ownership for the receiving teams, support route) and seven others, in [handoff-check.md](handoff-check.md). The package itself hasn't been revised.
- **Receiving teams:** names, and a lead to describe their current flow.
- **Tests and requirements:** the untested requirements; the final-decision wording requirement; pass criteria and targets.
- **Definitions and accountability:** the "big" and "anomalous" thresholds; who is accountable for a sent error; how approvals are logged.
- **Evidence:** business impact (approval-to-send days against 2.4); the Case 4 and 5 rerun evidence; the Architect's written findings.
- **Dates:** the plan start date.
- **Items "as you report":** the reruns, the Chief Claims Officer's approval, and the owners' confirmations are recorded from your word. I haven't seen the evidence.
