---
icon: filter
description: Which records each user can see and act on.
---

# Data Access & Scoping

Access is scoped by role. Users only see and act on data appropriate to their
role, enforced through their ERP identity.

**Illustrative split**

| Role | Sees |
|------|------|
| CEO / Owner | Financials, company-wide stock, approvals |
| Employee | Their operational tasks (orders, deliveries, invoices) |
| Sales Rep | Their deals, leads, and outreach |

{% hint style="warning" %}
**TODO:** Specify record-level scoping rules (e.g. own-records-only vs
team-visibility) per role, and how scoping applies to enriched/external data.
{% endhint %}
