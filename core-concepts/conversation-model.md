---
description: How commands are issued and how Agentee responds across channels.
icon: comments
---

# Conversation Model

## Natural-language commands

Any Agentee function can be triggered by typing a natural-language command — no navigation, no memorizing function names.

> **As a Sales Rep or Sales Manager**, I want to trigger any Agentee functionality by typing a natural-language command in chat, so I can initiate actions quickly without navigating or remembering functionality names.

## Turns and confirmations

* A conversation is a series of turns (see [Context & Memory](context-and-memory.md)).
* Agentee replies with **structured confirmations**, not just prose — e.g. `Order #SO-000123 has been created…`.
* Some updates arrive as **notifications** (e.g. an employee is told when an order is delivered), separate from the user's own turns.
