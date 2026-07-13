---
description: Role-based scoping, action logging, and reliable performance across channels.
---

# Roles & Permissions

> **As an Admin**, I want the system to enforce role-based data scoping, log
> every agent action triggered from chat, and maintain responsive performance
> across all channels, so the platform is secure, auditable, and reliable in
> daily use.

## Roles

| Role | Scope |
|------|-------|
| CEO / Owner | Revenue, stock alerts, PO approvals |
| Employee | Order/delivery/inventory operations, invoices |
| Sales Rep | Owns deals; proposals, leads, outreach |
| Sales Manager | Above-threshold approvals; audit-trail review |
| Technical Consultant | Technical validation, stack selection |
| System Admin | Workflow definition, roles, scoping |

## Three admin guarantees

1. **Role-based data scoping** — users see and act only within their role. See [Data Access & Scoping](data-access-scoping.md).
2. **Action logging** — every chat-triggered action is recorded. See [Audit & Logging](audit-and-logging.md).
3. **Responsive performance** — consistent across Web UI and Telegram.

{% hint style="info" %}
Roles derive from ERP identity via SSO, so Agentee inherits ERP permissions
rather than defining a parallel system.
{% endhint %}

{% hint style="warning" %}
**TODO:** Add the full role × action permission matrix.
{% endhint %}
