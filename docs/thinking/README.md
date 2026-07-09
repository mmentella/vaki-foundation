# VAKI Thinking Model

VAKI treats thinking as an explicit, iterative process for moving from incomplete reality to better decisions and more capable systems.

The model is not a rigid workflow. It is a reasoning topology: a shared structure for observation, framing, modeling, hypothesis formation, experimentation, evidence interpretation, decision, manifestation, sharing, and feedback.

Hypothesis and Experiment semantics are defined in the [Hypothesis and Experiment Model](HYPOTHESIS_AND_EXPERIMENT_MODEL.md). Hypothesis formation and Experiment may participate in Inquiry, but neither is a mandatory stage. Inquiry may proceed without either, and the topology remains recursive rather than a required sequence.

## Core loop

```text
Reality
  ↓ observe
Observations
  ↓ frame
Problem
  ↓ model
Model
  ↓ may inform
Hypotheses
  ↓ may guide
Experiments
  ↓ may create conditions for
Observations
  ↓ may bear as
Evidence
  ↓ interpret
Decisions
  ↓ instantiate
Manifestation
  ↓ make understandable and transferable
Share
  ↓ operate, use, review, adapt
Feedback
  └──────────────→ new Observations
```

The loop is recursive. Evidence may invalidate framing, models, hypotheses, or decisions. Operation may reveal that the original problem was framed incorrectly. A manifestation may create new capabilities and therefore new intents.

VAKI does not optimize for moving forward through stages. It optimizes for reducing important uncertainty, improving the quality of decisions, and making knowledge reusable beyond the original builder.

Questions and Inquiry are defined in the [Questions and Inquiry Model](QUESTIONS_AND_INQUIRY_MODEL.md). Questions may arise before, within, or after problem framing, and Inquiry may interact recursively with observation, modeling, hypothesis formation, experiment, evidence, decision, and feedback. Inquiry is not an additional required stage in this loop; it refines how VAKI understands question-oriented movement within the broader thinking topology.

## 1. Reality

Reality is the external reference that constrains VAKI reasoning.

Models, plans, simulations, metrics, and narratives are representations. They are useful only while they remain sufficiently aligned with the relevant part of reality.

When evidence conflicts with a model, the model is provisional; reality is not.

## 2. Observation

Observation records what is perceived, measured, or experienced before adding stronger interpretive claims.

The detailed semantics of observation are defined in [Observation Model](OBSERVATION_MODEL.md).

A good observation states:

- what was observed;
- under which conditions;
- through which instrument or process;
- with what known uncertainty or incompleteness;
- at what time or system state.

Observation is not yet explanation.

## 3. Problem Framing

Problem framing identifies the decision-relevant structure of the situation.

A useful frame makes visible:

- current state;
- desired state;
- actors;
- constraints;
- consequences;
- uncertainties;
- assumptions;
- evidence already available.

A frame is itself a hypothesis about what matters. It must remain revisable.

## 4. Modeling

A model is a purposeful simplification used to explain, predict, design, or decide.

The objective is not maximal detail. The objective is sufficient structure for the decision at hand.

A useful model makes explicit:

- scope;
- variables or elements;
- relationships;
- assumptions;
- known omissions;
- intended use;
- conditions under which it may fail.

## 5. Hypothesis

A hypothesis is a provisional and challengeable claim that may arise within Inquiry or other reasoning.

A useful hypothesis states:

- what is expected;
- under which conditions;
- why it is plausible;
- what observation could become relevant to supporting it;
- what observation could become relevant to weakening or invalidating it;
- which decision, if any, may depend on its current evidential status.

Hypotheses exist to expose reasoning to reality.

Detailed Hypothesis semantics are owned by the [Hypothesis and Experiment Model](HYPOTHESIS_AND_EXPERIMENT_MODEL.md).

## 6. Experiment

An experiment is a deliberate reality-facing inquiry arrangement or intervention whose semantics are owned by the [Hypothesis and Experiment Model](HYPOTHESIS_AND_EXPERIMENT_MODEL.md).

The best experiment is not necessarily the largest or most realistic one. It is the smallest credible inquiry arrangement that can improve relevant understanding.

