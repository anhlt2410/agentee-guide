---
description: What the agent can and can't do — and where the human stays in control.
---

# Agents & Capabilities

## What Agentee can do

* Create orders from a natural-language description
* Check inventory / stock levels and raise low-stock alerts
* Answer revenue and comparison queries (e.g. month-over-month)
* Prepare purchase orders, payment reminders, and follow-ups
* Mark orders delivered, update inventory, and generate invoices
* Create leads (including from a scanned image) and enrich them
* Draft and send outreach emails (with approval)

## The core boundary: AI prepares, humans decide

Agentee **drafts** actions; it does not fire them autonomously. For anything that
changes data or leaves the system (POs, emails, reminders), a user reviews and
approves first.

> AI prepares POs, payment reminders, or follow-ups. Users review and approve
> before anything is sent.

{% hint style="info" %}
This approval gate is the single most important thing to communicate to new
users: Agentee is fast, but it never sends or commits on your behalf without a
human confirming.
{% endhint %}

## What Agentee does not do

* It does not bypass ERP permissions — it can only act within the user's role and scope.
* It does not commit or send anything without an approval step.
* It does not migrate or restructure your existing ERP data.
