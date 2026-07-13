---
icon: diagram-project
description: >-
  Admins define a workflow and import it so Agentee understands and executes it.
---

# Dynamic Workflow Definition

Agentee's behavior is driven by workflows that a **System Admin** defines and
imports. This lets you tailor what Agentee understands and how it acts, without
code changes.

> **As a System Admin**, I want to manually define the workflow myself then
> import it into the system, so Agentee can understand the workflow I want it to
> implement and act accordingly.

## How it works

1. Admin authors a workflow definition (stages, roles, actions, approval gates).
2. Admin imports the definition into Agentee.
3. Agentee interprets natural-language requests against the defined workflow and executes the mapped actions.

See [Proposal Builder](core-workflows/proposal-builder.md) for a fully worked
example of a multi-stage, multi-role workflow.

{% hint style="danger" %}
**TODO — blocking:** This page needs the actual **import format**. Provide:
* The file format (Markdown? YAML? JSON?)
* The schema / field reference (stage, role, action, approval-gate, threshold…)
* A complete, valid example file
* Validation rules and error handling on import

Everything above the fold is the "what"; this schema is the "how" and can't be
drafted without the spec.
{% endhint %}
