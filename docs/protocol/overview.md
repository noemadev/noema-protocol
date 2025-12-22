# Protocol Overview

This document provides an overview of the Noema Protocol
from a protocol and specification perspective.

It describes the responsibilities, boundaries,
and interactions of core protocol components.

---

## Protocol Scope

Noema Protocol defines:

- conceptual interfaces between system components
- expected responsibilities of each component
- interaction patterns for autonomous agents

Noema Protocol does NOT define:

- concrete implementations
- specific models or algorithms
- deployment environments
- user-facing applications

---

## Protocol Components

At the protocol level, Noema consists of
the following components:

- Agent
- Reasoning
- Memory
- Execution
- Interfaces

Each component is defined by behavior
and responsibility, not by implementation.

---

## Agent

An agent is the primary unit of operation in Noema.

At the protocol level, an agent:

- maintains internal state
- coordinates reasoning, memory, and execution
- operates continuously or episodically

An agent is responsible for orchestrating
the overall decision and action loop.

---

## Reasoning Component

The reasoning component is responsible for
decision-making.

Protocol expectations:
- consumes goals and context
- produces decisions or intents
- does not perform side effects

Reasoning output must be explicit
and observable by the system.

---

## Memory Component

The memory component is responsible for
state persistence and contextual continuity.

Protocol expectations:
- stores structured state
- supports read and write operations
- provides historical context to reasoning

Memory must be accessible independently
of reasoning and execution.

---

## Execution Component

The execution component is responsible for
performing actions.

Protocol expectations:
- receives decisions from reasoning
- executes actions deterministically
- reports outcomes back to memory

Execution must be isolated from
decision-making logic.

---

## Interfaces

Interfaces connect Noema systems
to external environments.

Examples include:
- APIs
- services
- onchain systems
- offchain infrastructure

Interfaces are treated as replaceable
and loosely coupled components.

---

## Interaction Flow

At the protocol level, a typical interaction
follows this pattern:

1. Agent loads context from memory
2. Reasoning evaluates state and goals
3. Decisions are produced
4. Execution performs actions
5. Results are written back to memory

This loop defines the core operational
cycle of Noema agents.

---

## Compatibility

Implementations are considered compatible
if they respect:

- component boundaries
- interaction flow
- responsibility separation

Internal optimizations are allowed
as long as protocol expectations
are preserved.

---

## Notes

This overview defines protocol intent.

Detailed specifications for each component
are described in their respective documents.
