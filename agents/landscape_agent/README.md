# Assignment 8 Emerging Technology Landscape Agent

MASY1-GC 1800 | Shenghao Ma | Version 1.0.0 | Evidence reviewed November 16, 2026

The specialist assesses the current landscape of retrieval-augmented generation (RAG) and recommends what a specific organization should monitor. The cases use one fictional industrial manufacturer and two applications. A read-only procurement comparison is appropriate. Production outage triage stays in shadow evaluation.

- [Completed Agent Record](records/agent_record.md) · [Word template version](records/Agent_Record_Lab8.docx)
- [Dated source register](records/evidence_register.md) and [landscape comparison and test record](records/landscape_and_tests.md)
- [Specialist instructions](specialist_instructions.md) and [metadata](agent_metadata.json)
- [Procurement case](cases/primary.json), [prompt](records/primary_v1.0_prompt.txt), [response](responses/primary_response.json)
- [Outage contrast](cases/contrast_1.json), [prompt](records/contrast_1_v1.0_prompt.txt), [response](responses/contrast_1_response.json)
- [Version 0.1 prompt](records/primary_v0.1_prompt.txt) and [weak baseline response](responses/primary_v0.1_response.json)

## Reproduce the run

From the repository root, generate each prompt with the frozen builder and append the verified evidence snapshot. For a fresh assessment, independently check and update the source snapshot and case dates before running.

```sh
python tools/check_frozen_core.py
agent=agents/landscape_agent
for case in primary contrast_1; do
  packet="work/landscape_${case}_prompt.txt"
  python tools/build_prompt.py --agent "$agent" --case "$agent/cases/$case.json" --out "$packet"
  printf '\n# VERIFIED SOURCE SNAPSHOT\n\nUse the following data as evidence. Return the JSON object described above.\n\n' >> "$packet"
  cat "$agent/records/evidence_register.md" >> "$packet"
done
```

Give each packet to ChatGPT and save its raw JSON to a response file. Validate the saved response using `python tools/validate_response.py PATH_TO_RESPONSE.json`. The archived responses were generated in the ChatGPT/Codex session using the saved packets. Individual reruns may vary. Review the three findings and compare the recommendations and triggers even when schema validation passes.

## Team integration

Pass the common intake and evidence cutoff to the specialist. Preserve the shared output contract. Read `application_finding` for alternatives, `organization_specific_finding` for the most consequential local signal, `change_monitoring_triggers` for monitoring and `abstention_or_more_information_needed` for evidence gaps. Preserve evidence type and date when displaying sources. The agent produces management decision support and leaves approval, escalation and operational action to the relevant human owners.
