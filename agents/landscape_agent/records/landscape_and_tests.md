# Landscape comparison and test record

Evidence cutoff: 2026-11-16. Case inputs and thresholds are classroom assumptions. The tests below assess the specialist's reasoning and output. The proposed operational pilots remain unrun.

| Dimension | Primary: requisition policy help | Contrast: production IT outage triage |
| --- | --- | --- |
| Position | Evaluate read-only RAG against existing policy support | Evaluate analyst support in shadow replay; keep live routing |
| Strongest conventional alternative | Curated policy search and staffed procurement help desk | Approved severity rules and incident commander dispatch |
| Platform or complement | Joule for a future comparison, subject to tenant entitlement, corpus coverage, permissions and cost | Jira controlled intent flows for structured intake, subject to access and fallback replay |
| Performance criterion | Correct disposition and time to a correct answer by language | Time to correct escalation and critical under-triage |
| Decisive signal | Current bilingual policy citations and reliable escalation of exceptions | Whether AI suggestions miss or delay critical paging |
| Stop or reopen | Suspend affected answers on obsolete policy or bypassed human review. Add Joule only after entitlement, cost and bilingual sandbox checks. | Suspend testing on any critical under-triage, mandatory paging delay or unauthorized exposure. Rerun fallback testing after routing or permission changes. |

## Testing and revision

| Run or check | Result |
| --- | --- |
| Frozen scaffold | The scaffold integrity checker and original package checksums passed. Only the landscape specialist folder was added to the starter tree. |
| Primary and contrast | Both final responses passed the frozen validator and full JSON Schema Draft 2020-12 validation. Both case inputs passed the full input schema. |
| General conclusion held stable | Both outputs use the same dated conclusion on commercial implementation and deployment-dependent answer quality. The general finding strings are identical. |
| Context changed the decision | Procurement can compare read-only help with search and a help desk. Outage triage faces more consequential mistakes in estimating severity, so the live rules and human escalation remain in place while the assistant is replayed offline. Vendor dependencies, owners and gates change accordingly. |
| Preserved weakness | The [v0.1 primary response](../responses/primary_v0.1_response.json) passes schema validation but says to review quality, volume and updates “regularly.” It gives no owner, cadence, threshold or decision. Its Joule watch item also lacks a scoped vendor citation. |
| Revision | The specialist now requires each trigger to name its owner, frequency or event, observable gate and resulting decision. The evidence rule requires tenant verification, source-scope checks and a shared dated snapshot. The rerun provides accountable triggers in both contexts. Because both the evidence packet and instructions changed, this is a before/after demonstration and does not isolate their individual effects. |
| Limits | One saved response per final case measures neither repeatability nor operational accuracy. Procurement thresholds and incident replay gates are proposed. The outage test changes both application and adoption posture, so it demonstrates context sensitivity without isolating their individual effects. |

## Evidence scope

Vendor sources establish described capabilities and prerequisites. Independent empirical sources provide contrary reliability evidence and directional productivity evidence from specific settings. NIST supplies contextual risk guidance. Local prices, permissions, test outcomes, and return on investment remain unknown. See the [dated source register](evidence_register.md) and the exact [primary](../responses/primary_response.json) and [contrast](../responses/contrast_1_response.json) monitoring rules.
