# Specialist Agent Record

MASY1-GC 1800 | Assignment 8

The procurement case supports a bounded read-only comparison. The production outage contrast supports shadow evaluation. The commit listed below identifies the tested agent implementation.

## A. Agent and Version

| Field | Student record |
| --- | --- |
| Student / team | Shenghao Ma (Harry) / Individual |
| Assignment / specialist agent | Assignment 8 / Emerging Technology Landscape Agent v1.0.0 |
| Date | November 16, 2026 |
| GitHub repository | https://github.com/Harry-max264/Lab-8 |
| Branch | assignment-8 |
| Commit | [`4263072d8755e131c55d5b8817fd21a5a1b3b315`](https://github.com/Harry-max264/Lab-8/commit/4263072d8755e131c55d5b8817fd21a5a1b3b315) |
| Frozen scaffold version | MASY1800_ET_Agent_Scaffold_v1_0 |

## B. Specialist Purpose and Context

| Field | Student record |
| --- | --- |
| Governing analytical question | Where does this technology sit in the current landscape, and what signals should this organization monitor next? |
| Emerging technology | Retrieval-augmented generation (RAG) over internal authoritative documents |
| Intended application | Read-only employee purchase requisition policy and how-to questions |
| Organization / industry | Fictional mid-sized industrial manufacturer using SAP Ariba and Jira Service Management Cloud |
| Adoption posture | Moderate fast follower for procurement. Conservative for production outages. |
| Risk / consequence context | An incorrect response can misroute approvals. Policy owners retain approval and exception authority. |
| Management question / time horizon | In 90 days, decide whether to advance a read-only pilot and whether to compare Joule. |

## C. Three-Level Finding

| Field | Student record |
| --- | --- |
| ET generally | Retrieval-backed generation is commercially implemented for knowledge assistance. Answer and citation quality depend on the deployment. Independent studies document residual hallucinations. |
| ET for this application | Compare read-only RAG with curated policy search and a staffed procurement help desk. Measure time to a correct disposition in English and Mandarin. |
| ET for this application in this organization | Versioned policies support a reversible evaluation. Verify bilingual citations and approval routing first. Check tenant entitlement and coverage before adding Joule. |
| Bounded management implication | Run a paired, 60-task offline comparison with 30 per language. Keep exception handling with procurement. |
| Confidence / uncertainty | Moderate confidence in the evaluation design. Local quality, costs, savings, and tenant access require measurement. |
| What evidence or condition would change the conclusion | Advance only after each language reaches 27 of 30 correct dispositions, median time to a correct answer improves at least 20% per language, and critical routing errors and disclosures total zero. These are proposed gates. |

## D. Evidence and Testing

| Field | Student record |
| --- | --- |
| Most important evidence/source(s) | Atlassian virtual service agent documentation, Magesh et al. (2025), NIST AI 600-1, and SAP release and support documentation. See the [dated source register](evidence_register.md) for links and claim limitations. |
| Primary test - result | Final procurement response passed both validators. It gives a read-only comparison, a conventional baseline, and weekly and event-based review triggers. |
| Contrast test - what appropriately stayed stable | Both cases preserve the same dated general conclusion on commercial availability and deployment-dependent reliability. |
| Contrast test - what appropriately changed | Outage triage remains in shadow replay. Human dispatch and severity rules stay live. Critical under-triage replaces bilingual policy coverage as the leading signal. |
| Weakness/failure found | The initial output suggested checking quality “regularly” and gave no owner, cadence, gate, or action. It passed schema validation. |
| Revision made and why | Added a monitoring rule that requires an owner, cadence, gate and action, plus dated claim scope and tenant verification. Both final cases satisfy that rule. |
| Remaining limitation / abstention condition | The tests use synthetic cases and a single output per final case. Abstain on ROI, vendor selection, or live routing until representative local evidence exists. |

## E. Independent Judgment and Handoff

| Field | Student record |
| --- | --- |
| Is the agent credible enough for team consideration? Why? | Yes, for team consideration as a bounded landscape specialist. Both cases adhere to the shared contract and make different, evidence-calibrated decisions. Operational accuracy remains unmeasured. |
| Most important recommendation to the team | Retain curated search and the help desk as the procurement baseline. Watch bilingual source and routing quality weekly. Preserve source type, cutoff, monitoring triggers and abstention fields at handoff. |
| AI / verification note | ChatGPT/Codex specialized the prompt, generated and critiqued the saved outputs, and ran scaffold and full schema validation. Material claims were checked in original vendor docs, published studies and NIST guidance. |
