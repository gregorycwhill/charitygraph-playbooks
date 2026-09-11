# Playbooks repository development and review checks

**Status:** Reference — repository reproducibility instructions  
**Date:** 11 September 2026

The Playbooks repository currently contains the product contract, base policy,
contribution guidance, JSON Schema and one non-production example. It has no
provider integration, hosted inference service, production catalogue or build
system.

From a clean clone, inspect the contract and validate the example against
`schema/playbook.schema.json` with any standard JSON Schema validator available
to the reviewer. Check Markdown links and run `git diff --check`.

No credentials, private runtime material or CharityGraph source archive is
required for these checks. External-model output is not a repository fixture or
canonical CharityGraph knowledge.
