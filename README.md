# CharityGraph Playbooks

**Status:** Product contract and example repository; no released Playbooks yet

CharityGraph Playbooks is the fourth CharityGraph product:

- **Builder** constructs governed knowledge.
- **Data** publishes governed reusable data.
- **Viewer** lets people inspect and navigate it.
- **Playbooks** publishes governed, open analytical methods for using CharityGraph with general-purpose AI.

Playbooks is not a feature of Data or Viewer. Its public proposition is open analytical methods for using CharityGraph with the AI you already have.

```text
Playbook definition + parameters + CharityGraph references/context
    -> portable invocation -> user's chosen AI -> downstream analytical output
```

A Playbook definition is governed CharityGraph content. An invocation is a parameterised instance of a definition. External-model output is downstream user analysis and is not canonical CharityGraph knowledge merely because it used an official Playbook.

## Provider neutrality

No provider is required. ChatGPT, Claude, Gemini and Copilot may be mentioned as examples of user-selected environments, but this contract does not depend on any one provider.

## Governance

Shared product, editorial and governance authority remains in the canonical documents maintained by the sibling [CharityGraph Data repository](https://github.com/gregorycwhill/charitygraph-data), especially its [`PRODUCT.md`](https://github.com/gregorycwhill/charitygraph-data/blob/main/PRODUCT.md), [`PRINCIPLES.md`](https://github.com/gregorycwhill/charitygraph-data/blob/main/PRINCIPLES.md), [`DOCUMENT_AUTHORITY.md`](https://github.com/gregorycwhill/charitygraph-data/blob/main/DOCUMENT_AUTHORITY.md), [`PUBLIC_VNEXT_DECISION_LOG.md`](https://github.com/gregorycwhill/charitygraph-data/blob/main/PUBLIC_VNEXT_DECISION_LOG.md), [`AGENT_DATA_DISTRIBUTION_CONTRACT.md`](https://github.com/gregorycwhill/charitygraph-data/blob/main/AGENT_DATA_DISTRIBUTION_CONTRACT.md) and [`BRAND_AND_REUSE.md`](https://github.com/gregorycwhill/charitygraph-data/blob/main/BRAND_AND_REUSE.md).

This repository may refine Playbooks-specific rules but cannot override CharityGraph neutrality, evidence, privacy, contestability, brand or reuse policy. The repository is publicly available, but it has no production Playbook catalogue or release yet.

## Repository contents

- [`PLAYBOOK_CONTRACT.md`](PLAYBOOK_CONTRACT.md) — definition, invocation and output boundary;
- [`PLAYBOOK_BASE_POLICY.md`](PLAYBOOK_BASE_POLICY.md) — concise inherited epistemic rules;
- [`CONTRIBUTING.md`](CONTRIBUTING.md) — accessible contribution and status model;
- [`schema/playbook.schema.json`](schema/playbook.schema.json) — minimal definition schema; and
- [`examples/example-playbook.md`](examples/example-playbook.md) — one non-production contract example.

This repository intentionally contains no production catalogue, hosted chatbot, provider integration, API/MCP service or Viewer launch implementation.
