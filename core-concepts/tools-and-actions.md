---
icon: screwdriver-wrench
description: The concrete read and write actions Agentee can perform against your ERP.
---

# Tools & Actions

Agentee's capabilities map to a defined set of ERP actions, split into
**read** (no approval needed) and **write** (approval gate applies).

## Read actions

| Action | Example |
|--------|---------|
| Revenue query | "This month: VND 2.4 billion, up 18%." |
| Stock level check | "SKU-029 has 3 days of stock remaining." |
| Order status lookup | "Order #1042 has been delivered." |

## Write actions (require approval)

| Action | Notes |
|--------|-------|
| Create order | Returns a structured order confirmation (e.g. #SO-000123) |
| Mark order delivered | Updates fulfilment status |
| Update inventory | Adjusts stock after fulfilment |
| Generate invoice | Produces invoice once order completes |
| Prepare PO | Drafted for approval; not sent until confirmed |

## Modules exposed

CRM · Account · Inventory · HRM · Chat

## External connectors

| Connector | Used for | Detail |
|-----------|----------|--------|
| Image / OCR | Lead creation from a photo | See [Lead Creation](../features/core-workflows/lead-creation.md) |
| Apollo.io | Lead/company enrichment | See [Outreach Campaign Leads](../features/core-workflows/outreach-campaign-leads.md) |
| Gmail | Sending outreach from the rep's real address | OAuth; tracks sent/replied |

{% hint style="warning" %}
**TODO:** Confirm the full action list and exact response payload shapes per action.
{% endhint %}
