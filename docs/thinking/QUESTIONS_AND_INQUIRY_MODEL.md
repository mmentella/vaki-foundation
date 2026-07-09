# VAKI Questions and Inquiry Model

## 1. Purpose

This document defines how VAKI understands questions and inquiry as domain-independent reasoning structures.

Its purpose is to preserve the meaning of a Question as distinct from uncertainty, problem framing, hypothesis, evidence, experiment, and decision. It also defines Inquiry as the directed and revisable pursuit of better understanding in relation to one or more Questions.

This model is not a research workflow, lifecycle, state machine, project-management method, question backlog, knowledge-management system, approval process, schema, database model, graph model, API, or tooling specification.

The model owns:

- Question;
- Inquiry;
- Inquiry Context;
- Question emergence;
- Question evolution;
- bounded Answer semantics;
- Question Resolution;
- Question Suspension;
- Question Reopening;
- Recursive Inquiry;
- Question Quality;
- Inquiry Traceability.

It does not prescribe how manifestations must record, prioritize, assign, review, store, or manage questions. Manifestations may create local research practices, issue trackers, knowledge bases, experiment systems, registries, templates, or governance mechanisms when useful, but those are local implementation choices rather than Foundation semantics.

The purpose is narrower: to make the movement from insufficient understanding toward better understanding explicit without collapsing that movement into another Foundation concept.

## 2. Position in the Foundation

The VAKI Thinking Model describes the broad reasoning topology of observation, framing, modeling, hypothesis formation, experimentation, evidence interpretation, decision, manifestation, sharing, and feedback.

The Questions and Inquiry Model refines a cross-cutting semantic layer within that topology:

```text
insufficient understanding
  -> Question
  -> Inquiry
  -> changed understanding
  -> Answer, refined Question, suspended Question, reopened Question, Decision relevance, or further Inquiry
```

This is not a workflow or lifecycle. It names common semantic relations. A manifestation may move through them in different orders, revisit them, skip explicit representation where risk is low, or combine them with local practices.

Questions may arise before problem framing, inside problem framing, after evidence, during decision reasoning, from manifestation feedback, or from open-ended exploration. Inquiry may involve observation, modeling, hypothesis formation, evidence synthesis, experiment, comparison, simulation, interaction with reality, or reconsideration of prior reasoning. None of these activities is required in every inquiry.

The Foundation needs this model because existing documents already rely on questions. Evidence may be relevant to a question. Signals may indicate something relevant to a question. Experiments and prototypes may answer a question. Operation may expose new questions. Without a semantic owner, manifestations could silently redefine question as uncertainty, problem, hypothesis, evidence gap, experiment objective, or decision need.

## 3. Question

A Question is an explicit orientation of reasoning toward something not sufficiently understood for the current purpose.

A Question is explicit because it gives shape to what reasoning is trying to understand. It is not merely background ignorance, unease, confusion, or possibility. It does not have to be formally written, assigned, or tracked in a system, but it must be distinguishable enough that later reasoning can understand what was being pursued.

A Question concerns insufficient understanding. The insufficiency may involve what is true, what matters, why something happened, whether a model applies, which assumptions are fragile, what evidence is missing, what an observation means, whether an intervention will work, or whether a decision depends on unresolved knowledge.

A Question is relative to purpose. A question may be sufficient for one purpose and too vague, too broad, or too unresolved for another. Purpose does not have to be an immediate decision. It may be scientific, exploratory, operational, design-oriented, educational, diagnostic, interpretive, or preparatory.

A Question is not identical to:

- Uncertainty: uncertainty is a recognized limit of current knowledge, observation, model, or interpretation. A Question orients reasoning toward some aspect of insufficient understanding.
- Unknown: something may be unknown without being explicitly questioned.
- Problem: a problem is a situation being addressed. A Question asks what must be understood.
- Problem Frame: a problem frame describes current state, desired state, actors, constraints, uncertainties, assumptions, and consequences. A Question may precede, inhabit, challenge, or revise that frame.
- Claim: a claim asserts something. A Question does not assert its own answer.
- Hypothesis: a hypothesis is a provisional, testable claim. A Question may generate hypotheses, but is not one.
- Assumption: an assumption is taken as a condition in reasoning. A Question may expose, test, or challenge assumptions.
- Evidence Gap: an evidence gap is missing support relative to an object of evaluation. A Question may reveal an evidence gap, but is not reducible to one.
- Decision Situation: a decision situation exists when a choice or commitment can materially affect consequences, learning, constraints, resources, direction, or future options. A Question may be decision-relevant without being a decision situation.
- Information Request: an information request asks for information. A Question may require interpretation, modeling, observation, comparison, experiment, or reframing rather than simply retrieving information.

