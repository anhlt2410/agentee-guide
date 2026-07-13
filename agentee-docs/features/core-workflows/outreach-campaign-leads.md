---
description: >-
  Auto-enrich leads via Apollo.io, de-duplicate against CRM, and send outreach
  from the rep's own Gmail.
---

# Outreach Campaign Leads

## Goal

Give sales reps complete, current contact and company data automatically, then
let them reach out from their real inbox — no manual research, no manual entry.

> **As a Sales Agent**, I want to automatically enrich a newly created lead or
> company record using **Apollo.io** as the default enrichment provider, so reps
> always have complete, up-to-date data without manual research.

## Enrichment

Apollo.io is the **default enrichment provider**. Enrichment runs on newly
created lead or company records.

## Duplicate check

{% hint style="danger" %}
**Pre-condition:** Before any enrichment call, the agent **must** perform a
duplicate check against existing CRM records.
{% endhint %}

Match rules, in priority order:

| Priority | Match rule |
|:--------:|------------|
| 1 | `email` — exact match |
| 2 | `company domain` + `full name` — both must match |
| 3 | `company domain` only — applies to company-level records |

If a match is found, the agent should resolve to the existing record rather than
creating or enriching a duplicate.

## Sending outreach via Gmail

> I want to connect my Gmail account and have the agent send outreach emails
> directly from it, so emails land in prospects' inboxes from my real address,
> with high deliverability, and I can track when they've been sent or replied to.

* Connect Gmail via OAuth.
* Emails send from the rep's **real address** (better deliverability).
* Agentee tracks **sent** and **replied** status.

{% hint style="info" %}
Sending is a write action — outreach is drafted for the rep to approve before it
goes out. See [Agents & Capabilities](../../core-concepts/agents-and-capabilities.md).
{% endhint %}

{% hint style="warning" %}
**TODO:** Document Apollo.io API scopes/rate limits/cost and Gmail OAuth scopes.
These flows send data to third parties — cross-link
[Privacy](../../security/privacy.md) and [Data Handling](../../security/data-handling.md).
{% endhint %}
