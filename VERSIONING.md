# Versioning

This document defines how Noema Protocol versions are managed.

Noema Protocol follows a documentation-first and
specification-driven versioning approach.

---

## Version Format

Noema Protocol uses Semantic Versioning:


---

## Beta Versions (0.y.z)

During the beta phase:

- The protocol version is `0.y.z`
- Breaking changes are allowed
- Interfaces may change without backward compatibility
- Changes must be documented in the changelog
- Significant changes should be proposed via RFC

Beta versions prioritize iteration and architectural clarity.

---

## Stable Versions (1.0.0 and above)

Once the protocol reaches stability:

- Breaking changes require a MAJOR version bump
- MINOR versions add backward-compatible improvements
- PATCH versions fix documentation or specification errors
- Stability guarantees apply only to published stable versions

---

## RFC and Versioning

- Major or breaking changes must be proposed through an RFC
- Accepted RFCs define the scope of version changes
- Version bumps reflect the aggregated outcome of RFCs

---

## Specification Snapshots

Each released version represents a snapshot of the protocol
specification at a given point in time.

Implementations are expected to target a specific
protocol version explicitly.

---

## Notes

Version numbers describe the protocol specification,
not implementation maturity.

Stability is defined by specification guarantees,
not by release frequency.