A Question does not have to be immediately answerable. A valuable Question may be partially answerable, indirectly answerable, currently unanswerable, or useful because it exposes the limits of present understanding.

## 4. Inquiry

Inquiry is the directed and revisable pursuit of better understanding in relation to one or more Questions.

Inquiry is directed because it is oriented by a Question. Without some Question or insufficient understanding that matters, activity may still produce data, observations, artifacts, or motion, but it is not yet inquiry in the VAKI sense.

Inquiry is revisable because the Question, context, assumptions, evidence, interpretation, and relevance may change. Inquiry may clarify the original Question, decompose it, narrow it, broaden it, replace it, suspend it, resolve it for the current purpose, or expose deeper Questions.

Inquiry may involve, depending on context:

- further observation;
- inspection;
- comparison;
- modeling;
- simulation;
- synthesis of existing evidence;
- hypothesis formation or revision;
- deliberate experiment;
- asking another person;
- operational trial;
- interaction with reality;
- reconsideration of prior reasoning.

These are examples, not a sequence. Inquiry is not synonymous with experiment, research project, investigation procedure, data collection, or decision analysis.

An experiment is one possible form of inquiry activity. A research project may contain inquiry, but inquiry is not a project-management container. Data collection may support inquiry, but data collection without a meaningful relation to a Question is not sufficient. Decision analysis may use inquiry, but not all inquiry is decision-driven.

The purpose of Inquiry is not to force certainty. It is to improve understanding enough for the relevant purpose while preserving what remains unresolved.

## 5. Inquiry Context

Inquiry Context is the question-facing purpose, assumptions, constraints, current understanding, and relevance that make a Question meaningful and bound its pursuit.

Inquiry Context is not a mandatory schema or template. It does not require a fixed list of fields, a record type, a database, a graph, or an issue tracker.

Important inquiry should preserve enough context to understand:

- why the Question mattered;
- what purpose bounded the Inquiry;
- which assumptions materially shaped it;
- what was understood at the time;
- what constraints affected possible Inquiry;
- why a later Answer, suspension, resolution, or reopening was reasonable.

Inquiry Context is distinct from Observation Context, evidential context, contextual validity, and decision context.

Observation Context is owned by the Observation Model and concerns the conditions needed to understand an observation. Evidential interpretation and contextual validity are owned by the Evidence Model and concern how information bears on an object of evaluation. Decision context is owned by the Decision Model and concerns what commitment is justified under evidence, uncertainty, consequence, timing, and reversibility.

Inquiry Context owns only the context needed to understand the Question and its pursuit. It does not own the full context of an observation, evidential interpretation, decision situation, or problem frame.

## 6. Question Emergence

Questions may arise wherever insufficient understanding becomes important enough to orient reasoning.

Sources may include:

- Observation;
- anomaly;
- contradiction;
- failed expectation;
- Uncertainty;
- missing evidence;
- model failure;
- Hypothesis failure;
- experiment result;
- Decision need;
- Manifestation Feedback;
- operational failure;
- opportunity;
- intent;
- disagreement;
- newly available capability;
- changed context.

This list is illustrative. It is not a required causal pipeline.

The Questions and Inquiry Model does not own the source semantics. Observation remains owned by the Observation Model. Signal, Evidence, evidential interpretation, bodies of evidence, and Uncertainty remain owned by the Evidence Model. Problem Framing, Modeling, Hypothesis, Experiment, Manifestation, Share, and Feedback topology remain owned by the Thinking Model. Decision Situation, Decision Object, Decision Reasoning, Commitment, Reversibility, Optionality, Cost of Delay, and Learning Value remain owned by the Decision Model.

This model owns the Question once insufficient understanding becomes explicitly oriented as inquiry.

## 7. Question Evolution

Questions are revisable. They may change as understanding changes.

Question evolution names possible semantic changes to a Question. It does not define lifecycle states, workflow transitions, maturity gates, or required sequencing.

A Question may be:

- articulated, when vague insufficient understanding becomes explicit enough to guide reasoning;
- clarified, when ambiguous terms, scope, purpose, or assumptions are made more understandable;
- decomposed, when a broader Question is separated into subquestions;
- refined, when inquiry narrows, sharpens, or adjusts what is being asked;
- reframed, when inquiry changes the underlying interpretation of what matters;
- replaced, when a better Question supersedes the original orientation of reasoning;
- resolved for the current purpose, when understanding is sufficient for the purpose at hand;
- suspended, when further inquiry is not currently justified, possible, relevant, or timely;
- reopened, when evidence, context, assumptions, purpose, or relevance materially changes.

