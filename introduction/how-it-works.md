---
icon: gears
description: The architecture behind the chat — natural language in, ERP actions out.
---

# How it works

Agentee sits between the user and your ERP. The user sends a natural-language
message; Agentee interprets intent, calls the right ERP action through an API,
and returns a structured confirmation.

## Traditional ERP vs Agentee

| | Traditional ERP | Agentee |
|---|---|---|
| Interaction | Menu → Form → Click | Type a message |
| Effort | ~6 screens to create one order | 1 message |
| Result | Manual data entry | AI records it in the correct module |

**Example**

> **User:** Create an order for 50 iced milk coffees for the Q1 store, delivery tomorrow at 8:00 AM
>
> **Agentee:** Order #SO-000123 has been created for 50 iced milk coffees. Delivery: 8:00 AM tomorrow.

## Where the data lives

Agentee does not replace your data layer. It connects to the existing ERP
through APIs, so legacy data stays intact and **no migration is required**.

> The data is still there — but now people can simply talk to it.

## Deployment options

Agentee supports two deployment models:

| | Option A — Full Agentee | Option B — Keep your ERP + add Chat |
|---|---|---|
| What it is | Complete ERP with a built-in chat interface | Agentee Chat connects to your current ERP via API |
| Best for | New setup or replacing an existing system | Preserving existing ERP investment |
| Modules / support | CRM, Account, Inventory, HRM, Chat | Works with SAP, Odoo, MISA, and others |

{% hint style="info" %}
If the AI misunderstands a request, users can always open the traditional ERP
interface to check or edit data directly.
{% endhint %}

## Request lifecycle (high level)

1. User sends a message (Web UI or Telegram).
2. Agentee interprets intent against the defined workflows.
3. Agentee calls the relevant ERP action(s) via API.
4. For actions that change data or send communications, Agentee **prepares** the action and waits for human approval.
5. Agentee returns a structured confirmation and logs the action.

{% hint style="warning" %}
**TODO:** Add an architecture diagram (LLM ↔ workflow engine ↔ ERP API ↔ external connectors) once finalized.
{% endhint %}
