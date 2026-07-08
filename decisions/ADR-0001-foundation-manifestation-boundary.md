# ADR-0001: Foundation–Manifestation Boundary

- Status: Accepted
- Milestone: M1
- Decision scope: VAKI ecosystem architecture

## Context

VAKI is intended to support multiple independent manifestations across different domains. A manifestation may be software, hardware, research, a machine, a vessel, a process, or another designed system.

Without an explicit boundary, the Foundation risks becoming either too abstract to guide real work or too prescriptive to remain domain-independent. The opposite risk also exists: manifestations may silently redefine shared concepts and fragment the ecosystem.

M0 established a philosophical and methodological core. M1 requires an operational boundary that preserves coherence while allowing local freedom.

## Decision

VAKI Foundation owns only domain-independent invariants:

- philosophy;
- shared principles;
- shared terminology;
- domain-independent reasoning structures;
- evidence and decision semantics;
- lifecycle semantics;
- conformance rules required to claim alignment with VAKI Foundation.

Manifestations own domain-specific realization:

- implementation architecture;
- technology choices;
- tools and languages;
- physical design choices;
- domain-specific methods;
- operational procedures;
- performance targets;
- local governance and delivery processes.

The relationship is asymmetric:

> The Foundation defines shared meaning. Manifestations interpret and implement that meaning in context.

A manifestation may extend Foundation concepts locally, but must not silently redefine them.

Where a manifestation discovers a broadly reusable principle or method, it may propose that knowledge for promotion into the Foundation. Promotion is explicit and reviewed; it is never automatic.

## Consequences

### Positive

- The Foundation can remain small and durable.
- Manifestations can evolve independently.
- Different domains can choose appropriate tools without forced uniformity.
- Shared terminology remains stable enough for cross-domain learning.
- Domain discoveries can flow back into the Foundation through deliberate promotion.

### Negative

- Some duplication between manifestations is acceptable.
- Conformance requires judgment rather than mechanical identity.
- Boundary disputes may require explicit ADRs.
- The Foundation must resist the temptation to absorb implementation detail.

## Boundary test

Before adding a concept to the Foundation, ask:

1. Does this concept remain meaningful across materially different domains?
2. Can it guide reasoning or system evolution without prescribing a specific implementation?
3. Would removing the concept create semantic fragmentation across manifestations?
4. Is the concept mature enough to survive abstraction from the manifestation that produced it?

A concept should generally remain in a manifestation if the answer to the first two questions is no.

## Knowledge flow

The intended flow is bidirectional:

```text
Foundation
    ↓ defines invariants
Manifestation
    ↓ interacts with reality
Evidence and learning
    ↓ abstraction review
Foundation evolution
```

The Foundation is therefore stable, but not static.

## Non-goals

This ADR does not define:

- repository templates;
- mandatory programming languages;
- CI/CD standards;
- CAD conventions;
- trading methodologies;
- AI agent architecture;
- project-management frameworks;
- deployment platforms.

Those belong to manifestations unless future evidence demonstrates a truly domain-independent invariant.