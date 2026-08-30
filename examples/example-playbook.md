# Example Playbook: Peer and competitor landscape

**Status:** Example / draft / non-production. This is not an Official or Community released Playbook and has not been evaluated as a production method.

The embedded definition demonstrates the contract without creating a production catalogue entry. It asks an external AI to compare a supplied CharityGraph organisation or program with evidenced peers while keeping similarity distinct from proven competition.

```json
{
  "schema_version": "playbook-definition-v0.1",
  "id": "playbook:peer-competitor-landscape-example",
  "version": "v0.1.0",
  "title": "Peer and competitor landscape",
  "description": "Prepare an evidence-grounded landscape around a CharityGraph organisation or program for a stated decision question.",
  "governance_status": "community",
  "lifecycle_status": "draft",
  "contributors": [
    {
      "name": "CharityGraph example",
      "role": "contract illustration",
      "attribution": "CharityGraph contributors"
    }
  ],
  "subject_grains": ["organisation", "program", "service"],
  "parameters": [
    {
      "id": "subject_ref",
      "label": "CharityGraph organisation, program or service",
      "type": "subject_ref",
      "required": true,
      "visibility": "public"
    },
    {
      "id": "geography",
      "label": "Geography to consider",
      "type": "geography",
      "required": false,
      "visibility": "public"
    },
    {
      "id": "decision_question",
      "label": "What decision should this analysis inform?",
      "type": "text",
      "required": false,
      "visibility": "private"
    }
  ],
  "context_requirements": {
    "charitygraph_references": ["canonical subject/program/service URLs supplied by the invocation"],
    "data_release_or_snapshot": null,
    "retrieval_mode": "either",
    "external_evidence": "If used, identify demand/need or other external evidence separately from CharityGraph material.",
    "model_capabilities": ["citation-capable retrieval or supplied context", "structured comparison"]
  },
  "base_policy_version": "playbook-base-policy-v0.1",
  "instruction_template": "Use known CharityGraph context to eliminate questions before asking the user. Compare evidenced scope, activities, populations, geography and relationships. Describe similarity as similarity; do not call organisations competitors without evidence of competition. If CharityGraph material cannot be retrieved or was not supplied, say so.",
  "output_expectations": [
    "scope-aware peer landscape",
    "citations to CharityGraph and material external evidence",
    "uncertainty, missingness and retrieval status",
    "separate similarity from proven competition"
  ],
  "limitations": [
    "This draft does not establish market demand or unmet need.",
    "It does not infer causation, impact or organisational quality.",
    "Downstream analysis is not canonical CharityGraph knowledge."
  ],
  "feedback_routes": ["data_error", "playbook_method_problem", "execution_model_retrieval_problem"],
  "licence": "CC BY 4.0"
}
```

An invocation may supply the subject references and optional geography, ask the user only for a genuinely missing decision question, and use retrieval or packaged public context. The model must disclose inability to access intended CharityGraph material rather than silently substituting generic knowledge.
