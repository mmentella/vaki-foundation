# VAKI Foundation Specification

## 1. Purpose

This document defines the semantic relationship between the VAKI Foundation and VAKI manifestations.

It gives canonical meaning to the invariant:

```text
The Foundation defines.
Manifestations inherit, interpret, and implement.

A manifestation may extend the Foundation within its domain,
but it may not silently redefine it.
```

This is not a software specification, API specification, compliance framework, certification model, governance workflow, maturity model, repository template, machine-readable schema, versioning system, compatibility system, or development process.

Its purpose is narrower: to preserve shared meaning while allowing manifestations to remain locally autonomous.

## 2. What the Foundation Owns

The Foundation owns domain-independent meaning for the VAKI ecosystem.

Foundation ownership means semantic ownership. It defines the shared concepts, principles, and reasoning structures that manifestations use as common reference. It does not mean centralized operational control over how each manifestation is built, governed, deployed, operated, or represented.

The Foundation owns:

- invariant philosophy;
- durable cross-domain principles;
- canonical shared terminology;
- domain-independent reasoning structures;
- observation, evidence, uncertainty, decision, commitment, manifestation, sharing, and feedback semantics through their owning documents;
- the boundary between Foundation meaning and local manifestation realization.

The Foundation does not own domain-specific implementation choices. It does not prescribe tools, technologies, architectures, procedures, workflows, data structures, performance targets, deployment models, or local engineering decisions.

Foundation ownership exists to prevent semantic fragmentation, not to force uniformity.

## 3. What Manifestations Own

A manifestation is a concrete realization of VAKI ideas in a specific domain.

A manifestation may be software, hardware, research, a product, a machine, a vessel, a process, or another designed system. It may live in an independent repository and may choose the tools, technologies, languages, architectures, procedures, workflows, and local conventions appropriate to its domain.

Manifestations own domain-specific realization. This includes local design decisions, operational practices, implementation mechanisms, domain constraints, delivery processes, and the concrete behavior through which the manifestation interacts with reality.

Independence does not mean semantic isolation. A manifestation that claims alignment with VAKI Foundation uses Foundation meanings as shared reference. It may interpret, implement, and extend those meanings locally, but it should keep the difference between Foundation meaning and local meaning visible.

## 4. Inheritance of Foundation Meaning

Inheritance means that a manifestation treats relevant Foundation meanings as its shared semantic base.

It does not mean copying every Foundation document, adopting a common repository structure, using common tools, following a centralized workflow, or implementing a software-style inheritance model.

A manifestation inherits Foundation meaning when it accepts the relevant Foundation concepts, principles, and distinctions as the starting point for its own reasoning and design.

Inherited meaning remains Foundation meaning. A manifestation may use it, interpret it for its domain, and implement it through local practices, but it does not become free to silently replace that meaning with a different one.

Not every Foundation concept is equally relevant to every manifestation at every moment. Inheritance requires preserving the meanings that matter to the manifestation's domain, decisions, commitments, and claims of VAKI alignment. It does not require unnecessary duplication.

## 5. Domain Interpretation

Domain interpretation is the explicit way a manifestation understands Foundation meaning in its own domain.

Interpretation makes Foundation meaning usable under local conditions. It may explain domain assumptions, constraints, risks, vocabulary, examples, or boundaries that affect how a Foundation concept is applied in context.

Interpretation preserves the fundamental Foundation meaning. It does not replace the canonical meaning with a local one. A manifestation may say, in effect:

```text
This is how this Foundation concept is understood in this domain.
```

It should not imply:

```text
This local meaning is now the Foundation meaning.
```

In this document, interpretation refers to Foundation-to-domain interpretation. Evidential interpretation is owned by the [Evidence Model](thinking/EVIDENCE.md). Observation-side interpretation boundaries are owned by the [Observation Model](thinking/OBSERVATION_MODEL.md).

## 6. Domain Extension

A domain extension is a local addition made by a manifestation because its domain needs concepts, constraints, practices, or distinctions that the Foundation does not define.

An extension may be appropriate when a manifestation needs to name domain-specific structure, preserve local reasoning, expose a constraint, or make implementation-relevant knowledge understandable.

A domain extension:

- belongs initially to the manifestation;
- should remain distinguishable from Foundation meaning;
- does not automatically become Foundation knowledge;
- may generate feedback, evidence, and learning;
- may later be proposed for Foundation evolution through an explicit process outside the scope of this document.

An extension should not be presented as if it were already part of the Foundation. Local concepts can be valuable without being universal.

The test is not whether the extension is useful. The test is whether readers can tell where Foundation meaning ends and local domain meaning begins.

## 7. Implementation Freedom

Manifestations own implementation freedom.

They may choose local tools, technologies, languages, architectures, procedures, workflows, data structures, representations, performance targets, deployment models, operational practices, domain conventions, and engineering decisions.

This freedom does not require Foundation approval.

An implementation decision is not automatically a domain extension. Choosing a programming language, material, sensor, manufacturing process, data format, research method, operating procedure, or deployment model may be important locally without changing Foundation meaning.

Implementation freedom is bounded only by semantic honesty. A local implementation may differ radically from another manifestation while still preserving Foundation meaning. A local implementation may also appear compatible while silently redefining Foundation meaning. The difference is semantic clarity, not technical similarity.

## 8. Silent Redefinition Boundary

The boundary between interpretation, extension, implementation, explicit divergence, and silent redefinition is central to this specification.

