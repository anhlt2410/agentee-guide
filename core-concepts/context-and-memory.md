---
description: How Agentee remembers within a session — and forgets between them.
icon: brain
---

# Context & Memory

## Session-scoped memory

Within a single session, Agentee remembers what you've mentioned so you can hold a natural multi-turn conversation without repeating yourself.

> **As a Sales Rep**, I want the agent to remember what I've mentioned during a session so I can have natural multi-turn conversations.

**Example**

> **Rep:** Create a lead for Acme Corp. **Rep:** Now enrich it and draft an intro email. _(“it” resolves to Acme from the previous turn.)_

## Clean slate per session

Each **new session starts clean**. Agentee does not carry context across sessions, which prevents it from acting on stale information.

> ...while ensuring each new session starts clean to prevent actions based on stale context.

{% hint style="info" %}
Rule of thumb: context lives as long as the conversation does. Start a new session whenever you want a guaranteed fresh state.
{% endhint %}
