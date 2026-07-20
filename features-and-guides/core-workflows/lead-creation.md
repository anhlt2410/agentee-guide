---
description: Create a CRM lead by scanning an image or photo.
icon: user-plus
---

# Lead Creation

## Goal

Turn a photo (business card, form, sign-up sheet) into a structured CRM lead without manual data entry.

## How it works

1. The user sends or scans an **image/photo** in chat, or simply send lead information in texts.
2. Agentee extracts contact and company fields (OCR → structured lead).
3. The draft lead is shown for review before it's saved.

{% hint style="info" %}
Newly created leads can be automatically enriched and de-duplicated. The duplicate-check logic lives in [Outreach Campaign Leads](outreach-campaign-leads.md#duplicate-check) — Lead Creation reuses it, so the same record is never created twice.
{% endhint %}

### Sample lead information

For example:

* **Name**
* **Company**
* **Title**
* **Contact info** — email, LinkedIn, and similar details
* **Phone**
