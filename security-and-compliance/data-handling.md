---
icon: database
description: What data Agentee touches, where it goes, and how it's retained.
---

# Data Handling

## Your ERP data stays put

Agentee connects to your existing ERP through APIs. Legacy data remains
untouched and **no migration is required** — Agentee reads and writes through
the API rather than copying your database.

## Data that leaves your system

Two flows send data to third parties and must be understood before enabling:

| Flow | Data shared | Destination |
|------|-------------|-------------|
| Enrichment | Lead/company identifiers | Apollo.io |
| Outreach | Email content + recipient | Gmail (rep's account, via OAuth) |

{% hint style="warning" %}
**TODO:** Specify what payload is sent to the LLM provider, what (if anything) is
retained, and retention windows for logs, drafts, and enriched data.
{% endhint %}