Question decomposition is lightweight. Subquestions may clarify parts of a broader Question, depend on other Questions, expose assumptions, change the parent Question, or become irrelevant after another Question is resolved.

This model does not define dependency graph schemas, identifiers, storage mechanisms, registries, or backlog structures.

## 8. Inquiry and Existing Models

### 8.1 Question and Uncertainty

The Evidence Model owns Uncertainty semantics.

Uncertainty is the recognized limit of current knowledge, observation, model, or interpretation. A Question is the explicit orientation of reasoning toward something not sufficiently understood for the current purpose.

The relationship is many-to-many:

- not every uncertainty becomes a Question;
- one uncertainty may generate multiple Questions;
- one Question may expose multiple uncertainties;
- Inquiry may reduce uncertainty;
- Inquiry may reveal uncertainty;
- Inquiry may relocate uncertainty;
- Inquiry may reframe uncertainty;
- a Question may exist without an immediate Decision Situation.

Inquiry should preserve uncertainty where certainty is not justified. Resolving a Question for a current purpose does not mean all related uncertainty has disappeared.

### 8.2 Question and Problem Framing

The Thinking Model owns Problem Framing.

A Question is not a Problem Frame. A Problem Frame describes the current state, desired state, actors, constraints, uncertainties, assumptions, and consequences that define the problem being addressed. A Question orients reasoning toward something not sufficiently understood.

The relationship has no required ordering:

- a Question may arise before a Problem Frame;
- a Question may exist inside a Problem Frame;
- a Problem Frame may generate Questions;
- Inquiry may revise or invalidate a Problem Frame;
- Inquiry may exist with no immediate problem-solving purpose.

Open-ended scientific inquiry, exploratory research, operational diagnosis, design exploration, and decision-driven inquiry can all use Questions without forcing the same problem-framing sequence.

### 8.3 Question and Hypothesis

The Thinking Model and Glossary own Hypothesis semantics.

A Question is not a Hypothesis. A Hypothesis is a provisional, testable claim about how reality behaves or how a proposed intervention is expected to work.

Inquiry may proceed without a formal Hypothesis. A Question may generate multiple competing Hypotheses. A Hypothesis may be weakened or invalidated without resolving the original Question. Hypothesis failure may reframe the Question, replace it with a better Question, or expose another Question that matters more.

A Hypothesis is not automatically an Answer merely because it is plausible, preferred, currently unchallenged, or convenient.

### 8.4 Inquiry and Observation

The Observation Model owns Observation semantics.

Inquiry may orient attention, inspection, measurement, or interaction with reality. It may influence what is sought, what is inspected, or where attention is directed.

That influence does not make the Questions and Inquiry Model the owner of:

- what it means to become an Observation;
- selection semantics;
- Observation Context;
- preservation;
- provenance;
- measurement boundary;
- correction;
- absence of observation;
- observation of absence;
- Observation Quality;
- the boundary between feedback and observation.

Inquiry may influence what is sought. The Observation Model owns what is observed and preserved.

### 8.5 Inquiry and Evidence

The Evidence Model owns Signal, Evidence, evidential interpretation, Evidence Quality, Evidence Strength, Body of Evidence, and Uncertainty.

Evidence may bear on a Question when interpretation makes clear what aspect of the Question is supported, weakened, qualified, unresolved, or reframed.

Often the evidential relation will be mediated through:

- Claim;
- Hypothesis;
- Model;
- Uncertainty;
- Decision Context.

Mediation is not required in every case. A preserved observation or body of evidence may directly affect a Question when the interpretive relation is clear. For example, evidence may show that a Question was based on a false assumption, that the Question needs narrower scope, that no responsible answer is possible under current conditions, or that a partial Answer is sufficient for the current purpose.

Evidence does not become evidence merely because it is attached to a Question. The Evidence Model still owns whether information bears evidentially, with what quality, strength, scope, limitations, and interpretation.

### 8.6 Inquiry and Decision

The Decision Model owns Decision reasoning and Commitment semantics.

Inquiry may be decision-driven when a Decision depends on better understanding. Inquiry may be decision-relevant when its outcome could affect future commitment. Inquiry may also exist without immediate commitment.

