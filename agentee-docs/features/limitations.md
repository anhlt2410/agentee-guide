---
description: What Agentee can't do yet, and how to work around it.
---

# Limitations & Known Issues

## The fallback principle

Agentee is an interface over your ERP, not a replacement for it. When the AI
misinterprets a request, the traditional ERP is always available.

> If the AI misunderstands a request, users can always open the traditional ERP
> interface to check or edit data directly.

## Known limitations

* No cross-session memory by design — see [Context & Memory](../core-concepts/context-and-memory.md).
* Write actions always require human approval; there is no fully autonomous mode.

{% hint style="warning" %}
**TODO:** Fill in concrete known issues (unsupported query types, channel
feature gaps between Web and Telegram, enrichment coverage limits, etc.).
{% endhint %}
