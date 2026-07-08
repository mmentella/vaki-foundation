# VAKI Design Methodology

VAKI treats design as an iterative process for reducing uncertainty and transforming knowledge into systems that increase autonomy.

The methodology is domain-independent. It does not prescribe a programming language, CAD tool, project-management framework, research technique, manufacturing process, or deployment model.

Its purpose is to preserve the reasoning structure beneath those choices.

## 1. Start from intent

State why the system should exist and whose autonomy it should improve.

Clarify the desired change in capability before defining the artifact.

A product, service, machine, experiment, or software system is a means. The intended increase in capability is the purpose.

## 2. Frame the problem

Describe the problem in terms of reality, actors, constraints, current limitations, and consequences.

Separate the problem from the first proposed solution.

A useful problem frame makes visible:

- the current state;
- the desired state;
- the people or systems affected;
- hard constraints;
- important uncertainties;
- assumptions already being made;
- evidence currently available.

## 3. Observe before abstracting

Collect observations from the real system or environment.

Distinguish direct observations from interpretations and hypotheses.

Where possible, create observability before optimizing behavior.

## 4. Build an explicit model

Create the simplest useful model of the system that explains the relevant structure and supports decisions.

A model may be conceptual, mathematical, physical, computational, procedural, or a combination of these.

Every model is partial. Its scope and limitations should be explicit.

## 5. Form hypotheses

Translate uncertainty into testable statements.

A useful hypothesis should identify:

- what is expected;
- under which conditions;
- what evidence supports it;
- what evidence would weaken or invalidate it;
- what decision depends on the result.

## 6. Design experiments for learning

Choose the smallest credible experiment that can reduce the uncertainty relevant to the next decision.

Experiments should avoid unnecessary scope. Prefer learning value over premature completeness.

A prototype is successful when it answers its question, even when the answer invalidates the original idea.

## 7. Interpret evidence in context

Do not confuse measurements, proxies, local metrics, or intermediate performance with final system success.

Evaluate evidence against the actual objective, relevant constraints, and operating environment.

Preserve uncertainty where the evidence does not justify certainty.

## 8. Decide explicitly

Important decisions should make visible:

- context;
- options considered;
- assumptions;
- evidence;
- constraints;
- trade-offs;
- expected consequences;
- conditions that could trigger reconsideration.

The purpose is not bureaucracy. It is to avoid losing the reasoning that made the decision intelligible.

## 9. Build the smallest coherent manifestation

Transform the current model and decisions into a concrete system capable of interacting with reality.

The manifestation should be coherent enough to produce meaningful feedback, but no larger than required by the current evidence.

Avoid adding complexity whose need has not yet been demonstrated.

## 10. Operate, observe, and learn

Real operation is part of design.

Observe how the manifestation behaves, where assumptions fail, which constraints dominate, and what new questions emerge.

Operational knowledge should return to the knowledge base rather than remaining only in individual memory.

## 11. Evolve or retire

Systems should change when evidence, context, objectives, or constraints change.

Evolution is not failure of the original design. Refusing to update a system after reality changes is the failure.

When a manifestation no longer serves its purpose, retirement is a valid design outcome.

## Methodological loop

The methodology is iterative rather than linear:

```text
Intent
  ↓
Problem Framing
  ↓
Observation
  ↓
Model
  ↓
Hypothesis
  ↓
Experiment
  ↓
Evidence
  ↓
Decision
  ↓
Manifestation
  ↓
Operation and Feedback
  └──────────────→ Observation / Framing / Model
```

The loop may move backward whenever evidence requires it.

VAKI does not reward progress through stages. It rewards improved understanding, better decisions, and greater autonomy.