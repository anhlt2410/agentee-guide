---
icon: file-signature
description: A 5-stage, multi-role workflow for generating and approving proposals.
---

# Proposal Builder

## Goal

Take a deal from raw requirements to an approved, ready-to-send proposal, with
the right people validating each part.

## The 5 stages

1. **Requirement Analysis**
2. **Scope Confirmation**
3. **Technical Proposal**
4. **Cost Estimation**
5. **Finalization**

## Roles & responsibilities

| Role | Responsibility |
|------|----------------|
| **Sales Rep** | Owns the deal; triggers the proposal, confirms scope, and gives final approval before sending. |
| **Sales Manager** | Approves proposals that exceed the discount threshold; reviews the audit trail. |
| **Technical Consultant** | Internal expert; validates technical sections, selects architecture/stack, and reviews cost-estimation effort. Engaged **between scope confirmation and final generation**. |

## Flow with approval gates

```
Requirement Analysis
        │
Scope Confirmation ──(Sales Rep confirms)
        │
        ├─ Technical Consultant validates tech sections + picks stack
        │  and reviews cost-estimation effort
        │
Technical Proposal → Cost Estimation
        │
        ├─ Sales Manager approves IF discount > threshold
        │
Finalization ──(Sales Rep final approval)──► Send
```

{% hint style="info" %}
Every action here is logged; the Sales Manager can review the full audit trail.
See [Audit & Logging](../../admin/audit-and-logging.md).
{% endhint %}

{% hint style="warning" %}
**TODO:** Define the discount threshold value/source and the exact hand-off
mechanics to the Technical Consultant (notification? assignment?).
{% endhint %}
