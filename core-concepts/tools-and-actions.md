---
description: The concrete read and write actions Agentee can perform against your ERP.
icon: screwdriver-wrench
---

# Tools & Actions

Agentee's capabilities map to a defined set of ERP actions, split into **read** (no approval needed) and **write** (approval gate applies).

## Read actions

| Action            | Example                                |
| ----------------- | -------------------------------------- |
| Revenue query     | "This month: VND 2.4 billion, up 18%." |
| Sale report check | "Sales report for this month"          |
| Get deal list     | "Get deal list for this month"         |

## Write actions (require approval)

| Action               | Notes                                          |
| -------------------- | ---------------------------------------------- |
| Create lead          | Create lead from this business card            |
| Mark order delivered | Updates fulfilment status                      |
| Update inventory     | Adjusts stock after fulfilment                 |
| Generate invoice     | Produces invoice once order completes          |
| Prepare PO           | Drafted for approval; not sent until confirmed |

## Modules exposed

CRM · Account · HRM · Chat

## External connectors

| Connector   | Used for                                     | Detail                                                                                          |
| ----------- | -------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| Image / OCR | Lead creation from a photo                   | See [Lead Creation](../features-and-guides/core-workflows/lead-creation.md)                     |
| Apollo.io   | Lead/company enrichment                      | See [Outreach Campaign Leads](../features-and-guides/core-workflows/outreach-campaign-leads.md) |
| Gmail       | Sending outreach from the rep's real address | OAuth; tracks sent/replied                                                                      |