| Concept | Meaning |
|---|---|
| Interpretation | Local explanation of Foundation meaning in a domain while preserving the canonical meaning. |
| Extension | Local addition that remains distinguishable from Foundation meaning. |
| Implementation decision | Local choice about how to build, operate, represent, or organize the manifestation. |
| Explicit divergence | A visible, named departure from inherited Foundation meaning, with reasoning or decision context. |
| Silent redefinition | A change to Foundation meaning that is presented or allowed to appear as if no change occurred. |

A manifestation may explicitly diverge from a Foundation concept or principle when its domain context requires it. That divergence may be temporary, bounded, experimental, or deliberate. The issue is not that divergence can never happen. The issue is that it must not be hidden.

A manifestation crosses into silent redefinition when it:

- changes the meaning of a Foundation concept without making the change visible;
- significantly narrows a Foundation meaning while presenting the narrower meaning as canonical;
- adds domain-specific meaning that can be confused with Foundation meaning;
- knowingly departs from an inherited principle or concept without naming the departure;
- relies on assumptions that materially change interpretation while leaving those assumptions invisible.

The required response is semantic transparency. The difference should be visible, explicit, named when appropriate, and traceable to reasoning or decision context.

This specification does not mandate one mechanism for doing that. A manifestation may use documentation, decision records, ADRs, declared assumptions, architecture notes, domain specifications, or another local representation. The canonical requirement is clarity of meaning, not uniformity of format.

## 9. Traceability Without Bureaucracy

Traceability exists so that shared meaning can remain inspectable without turning the Foundation into a control system.

A manifestation should be able to make conceptually visible:

- which Foundation meanings it inherited;
- how those meanings were interpreted where interpretation matters;
- which extensions are local to the manifestation;
- which important local decisions produced commitment;
- where known divergences or unresolved tensions exist.

This traceability is conceptual. It does not require a manifest file, registry, checklist, mandatory trace graph, identifier system, machine-readable metadata, or central validation process.

The Foundation defines the need for semantic clarity. Each manifestation chooses representations appropriate to its domain, risk, and consequence.

Traceability should be proportional. More important decisions, higher consequence commitments, stronger claims of Foundation alignment, and greater risk of semantic confusion require more preserved reasoning. Low-risk implementation detail should not be inflated into bureaucracy.

When Foundation state matters to later understanding, a manifestation should be able to identify sufficiently which Foundation state informed its interpretations and decisions. This document does not define semantic versioning, migration rules, compatibility guarantees, support policy, or a version registry.

## 10. Feedback and Foundation Learning

The relationship between Foundation and manifestation is not one-way.

A manifestation operates in reality. It produces outcomes, receives feedback, creates observations, may generate evidence, and may produce learning.

The conceptual flow is:

```text
Manifestation
  -> outcomes
  -> feedback
  -> Observation
  -> Evidence
  -> learning
  -> possible deliberate Foundation evolution
```

Feedback from a manifestation does not automatically modify the Foundation.

Foundation evolution should be explicit, deliberate, and reviewed. A manifestation may discover a broadly reusable principle, method, distinction, or boundary, but that discovery remains manifestation knowledge until it is intentionally promoted into Foundation knowledge through a process outside the scope of this document.

This protects both sides of the relationship. Manifestations can experiment and learn locally without destabilizing the Foundation, and the Foundation can evolve from real-world learning without absorbing every local practice.

## 11. Non-Goals

This document does not define:

- compliance;
- certification;
- maturity models;
- scoring;
- registries;
- repository templates;
- machine-readable metadata;
- CI validation;
- policy engines;
- plugin architecture;
- repository structure;
- engineering process;
- product lifecycle;
- contribution governance;
- Foundation versioning system;
- migration rules;
- compatibility framework;
- approval workflows;
- local ADR process;
- implementation architecture.

These may exist inside a manifestation when locally useful, but they are not created by this specification.

## 12. Relationship to Existing Foundation Documents

This document connects existing Foundation documents without replacing their ownership.

[VAKI Principles](philosophy/PRINCIPLES.md) owns durable cross-domain principles. This specification clarifies how manifestations inherit, interpret, implement, and extend those principles without silently redefining them.

[VAKI Glossary](GLOSSARY.md) owns canonical shared terminology. This specification uses glossary meanings and defines the Foundation-to-manifestation relationship around them.

[VAKI Thinking Model](thinking/README.md) describes the general topology of knowledge construction, including manifestation, sharing, feedback, and recursive learning. This specification clarifies how that topology relates to Foundation meaning and manifestation autonomy.

[VAKI Observation Model](thinking/OBSERVATION_MODEL.md) owns observation semantics. This specification references observation only as part of the manifestation feedback and learning flow.

[Evidence Model](thinking/EVIDENCE.md) owns evidence, evidential relationships, interpretation of evidential relevance, body of evidence, and uncertainty semantics. This specification does not redefine those concepts.

[Decision Model](method/DECISION_MODEL.md) owns decision reasoning, decision semantics, commitment, reversibility, optionality, and decision traceability. This specification references decisions and commitments only to explain how local reasoning becomes manifestation behavior.

[VAKI Design Methodology](method/DESIGN_METHODOLOGY.md) owns domain-independent methodological guidance. This specification clarifies the boundary between that guidance and local manifestation implementation.

[ADR-0001: Foundation-Manifestation Boundary](../decisions/ADR-0001-foundation-manifestation-boundary.md) establishes the architectural boundary. This specification makes the semantic relationship canonical for M1.3 while preserving ADR-0001 as the accepted architectural decision.
