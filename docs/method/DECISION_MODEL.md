# VAKI Decision Model

## 1. Purpose

This document defines how VAKI chooses an appropriate commitment under current evidence, uncertainty, consequences, timing, and reversibility.

It is the semantic foundation of decision reasoning. Operational decision processes, workflows, record formats, approval mechanisms, governance practices, and implementation tooling may be created by manifestations, but they are not defined here.

The model is domain-independent. It applies across software, research, physical systems, machines, vessels, products, processes, and other manifestations without prescribing local tools, governance roles, approval gates, schemas, scoring systems, or templates.

VAKI does not treat decisions as the end of uncertainty. Decisions are commitments made while uncertainty remains.

## 2. Position in the Thinking Model

The Evidence Model establishes the boundary used here:

```text
Experiment or interaction with reality
  -> Observation
  -> Evidence
  -> changed state of uncertainty
  -> decision reasoning
```

The Decision Model begins at decision reasoning. It uses the current body of evidence and state of uncertainty to determine what commitment is justified, including its size, reversibility, timing, and consequences.

Evidence changes what is reasonable to believe. It does not mechanically determine a decision. Decision reasoning determines what is reasonable to commit while uncertainty remains. Commitment then constrains what can become manifest.

The semantic bridge is:

```text
Evidence
  -> changed state of uncertainty
  -> Decision Reasoning
  -> Commitment
  -> Manifestation
```

This bridge is not a lifecycle. It clarifies that commitment connects reasoning to the reality-facing form of a manifestation.

In the broader Thinking Model:

```text
Evidence
  -> Decision
  -> Manifestation
  -> Share
  -> Feedback
  -> Observation
```

This position does not make decision a one-way passage. Evidence may send reasoning backward to framing, modeling, hypothesis, or experiment. Feedback may revise the decision or show that a previous decision remains appropriate.

## 3. Decision Situation

A decision situation exists when a choice or commitment can materially affect consequences, learning, constraints, resources, direction, or future options.

A useful decision situation makes visible:

- what requires a choice or commitment;
- why a decision is needed now or under current conditions;
- what happens if no explicit decision is made;
- relevant timing or decision windows;
- relevant constraints;
- current uncertainty;
- affected scope.

Not every uncertainty creates a decision situation. Some uncertainty can be observed, tolerated, deferred, or made irrelevant by the design. Not every decision requires extensive analysis. The amount of reasoning preserved should be proportional to the consequences of losing that reasoning.

Inaction, delay, and continuation can create consequences. When they do, they are part of the decision situation rather than the absence of a decision.

A choice, preference, or mental selection is not necessarily a decision. A choice becomes decision-relevant when it creates or implies material commitment.

## 4. Decision Object

The decision object is what is actually being decided.

A decision object may concern:

- direction;
- allocation;
- commitment;
- constraint;
- experiment;
- continuation;
- pause;
- reversal;
- abandonment.

The decision object should be specific enough to expose the commitment being created. Vague decisions such as "continue improving" hide the real choice. The actual decision may be to allocate effort, keep a direction, postpone a competing option, preserve a capability, run an experiment, or accept a constraint.

The same situation may contain several decision objects. Separating them prevents a broad decision from being justified by evidence that only supports a narrower one.

A choice without commitment is not yet a decision in the VAKI sense. The relevant commitment may concern resources, direction, constraints, dependencies, scope, future options, or irreversibility.

## 5. Options and Inaction

A decision should consider materially distinct options. Exhaustive enumeration is not required, and often is not useful. The relevant question is whether the reasoning has avoided a false binary and has considered the options that could change the appropriate commitment.

Options may include:

- acting now;
- acting in a smaller or staged way;
- experimenting before broader commitment;
- continuing the current state;
- delaying intentionally;
- delegating the decision to another context;
- reversing a prior decision;
- stopping an effort.

Options differ not only in expected outcome. They may also differ in:

- reversibility;
- information gained;
- future options preserved or destroyed;
- delay introduced;
- resources committed;
- dependencies created;
- constraints imposed.

A false binary occurs when a situation is framed as only "do it" or "do not do it" while smaller commitments, reversible actions, experiments, pauses, or scope changes are available.

## 6. Body of Evidence and State of Uncertainty