A Decision may be made while important Questions remain unresolved. Making a Decision does not resolve a Question. A Decision is a justified commitment under current knowledge and uncertainty, not proof that inquiry is complete.

A Question may be suspended because further Inquiry is not currently justified. That judgment may depend on consequence, reversibility, optionality, cost of delay, learning value, or commitment reasoning, all of which remain owned by the Decision Model.

A Question may reopen after evidence, context, assumptions, purpose, or relevance changes. Decision review and commitment trace remain owned by the Decision Model; Question Reopening remains owned by this model.

## 9. Answer and Resolution

An Answer is a bounded response to a Question that changes understanding within relevant scope, context, assumptions, and remaining uncertainty.

Answer is a lightweight concept in this model. This document does not define an Answer taxonomy.

An Answer is not universal closure. It may be provisional, incomplete, context-bound, indirect, or revisable. It may expose deeper Questions. Inquiry does not always produce an Answer.

Question Resolution is the condition in which a Question has been answered sufficiently for the current purpose without implying universal truth.

Resolution means that the Question no longer needs further inquiry for the purpose currently in view. It does not mean:

- the Answer is universally true;
- the Question can never reopen;
- all related uncertainty has been eliminated;
- no future evidence can change the Answer;
- a Decision or Commitment is automatically justified;
- every manifestation must treat the Question as resolved in every context.

The scope and assumptions of an Answer matter. Preserving an Answer without preserving its scope, assumptions, context, or remaining uncertainty can turn useful understanding into misleading certainty.

## 10. Suspension and Reopening

Question Suspension is the semantic treatment of an unresolved Question as not currently pursued because further Inquiry is not currently justified, possible, relevant, or timely.

Suspension is not resolution. A suspended Question remains unresolved. Suspension preserves the distinction between "not currently pursuing" and "answered."

A Question may be suspended because:

- current evidence is insufficient and further inquiry is not currently possible;
- the Question is no longer relevant to the current purpose;
- another Question has become more important;
- the cost or delay of further inquiry is not currently justified;
- the Question is currently unanswerable under available conditions;
- the Question should be revisited only if context changes.

These are examples, not required categories.

Currently unanswerable is not false. Irrelevant for the current purpose is not disproven. Suspended is not resolved.

Question Reopening is renewed Inquiry into a previously resolved or suspended Question because evidence, context, assumptions, purpose, or relevance has materially changed.

Resolution does not prevent later reopening. Reopening is understood in relation to prior Answers, assumptions, evidence, Negative Knowledge as defined by the Evidence Model, and the context under which the Question was previously resolved or suspended.

A Question may be malformed when its assumptions, framing, wording, or structure prevent responsible Inquiry or Answer. Such a Question may need clarification, reframing, decomposition, or replacement. This model does not define a formal category system for malformed Questions.

## 11. Recursive Inquiry

Inquiry is recursive and revisable.

An Answer may lead to a deeper Question. Evidence may revise the Question it was intended to address. Contradiction may generate further Inquiry. Decomposition may create subquestions. A subquestion result may revise the parent Question. Changed context may reopen a Question. Manifestation Feedback may generate new Questions. A malformed Question may be replaced by a better Question.

These relations are not a process pipeline. They express the fact that inquiry changes the understanding that made the original inquiry meaningful.

Recursive Inquiry is not failure. Refusing to revise a Question after evidence, context, assumptions, or understanding change is the failure.

## 12. Question Quality

Question Quality is multidimensional, context-dependent, and non-scoring.

VAKI does not define a universal question quality checklist or score. A single metric would hide why a Question may be useful in one context and weak in another.

Relevant dimensions may include:

- Relevance: whether the Question matters to the purpose, uncertainty, model, evidence, decision, or learning at hand.
- Clarity: whether the Question is understandable enough to orient reasoning.
- Scope: whether the Question is bounded enough to pursue without silently excluding what matters.
- Answerability: whether the Question can be responsibly answered, partially answered, indirectly answered, or recognized as currently unanswerable.
- Assumption Exposure: whether the Question reveals assumptions that materially affect reasoning.
- Discriminatory Power: where relevant, whether the Question can distinguish between competing explanations, hypotheses, models, or options.
- Capacity to orient useful Inquiry: whether the Question can guide observation, evidence synthesis, modeling, comparison, or other reasoning activity.

Answerability must be treated carefully. A valuable Question may be partially answerable, indirectly answerable, currently unanswerable, or valuable because it exposes limits rather than producing a final Answer.

Question Quality is distinct from Observation Quality, Evidence Quality, Evidence Strength, and Decision Quality. Those remain owned by their respective models.

