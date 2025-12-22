# Reasoning Component

This document defines the Reasoning component
of the Noema Protocol.

Reasoning is responsible for deciding what an agent
should do based on goals and context.

---

## Responsibility

The Reasoning component:

- evaluates goals and intent
- processes available context
- produces decisions or action intents

Reasoning does NOT:
- perform side effects
- modify external systems
- directly execute actions

This separation ensures predictable behavior
and easier inspection.

---

## Inputs

At the protocol level, reasoning may consume:

- agent goals
- current system state
- historical context from memory
- external signals or observations

Inputs must be explicitly provided.
Implicit or hidden state is discouraged.

---

## Outputs

Reasoning produces explicit outputs, such as:

- decisions
- action plans
- prioritized intents
- no-op (when no action is required)

Outputs must be structured and observable
by the execution component.

---

## Stateless vs Stateful Reasoning

Reasoning may be implemented as:

- **Stateless**  
  Decisions are made purely from provided inputs.

- **Stateful**  
  Intermediate reasoning state may exist,
  but must be externalized through memory
  if persistence is required.

Protocol compatibility does not depend
on internal reasoning mechanisms.

---

## Determinism

Reasoning should aim to be:

- understandable
- reproducible
- inspectable

Non-deterministic behavior is allowed,
but its effects should be observable
and traceable through memory and logs.

---

## Failure Handling

If reasoning cannot produce a valid decision:

- it may return a no-op
- it may emit an error or warning
- it must not trigger execution directly

Failure states should be recorded
for later inspection.

---

## Separation from Execution

Reasoning must remain isolated from execution.

This ensures:
- decisions can be reviewed
- actions can be controlled
- failures can be handled safely

Any coupling between reasoning and execution
violates protocol intent.

---

## Notes

This document defines expected behavior,
not specific algorithms.

Implementations may use different models,
heuristics, or rule systems,
as long as protocol boundaries are respected.