Decision reasoning uses a body of evidence as defined by the Evidence Model: relevant evidence considered together in relation to a claim, uncertainty, model, or decision.

A body of evidence may contain:

- support;
- contradiction;
- qualification;
- unresolved conflict;
- known gaps;
- dependencies between evidence.

The Decision Model must not collapse this body into one confidence score. Strong evidence for a narrow claim may be insufficient for a broad commitment. Weak evidence may still justify action when waiting is costly, the decision is reversible, or inaction creates greater consequences.

Decision reasoning also uses the current state of uncertainty. Uncertainty is not a scalar. A decision may face uncertainty about:

- what is true;
- what matters;
- what will happen;
- whether evidence transfers;
- whether effects are reversible;
- whether delay changes the situation;
- whether observations are trustworthy;
- whether objectives or constraints are stable.

The purpose of evidence is not to eliminate uncertainty. Its purpose is to change the state of uncertainty enough to improve the next commitment.

Action may be justified even when important uncertainty remains.

## 7. Consequences and Trade-offs

Decision reasoning considers consequences of:

- choosing an option;
- choosing incorrectly;
- waiting;
- doing nothing;
- losing future options;
- creating commitments that are expensive to reverse.

A trade-off exists when an option improves one relevant value, constraint, capability, or future condition while degrading or risking another.

Trade-offs should be made visible when they affect important decisions. They should not be hidden inside preference, momentum, or a single summary judgment.

VAKI does not require a universal risk formula. The relevant consequence structure depends on the decision object, affected scope, reversibility, uncertainty, and timing.

## 8. Reversibility

VAKI follows the principle:

```text
Reversibility where uncertainty is high.
```

Reversibility is the degree to which a decision can be changed, undone, narrowed, or redirected without unacceptable loss of resources, time, trust, capability, safety, or future options.

Reversibility does not mean indecision. A reversible decision is still a commitment. It is a commitment designed so that reality can teach without forcing premature permanence.

Reversible decisions can often be made with less evidence because the cost of error is bounded and the action may produce useful information.

Irreversible, path-dependent, or expensive-to-reverse decisions usually require stronger evidence, narrower scope, staged commitment, or explicit acceptance of the consequence of being wrong.

Reversibility is never free. Apparent reversibility may hide switching costs, lost time, damaged credibility, dependencies, or destroyed options. A decision should not be called reversible merely because it can be described as reversible.

## 9. Optionality

Optionality is the preservation or creation of meaningful future choices.

An option can be valuable because it:

- preserves freedom to change direction;
- delays irreversible commitment;
- creates new information;
- exposes constraints;
- enables adaptation.

Optionality matters when future learning, context change, or unresolved uncertainty may change what should be done next.

Optionality is not a universal objective. Preserving every option can consume resources, delay learning, obscure commitment, or prevent coherent action. Sometimes commitment is necessary because the value of focused action exceeds the value of keeping alternatives open.

The question is not whether optionality is good in the abstract. The question is which future choices are meaningful enough to preserve or create under current uncertainty and consequence.

## 10. Cost of Delay

Waiting is not neutral.

Decision reasoning should consider:

- information expected from waiting;
- opportunity lost through delay;
- cost accumulated while waiting;
- whether the environment is changing;
- whether the decision window may close;
- whether delay itself creates dependencies or constraints.

Waiting may be rational when it is likely to improve the decision more than it degrades the situation. Waiting may be irrational when the expected information is weak, late, redundant, or irrelevant to the commitment being considered.

VAKI does not prefer speed for its own sake. The issue is whether delay changes the evidence, uncertainty, options, consequences, or timing enough to justify its cost.

## 11. Learning Value

Learning value is the extent to which a decision is expected to produce evidence that can change future reasoning.

A decision may have learning value when it:

- tests a hypothesis;
- exposes a constraint;
- creates feedback;
- reveals whether evidence transfers;
- clarifies reversibility;
- distinguishes signal from outcome;
- reduces uncertainty relevant to a later commitment.

Experiment, prototype, staged commitment, and reversible action are common ways to create learning value.