## 13. Inquiry Traceability

Inquiry Traceability is the conceptual ability to understand where a Question came from, why it mattered, what bounded its Inquiry, what changed in understanding, and how the Question evolved.

Important Inquiry should be traceable enough to understand:

- where the Question came from;
- why the Question mattered;
- what Inquiry Context bounded it;
- what changed in understanding;
- whether the Question was refined, replaced, resolved, suspended, or reopened;
- whether later reasoning changed in relation to the Inquiry.

This traceability is conceptual. It does not imply identifiers, registries, databases, graphs, issue trackers, mandatory records, schemas, or tooling.

Traceability ownership is layered:

- the Observation Model owns Observation origin trace;
- the Evidence Model owns evidential relationship trace;
- the Decision Model owns Decision reasoning and Commitment trace;
- this model owns Question origin, Inquiry Context, and Question evolution trace.

The purpose is not bureaucracy. The purpose is to preserve enough meaning that later reasoning can understand, challenge, revise, or reuse the inquiry.

## 14. Failure Modes

Common question and inquiry failure modes include:

- a leading Question that assumes the desired direction of reasoning;
- a Question that contains its preferred Answer;
- Uncertainty mistaken for a Question;
- a Problem mistaken for a Question;
- a Hypothesis treated as an Answer;
- data collection without a meaningful Inquiry relation;
- Evidence answering a proxy Question instead of the actual Question;
- a Decision treated as Question Resolution;
- a currently unanswerable Question treated as false;
- Question origin or purpose lost;
- available tools defining the Question;
- measurable Questions crowding out harder but important Questions;
- Inquiry reopened while ignoring relevant negative knowledge;
- an Answer preserved without scope, assumptions, context, or remaining uncertainty.

These failure modes are not governance controls, checklist items, approval gates, or workflow requirements. They are recurring ways inquiry can become detached from understanding, context, evidence, uncertainty, or purpose.

## 15. Invariants

Across VAKI manifestations:

1. A Question must remain distinguishable from the Uncertainty, Problem, Claim, Hypothesis, Assumption, or Decision Situation that gave rise to it.
2. Inquiry must remain revisable when evidence, context, assumptions, purpose, or understanding changes the relevance, scope, or framing of the Question.
3. A Hypothesis must not be treated as an Answer merely because it is plausible, preferred, or currently unchallenged.
4. An Answer must preserve enough scope, assumptions, context, and remaining uncertainty to prevent unjustified generalization.
5. A Decision made while Inquiry remains unresolved must not silently convert the Question into a resolved Question.
6. Inquiry may reduce, reveal, relocate, or reframe Uncertainty.
7. A Question may be suspended without being resolved and may be reopened when evidence, context, assumptions, purpose, or relevance materially changes.

## 16. Relationship to Existing Documents

This model refines the question and inquiry semantics used across the Foundation without replacing existing ownership.

The [VAKI Thinking Model](README.md) owns the broad reasoning topology, including Problem Framing, Modeling, Hypothesis, Experiment, Decision, Manifestation, Share, and Feedback topology. This model defines how Questions and Inquiry move within and across that topology.

The [Observation Model](OBSERVATION_MODEL.md) owns Observation, Observation Context, selection, preservation, provenance origin, measurement boundary, correction, absence/non-observation, Observation Quality, and the feedback-to-observation boundary. This model may describe how Inquiry orients attention, but it does not define what becomes an Observation.

The [Evidence Model](EVIDENCE.md) owns Signal, Evidence, evidential interpretation, Evidence Quality, Evidence Strength, Body of Evidence, and Uncertainty. This model defines how Questions relate to Inquiry and how evidence may bear on a Question without redefining Evidence.

The [Decision Model](../method/DECISION_MODEL.md) owns Decision Situation, Decision Object, Decision Reasoning, Commitment, Reversibility, Optionality, Cost of Delay, Learning Value, and decision/commitment trace. This model defines why Questions may remain unresolved, suspended, or reopened even when a Decision has been made.

The [Design Methodology](../method/DESIGN_METHODOLOGY.md) owns domain-independent system evolution guidance. This model defines question and inquiry semantics that may operate inside that methodology without prescribing a local design process.

The [Foundation Specification](../FOUNDATION_SPEC.md) and [ADR-0001](../../decisions/ADR-0001-foundation-manifestation-boundary.md) own the Foundation-to-manifestation relationship. This model respects that boundary by defining shared meaning while leaving domain-specific inquiry practices, tools, workflows, records, and governance to manifestations.