An experiment may weaken, qualify, or invalidate the preferred idea, but an experiment result is not automatically evidence.

Learning value takes precedence over confirmation value.

## 7. Evidence

Evidence is not synonymous with data.

A measurement becomes evidence only relative to a claim, model, hypothesis, or decision.

VAKI distinguishes:

```text
data
≠ observation
≠ signal
≠ evidence
≠ knowledge
≠ decision
```

These layers may be connected, but none should be silently substituted for another.

## 8. Interpretation

Evidence requires interpretation in context.

Interpretation should consider:

- measurement quality;
- alternative explanations;
- confounding factors;
- scope of applicability;
- cost of error;
- whether the evidence concerns a proxy or the actual objective;
- whether results survive relevant operating constraints.

A strong local result is not automatically system-level success.

## 9. Decision

A decision is a commitment of resources, direction, or constraints based on the current state of knowledge.

Important decisions should preserve:

- context;
- options considered;
- assumptions;
- evidence;
- uncertainties;
- trade-offs;
- expected consequences;
- conditions for reconsideration.

The purpose is not process overhead. It is to preserve the reasoning needed for later understanding and revision.

## 10. Manifestation

A manifestation is the concrete form through which VAKI reasoning interacts with reality.

It may be software, hardware, research, a machine, a vessel, a process, or another designed system.

A manifestation should be coherent enough to produce meaningful feedback and no more complex than current evidence justifies.

A manifestation is not complete merely because it works locally. It must also be made sufficiently understandable for others to inspect, use, adapt, maintain, or challenge.

## 11. Share

Share is the act of making a manifestation and its relevant knowledge understandable, inspectable, and transferable.

A VAKI project does not end when it works. It reaches a higher level of completion when someone else can understand it.

Sharing may include:

- explaining intent and problem framing;
- preserving assumptions and constraints;
- documenting decisions and trade-offs;
- exposing source, design materials, or operating instructions;
- explaining how to reproduce, operate, maintain, repair, adapt, or evaluate the manifestation;
- preserving known limitations and negative knowledge.

Share is not marketing. It is the autonomy-preserving step that prevents knowledge from remaining trapped in the original builder, tool, or context.

Without Share, feedback is weak because others cannot inspect the reasoning or interact with the manifestation meaningfully.

## 12. Operation and Feedback

Operation is part of design.

A shared manifestation enters reality, where assumptions encounter conditions that models may not have captured and where other people can use, inspect, adapt, and challenge it.

Feedback should be converted into observations, not merely reactions.

The system should ask:

- What changed?
- Which assumption was wrong or incomplete?
- Which constraint dominates in practice?
- Which metric was misleading?
- Which new capability or failure mode appeared?
- Which part of the model should be revised?
- What did sharing make easier or harder to understand, reuse, maintain, or adapt?

## Movement through the model

The model allows both forward and backward movement.

Typical backward transitions include:

```text
Evidence → Hypothesis
Evidence → Model
Decision → Problem Framing
Manifestation → Model
Share → Manifestation
Share → Decision
Feedback → Observation
Feedback → Problem Framing
```

Backward movement is not failure. Refusing to revise an invalidated layer is failure.

## Invariants

Across all VAKI manifestations:

1. Observation must be distinguishable from interpretation.
2. Assumptions must be made visible when they affect important decisions.
3. Hypotheses must be vulnerable to evidence.
4. Experiments must remain distinguishable from Observation and Evidence.
5. Evidence must be interpreted in context.
6. Proxy success must not be silently treated as objective success.
7. Important decisions must preserve enough reasoning to be revisited.
8. Manifestations must be shared enough to become understandable, inspectable, and transferable.
9. Operation must feed learning back into the system.
10. Negative knowledge must be preserved when it prevents repeated failure.
11. The objective is not activity. The objective is better understanding, better decisions, and greater autonomy.

## Relationship to the Design Methodology

The Design Methodology describes how VAKI transforms intent into evolving systems.

The Thinking Model describes the reasoning structure operating inside that process.

The two are complementary:

```text
Design Methodology = system evolution structure
Thinking Model      = reasoning structure within that evolution
```

Together they form the initial operating model of VAKI Foundation M1.