Learning value does not always dominate direct utility. A decision that teaches little may still be appropriate when the evidence is sufficient, timing is urgent, or the necessary commitment is clear. A decision that teaches much may still be inappropriate if it creates excessive consequence, destroys critical options, or delays a necessary commitment.

## 12. Commitment

Commitment is the amount of resources, direction, constraints, dependency, or irreversibility created by a decision.

The central architectural principle of the Decision Model is:

```text
Commitment should increase only as justified by evidence, uncertainty reduction, consequences, and reversibility.
```

This is not an equation and not a scoring rule. It is a constraint on reasoning.

Commitment may be:

- incremental;
- staged;
- bounded;
- provisional;
- conditional;
- full.

These are not mandatory lifecycle states. They are ways to align commitment with the current decision situation.

High uncertainty does not always require low commitment. If delay is dangerous, inaction is worse, or the decision window is closing, a larger commitment may be rational even under uncertainty. In that case, the reasoning should preserve why the consequence of waiting or inaction justified the commitment.

Low uncertainty does not automatically justify broad commitment. Evidence may be strong locally but weak in transfer, scope, durability, or system-level relevance.

## 13. Decision

A decision is a commitment of resources, direction, or constraints based on the current state of knowledge.

A decision may arise from a choice, but it is not identical to choice. It exists when selection, continuation, delay, pause, abandonment, or preservation of an option creates material commitment or consequences.

Important decisions should preserve:

- context;
- decision object;
- options considered;
- assumptions;
- body of evidence;
- current uncertainties;
- constraints;
- trade-offs;
- expected consequences;
- reversibility;
- optionality affected;
- cost of delay;
- learning value;
- conditions for reconsideration.

The purpose is not process overhead. It is to preserve the reasoning needed for later understanding, challenge, adaptation, and revision.

A decision is not proof. It is a justified commitment made under the limits of what is currently knowable and relevant.

## 14. Decision Quality and Outcome Quality

Decision quality and outcome quality are distinct.

A rational decision may produce a bad outcome when reality changes, uncertainty resolves unfavorably, evidence was incomplete in a way that could not reasonably be known, or a low-probability consequence occurs.

A poor decision may produce a good outcome through luck, hidden compensating factors, or conditions that happened to favor it.

Decision quality should be evaluated against what was knowable, relevant, and reasonably interpretable at the time, including:

- the decision situation;
- the body of evidence;
- uncertainty that remained;
- options considered;
- consequences and trade-offs;
- timing;
- reversibility;
- assumptions and constraints.

Outcome quality matters for learning. It should revise evidence, models, and future decisions. It should not be used to erase the reasoning context of the original decision.

## 15. Review Conditions

Important decisions should identify conditions under which they should be revisited.

Possible review triggers include:

- new evidence;
- changed assumptions;
- changed constraints;
- changed objectives;
- unexpected consequences;
- expiration of contextual validity;
- contradiction between expected and observed behavior;
- loss of reversibility previously assumed;
- cost of delay changing materially;
- optionality being consumed faster than expected.

Review conditions are not periodic review schedules, approval cycles, workflow states, or governance transitions. They are reasoning triggers that preserve the ability to revise a decision when its basis changes.

A decision may remain rational even when later evidence makes a different decision appropriate.

## 16. Decision Failure Modes

Common decision failure modes include:

- narrative over reality;
- hidden assumptions;
- false certainty;
- treating absence of options as absence of choice;
- confusing confidence with consequence;
- treating evidence strength as decision strength;
- sunk-cost attachment;
- outcome bias;
- hindsight bias;
- analysis paralysis;
- premature commitment;
- reversible decisions treated as irreversible;
- irreversible decisions treated as cheap experiments;
- ignoring cost of delay;
- preserving optionality after it has become more costly than useful;
- destroying optionality without recognizing it;
- mistaking local success for system-level success;
- treating inaction as neutral when it changes consequences.

These failure modes are not a checklist. They are recurring ways decision reasoning becomes detached from evidence, uncertainty, consequence, or reality.

## 17. Traceability

Important decisions should be traceable to the reasoning that made them understandable.

The evidence trace is:

```text
Decision
  -> Body of Evidence
  -> Evidence
  -> Observation
  -> provenance, experiment, experience, or operational feedback
```

The reasoning trace also preserves:

```text
Decision
  -> assumptions
  -> uncertainties
  -> alternatives
  -> trade-offs
  -> expected consequences
  -> review conditions
```

Traceability is conceptual. This document does not define identifier systems, templates, databases, schemas, or tooling.

Traceability exists so a future person can understand why a decision was reasonable, what would change it, and how it should be revised when evidence, constraints, or context change. It does not imply ownership rules, approval roles, escalation paths, or authorization structures.

## 18. Decision and Action

A decision and an action are related but not identical.

A choice and a decision are also related but not identical. Choice selects or prefers; decision commits. A choice may remain private, tentative, or consequence-free. A decision changes what is committed, constrained, continued, stopped, preserved, or made possible.

A decision may:

- authorize action;
- constrain future action;
- delay action intentionally;
- initiate an experiment;
- stop an effort;
- preserve an option;
- create staged commitment;
- reverse or retire a prior commitment.

Action without an explicit decision can still create commitment. A decision without immediate action can still change direction, constraints, or future options.

The model distinguishes deciding from merely doing because VAKI cares about preserved reasoning, not only activity.

## 19. Relationship to Manifestation and Feedback

Decisions shape manifestations by selecting commitments that become concrete enough to interact with reality.

The relevant loop is:

```text
Decision
  -> Manifestation
  -> Share
  -> Operation
  -> Feedback
  -> Observation
  -> Evidence
  -> revised uncertainty
  -> decision revision or continuation
```

This document does not duplicate the Thinking Model. It clarifies the role of decision within the loop: decision reasoning converts current knowledge and uncertainty into justified commitment. Manifestation makes that commitment concrete enough to interact with reality, and later feedback tests whether the commitment remains appropriate.

Sharing strengthens the loop by preserving enough intent, assumptions, evidence, and trade-offs for others to inspect, operate, challenge, adapt, and learn from the manifestation.

## 20. Invariants

Across VAKI manifestations:

1. Decisions are made under uncertainty, not after uncertainty disappears.
2. Inaction, delay, and continuation are decisions when they affect consequences.
3. A choice without commitment is not yet a decision in the VAKI sense.
4. A decision object should expose the actual commitment being created.
5. Evidence requirements should be proportional to consequence, irreversibility, scope, cost of error, and cost of delay.
6. A body of evidence must not be collapsed into a universal confidence score.
7. Evidence changes what is reasonable to believe; decision reasoning determines what is reasonable to commit.
8. Commitment should increase only as justified by evidence, uncertainty reduction, consequences, and reversibility.
9. Reversible action can be a method of learning.
10. Irreversible or path-dependent commitment requires stronger justification or smaller staged commitment.
11. Waiting has both informational value and opportunity cost.
12. Optionality is valuable when future learning or context change matters, but preserving every option can itself be costly.
13. More analysis is not automatically better decision making.
14. Decision quality and outcome quality are distinct.
15. Important decisions should preserve enough reasoning to be understood, challenged, and revised.
16. Decisions should be revisited when their assumptions, evidence, constraints, objectives, or context materially change.
17. A decision may remain rational even when later evidence makes a different decision appropriate.

## 21. Relationship to Existing Foundation Documents

This model extends the Thinking Model by defining the decision layer that follows evidence and precedes manifestation.

It depends on the Evidence Model by using:

- body of evidence;
- state of uncertainty;
- contextual validity;
- traceability;
- revision and supersession;
- the distinction between evidence strength and decision strength.

It supports the Design Methodology by clarifying what it means to decide explicitly and how the smallest coherent manifestation should be bounded by current evidence and justified commitment.

It refines the Principles by making explicit:

- Reality over narrative;
- Make assumptions explicit;
- Evidence over intuition, intuition as hypothesis;
- Experiment to learn;
- Distinguish signal from outcome;
- Reversibility where uncertainty is high;
- Documentation preserves meaning;
- Evolution is part of design.

It respects ADR-0001 by remaining domain-independent. It defines shared decision semantics for the Foundation but does not prescribe technologies, workflows, schemas, approval structures, governance roles, or local operational procedures.

Manifestations may implement decision practices differently, but they should not silently redefine the core meanings of decision, evidence, uncertainty, commitment, reversibility, optionality, consequence, or traceability.
