# Core Concepts

This document explains the core concepts of Noema Protocol
in simple and practical terms.

Noema is built around the idea that intelligence should
operate as a structured system, not a single response.

---

## Intelligence as a System

In Noema, intelligence is not defined by a model
or a single algorithm.

It is defined by how different components work together
to produce consistent behavior over time.

This system-based approach makes AI easier to control,
understand, and extend.

---

## Agents

An agent in Noema is an entity that can:

- evaluate context
- make decisions
- perform actions
- persist state over time

Agents are long-lived system components,
not one-off request handlers.

---

## Reasoning

Reasoning is the process of deciding what to do.

It takes into account:
- goals
- current state
- available information

Reasoning produces intent and decisions,
but does not execute actions directly.

This separation keeps behavior predictable
and easier to inspect.

---

## Memory

Memory provides continuity.

It allows agents to:
- remember past actions
- store state and context
- reuse information across executions

Memory is not limited to conversation history.
It represents structured, persistent knowledge
about the system and its environment.

---

## Execution

Execution is the act of doing work.

It includes:
- triggering workflows
- calling external systems
- performing side effects

Execution follows decisions produced by reasoning
and records outcomes back into memory.

---

## Separation of Concerns

Noema enforces a clear separation between:

- thinking (reasoning)
- remembering (memory)
- doing (execution)

This separation improves reliability,
debuggability, and system safety.

---

## Autonomy

Autonomy in Noema means that agents can:

- operate without constant user input
- maintain internal state
- adapt behavior based on outcomes

Autonomy is achieved through architecture,
not through more complex prompts.

---

## Determinism and Control

Noema prioritizes explicit behavior.

Agents should behave in ways that are:
- understandable
- inspectable
- reproducible

This makes AI suitable for real systems
where predictability matters.

---

## Notes

These concepts define how Noema systems
should be structured.

Specific implementations may vary,
as long as these conceptual boundaries
are respected.
