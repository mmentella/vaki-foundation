# First Manifestation Validation Discovery

## 1. Executive Verdict

READY WITH VALIDATION GUARDRAILS.

The Foundation is ready to be tested against a first real Manifestation, provided the pilot is explicitly treated as validation of semantic usability rather than the beginning of M2, a new Foundation milestone, or a production Manifestation.

The most informative first pilot is a minimal Research Manifestation shaped around one real quantitative research question, one explicit hypothesis, one bounded dataset or dataset slice, one controlled investigation, explicit observations, evidence reasoning, and one decision recommendation or decision outcome.

This pilot is recommended because it applies pressure to the full M1 cognitive surface while remaining narrow enough to separate Foundation defects from quantitative-domain vocabulary, implementation friction, and local research practice.

Repository basis: this discovery pass used the current README, Foundation Specification, Glossary, Manifesto, Principles, Thinking Model, Questions and Inquiry Model, Hypothesis and Experiment Model, Observation Model, Evidence Model, Decision Model, Design Methodology, M1 closure report, M1.2 audit reports, and ADR-0001. The canonical philosophy file in the repository is `docs/philosophy/MANIFESTO.md`.

The pilot must not be allowed to become VAKI Quant. Its value is not production usefulness. Its value is whether Foundation semantics can guide a real Manifestation without becoming prescriptive, losing precision, or absorbing local concepts prematurely.

## 2. Why Manifestation Validation Comes Before M2

M1 is closed with non-blocking notes. The closure report states that M1 is semantically complete at Foundation level, that M1.6 is not needed, and that further cognitive models should not be added without concrete evidence from repository use or Manifestation experience.

The next architectural posture is therefore validation through real Manifestation use, not semantic expansion.

Manifestation validation should come before M2 because the Foundation now needs contact with reality-facing use. Repository-internal coherence has already been reviewed enough for M1 closure. Another general audit would mainly retest documents against documents. A pilot can test whether the semantics remain usable when a local domain must interpret, extend, implement, and preserve them under real constraints.

This does not reopen M1. It creates evidence that may later justify targeted clarification, local extension, another pilot, or, only under explicit reopening criteria, Foundation review.

## 3. Validation Question

The central validation question is:

```text
Can the Foundation guide a real Manifestation without becoming prescriptive,
losing semantic precision, or prematurely absorbing concepts that should remain
local to the Manifestation or its domain?
```

The first pilot should test five subquestions:

1. Can a local Manifestation interpret Foundation meanings while preserving their canonical distinctions?
2. Can it introduce local quantitative research concepts without making them Foundation concepts?
3. Can it use Question, Hypothesis, Experiment, Observation, Evidence, Decision, and Design as composable semantic structures without converting them into a mandatory workflow?
4. Can the Design Methodology guide the pilot without dictating tools, language, storage, dataset format, statistical method, orchestration, or repository layout?
5. Can feedback from the Manifestation return toward Foundation review through classification and evidence, without automatic promotion?

## 4. Candidate Pilot Assessment

### Recommended candidate: one quantitative hypothesis against one defined dataset

This candidate gives the best validation information per unit of complexity.

It has strong semantic coverage because quantitative research naturally exercises Question, Inquiry, Hypothesis, Experiment, Observation, Evidence, uncertainty, Decision, Design, domain extension, and implementation freedom. It is also bounded if restricted to one question, one hypothesis, one dataset slice, and one decision outcome.

It is realistic because quantitative research creates genuine pressure around data, measurement, signal, evidence, hypothesis status, model assumptions, proxy outcomes, and decision sufficiency. Those are exactly the places where Foundation semantics should either help or fail visibly.

It is repeatable enough for validation if the dataset boundary, observation context, evidence reasoning, assumptions, and decision basis are preserved. It does not require production trading infrastructure, live execution, or portfolio systems.

Its main risk is domain gravity. Quantitative vocabulary can expand quickly into alpha research, backtesting frameworks, market regimes, leakage controls, transaction cost models, risk models, execution assumptions, and portfolio construction. The pilot must use that pressure deliberately while refusing to canonize local domain terms.

### Alternative: minimal software engineering Manifestation

A small software engineering pilot would test Design Methodology and decision traceability well, but it would likely under-stress Observation and Evidence. Engineering implementation issues could also dominate the validation pass and be mistaken for Foundation defects.

It is useful later, especially for testing design and manifestation autonomy, but it is less informative as the first pilot.

### Alternative: personal decision-support Manifestation

This would exercise Question, Evidence, Decision, uncertainty, reversibility, and traceability. It would be bounded and low-cost.

Its weakness is realism under domain pressure. It may avoid the stronger semantic stress caused by measurement, dataset context, evidential interpretation, hypothesis challengeability, and local domain terminology. It could validate decision semantics but leave research semantics under-tested.

### Alternative: lightweight operational monitoring Manifestation

This would stress feedback-to-observation, signal versus outcome, observability, and operation. It is a good later pilot for Feedback, Observation, and Design.

As a first pilot, it risks narrowing the validation around runtime or operational behavior and may not sufficiently exercise Hypothesis, Experiment, and evidence-based decision reasoning.

### Alternative: larger VAKI Quant Manifestation

A larger VAKI Quant Manifestation would be premature.

It would introduce too many domains at once: quantitative research, data engineering, backtesting, risk, portfolio construction, execution, observability, orchestration, deployment, and possibly governance. Failures would become difficult to classify. Foundation defects, domain extension needs, implementation problems, and product-scope decisions would blur.

The first pilot should preserve VAKI Quant as a future beneficiary, not become it.

## 5. Recommended First Pilot

The recommended first pilot is:

```text
A minimal Research Manifestation that discovers and validates one quantitative
hypothesis against one defined dataset or bounded dataset slice, producing
explicit observations, evidence reasoning, and one decision recommendation
without creating production quantitative infrastructure.
```

The pilot should be real enough that the hypothesis could be wrong, the dataset could expose ambiguity, the evidence could be inconclusive, and the decision recommendation could be to stop, revise, narrow, continue, or run another experiment.

It should not be optimized to demonstrate success. It should be optimized to expose semantic failure.

## 6. Pilot Boundary

The minimum viable pilot boundary should include:

- one research question;
- one explicit hypothesis;
- one bounded dataset or dataset slice;
- one experiment family or controlled investigation;
- explicit observation records with enough context to inspect what was measured or detected;
- explicit evidence reasoning that states what the observations bear on and with what limitations;
- one decision outcome or decision recommendation;
- local design decisions needed to make the pilot coherent;
- a register of local semantic extensions, if any;
- a Foundation feedback report using the classification model in this document.

The pilot must remain out of scope for:

- live trading;
- execution engines;
- portfolio construction;
- risk engines;
- production market data infrastructure;
- large-scale symbolic discovery;
- distributed orchestration;
- production observability;
- capital allocation;
- broker or exchange integration;
- generalized backtesting platforms;
- reusable quantitative research frameworks;
- Foundation document edits;
- new Foundation semantic owners;
- M2 planning or implementation.

These exclusions are appropriate because they remove implementation and product complexity that would make semantic validation noisy. They do not remove the core semantic pressure: the pilot still has to interpret Foundation concepts, preserve epistemic distinctions, reason from observation to evidence, make a decision under uncertainty, and keep quantitative terms local.

## 7. Foundation Semantic Surfaces Under Test

The pilot should exercise these current Foundation surfaces without redefining them:

- Foundation and Manifestation relationship semantics from the Foundation Specification and ADR-0001;
- canonical terminology from the Glossary;
- non-pipeline reasoning topology from the Thinking Model;
- Question and Inquiry semantics from the Questions and Inquiry Model;
- Hypothesis and Experiment semantics from the Hypothesis and Experiment Model;
- Observation and Observation Context semantics from the Observation Model;
- Evidence, Signal, Body of Evidence, Uncertainty, Negative Knowledge, and Contextual Validity from the Evidence Model;
- Decision, Commitment, Reversibility, Optionality, Cost of Delay, Learning Value, and review conditions from the Decision Model;
- domain-independent design guidance from the Design Methodology;
- durable principles including Reality over narrative, Questions before solutions, Evidence over intuition, Experiment to learn, Distinguish signal from outcome, Reversibility where uncertainty is high, and Documentation preserves meaning.

The pilot should not treat this list as a mandatory stage sequence. It should use the relevant surfaces where the research case naturally requires them.

## 8. Finding Classification Model

### A. Foundation defect

A Foundation defect is a problem in canonical Foundation meaning or ownership that prevents legitimate Manifestation use.

Examples include:

- contradictory canonical meanings;
- missing semantic ownership for a domain-independent concept required by the pilot;
- ambiguity across canonical documents that cannot be resolved by existing ownership;
- a semantic boundary that fails under legitimate use;
- two Foundation concepts that cannot be distinguished in practice;
- a required cross-domain concept with no coherent semantic home.

A Foundation defect should be rare. It requires evidence that the problem belongs to shared meaning, not merely to the pilot's domain, implementation, or chosen method.

### B. Manifestation-local need

A Manifestation-local need is a concept, structure, procedure, convention, vocabulary item, or record needed by the pilot but not requiring Foundation ownership.

Examples may include local naming conventions, research notes, dataset handling rules, local acceptance criteria, local result formats, project-specific assumptions, or a pilot-specific interpretation record.

The test is whether the need helps this Manifestation operate clearly without changing Foundation meaning.

### C. Implementation problem

An implementation problem is caused by code, data handling, tooling, orchestration, performance, storage, interfaces, local architecture, environment, or deployment.

Implementation problems must not be misclassified as semantic defects merely because they slow the pilot down. A broken parser, inconvenient dataset format, slow computation, missing package, bad schema, or awkward notebook structure is not a Foundation problem unless it exposes a semantic ambiguity that remains after the implementation issue is removed.

### D. Domain-specific semantic extension

A domain-specific semantic extension is a concept genuinely required by the quantitative research domain but not necessarily universal enough for Foundation ownership.

Possible examples include market regime, alpha hypothesis, feature, backtest, walk-forward validation, overfitting, leakage, transaction-cost assumption, train/test split, benchmark, or lookahead bias. These examples are not canonized.

Such terms should be locally governed by the Manifestation. They should be recorded when they affect interpretation, evidence, decision, or claims of Foundation alignment. They should remain visibly local unless repeated cross-Manifestation evidence shows a broader need.

### E. Candidate Foundation clarification

A candidate Foundation clarification is a finding that does not yet prove a Foundation defect but suggests existing semantics may need clearer wording after repeated use.

This category is appropriate when the pilot can proceed by using existing owners, but confusion appears likely to recur in other Manifestations.

The threshold separating this from a Foundation defect is evidence of failure. A candidate clarification indicates risk or repeated interpretive friction. A defect indicates canonical contradiction, missing ownership, or boundary failure that cannot be resolved locally.

### Extension semantics discriminator

When the pilot introduces a new term or structure, classify it before asking whether Foundation should change:

| Candidate | Meaning in validation | Default disposition |
|---|---|---|
| Local term | A name used for readability inside this pilot | Keep local |
| Local specialization | A local narrowing or application of a Foundation concept that preserves canonical meaning | Document in the interpretation record |
| Domain semantic extension | A quantitative research concept needed across similar domain work but not proven cross-domain | Record in the domain extension register |
| Implementation construct | A code, data, tool, storage, orchestration, or architecture mechanism | Treat as implementation unless it exposes semantic ambiguity |
| Missing Foundation abstraction | A domain-independent concept required for legitimate Manifestation use and not coherently owned | Classify as candidate clarification or Foundation defect depending on evidence |

Use the least central classification that preserves honesty. A useful local concept should not move upward merely because it is important to the pilot.

## 9. Foundation Failure Signals

| Failure signal | What would be observed | Likely classification | Blocks pilot? | Triggers Foundation review? | Additional evidence needed |
|---|---|---|---|---|---|
| Incompatible interpretations of the same Foundation concept | Pilot records use Question, Hypothesis, Observation, Evidence, or Decision in mutually incompatible ways while all claim canonical alignment | Candidate clarification or Foundation defect | Only if the pilot cannot proceed honestly | Yes if not resolvable through existing owners | Show whether conflict remains after referencing the owning document |
| Pilot cannot proceed without adding implementation detail to Foundation | Team believes Foundation must prescribe language, storage, dataset format, statistical method, or runner | Manifestation-local need or implementation problem | No | No, unless Foundation text causes the belief | Identify which Foundation passage creates prescription pressure |
| Quantitative vocabulary promoted into Foundation because first pilot needs it | Local terms are written as if they are canonical shared VAKI concepts | Domain-specific semantic extension misclassified as Foundation | No, but block promotion | Yes only as boundary misuse | Show whether term is meaningful across materially different domains |
| Observation and Evidence collapse | Dataset rows, metrics, or results are treated as evidence without stating what they bear on | Foundation defect only if current owners cannot separate them; otherwise local misuse | No, unless uncorrected | Maybe | Map record to Observation Model and Evidence Model boundaries |
| Experiment means only software execution | Running code is called Experiment without inquiry arrangement, reality-facing relation, or conditions for observation | Manifestation-local misuse or candidate clarification | No, if corrected | Maybe if repeated | Determine whether confusion comes from Foundation wording or local tooling habits |
| Hypothesis reduced to trading rule or parameter configuration | A rule such as "buy when X" is treated as the hypothesis without a provisional claim about reality | Domain-specific extension or local misuse | No, if reframed | Maybe | Separate domain rule from challengeable claim |
| Decision reduced to automated action | A generated signal or action is called a Decision without commitment reasoning | Local misuse; possible candidate clarification | No, if decision record corrects it | Maybe if repeated | Show whether material commitment and options were considered |
| Design reduced to architecture or code structure | Design record only discusses repository layout or components, not intent, uncertainty, evidence, and evolution | Manifestation-local need or misuse | No | No, unless Foundation guidance is unusable | Compare against Design Methodology without prescribing architecture |
| Every local concept requires central approval | Pilot waits for Foundation validation before naming local concepts | Boundary misunderstanding | Yes if it prevents local work | Yes as Foundation/Manifestation relationship concern | Identify whether Foundation Specification is unclear or local governance invented approval |
| Divergence hidden as interpretation | Local meaning changes a canonical concept but is documented only as normal interpretation | Candidate clarification or Foundation defect if boundary cannot classify it | Yes if material | Yes | Determine whether divergence is explicit, bounded, and traceable |
| Implementation friction mistaken for semantic insufficiency | Tooling or data pain is presented as missing Foundation semantics | Implementation problem | No | No | Reproduce issue without semantic ambiguity |
| Foundation becomes mandatory procedural workflow | Pilot records stages as required gates because Foundation diagrams are read linearly | Candidate clarification | Yes if it distorts validation | Yes if repeated | Show whether non-pipeline language was ignored or insufficient |

## 10. Validation Surface Map

| Foundation surface | Pilot pressure | Evidence of success | Failure signal |
|---|---|---|---|
| Foundation-Manifestation relationship | Pilot must inherit and interpret Foundation meanings while making local choices | Foundation meanings, local interpretations, extensions, and implementation choices remain distinguishable | Local terms appear canonical, or Foundation is asked to approve implementation |
| Question | One research question must orient inquiry without asserting its answer | Question is explicit, bounded by purpose, and distinct from hypothesis, uncertainty, and decision need | Question contains preferred answer or becomes a hypothesis |
| Inquiry | Research activity must remain directed and revisable | Inquiry can refine, suspend, or reopen the question as evidence changes | Activity becomes data collection without question relation |
| Hypothesis | One provisional claim must be challengeable | Hypothesis states claim, conditions, expected observable consequences where useful, and possible weakening evidence | Hypothesis becomes a trading rule, parameter set, or desired outcome |
| Experiment | Investigation must create or select conditions for relevant observations | Experiment is an inquiry arrangement, not merely code execution; it can produce unexpected or inconclusive observations | Running a script is treated as sufficient semantic experiment |
| Observation | Dataset-derived records and results must preserve what was measured or detected with context | Observations remain distinguishable from interpretation, signal, and evidence | Metrics or rows are treated as conclusions |
| Evidence | Observations must bear on the hypothesis, question, uncertainty, or decision through interpretation | Evidence states relevance, support, contradiction, qualification, gaps, uncertainty, and contextual validity | Observation, signal, evidence, and decision collapse into one result |
| Uncertainty | Pilot must preserve remaining uncertainty after evidence | Evidence reduces, reveals, relocates, or reframes uncertainty without claiming certainty | One result is treated as proof |
| Decision | Pilot must produce a decision recommendation or outcome under uncertainty | Decision object, options, evidence, uncertainty, reversibility, cost of delay, learning value, and review conditions are visible enough | Decision becomes automated action or confidence threshold |
| Commitment | Recommendation must expose what commitment is justified | Commitment remains bounded, staged, reversible, or conditional as evidence warrants | Local success justifies broad production commitment |
| Design | Local design choices must be guided by intent and evidence without technology prescription | Tools, storage, methods, and layout are chosen locally and justified only where meaningful | Design is reduced to code architecture or Foundation dictates tools |
| Feedback | Pilot findings must return as observations/evidence for Foundation review | Feedback is classified and traceable without automatic promotion | Every lesson becomes a proposed Foundation change |
| Extension semantics | Quantitative terms must be introduced locally when needed | Domain terms are registered with local meaning, owner, and relation to Foundation concepts | Domain vocabulary is canonized or hidden inside Foundation terms |

## 11. Required Validation Artifacts

Use minimal artifacts. They may be lightweight Markdown records inside the pilot Manifestation. The Foundation should not prescribe exact formats.

| Artifact | Purpose | Owner | Question answered | Status |
|---|---|---|---|---|
| Pilot charter | Bound the pilot, exclusions, validation question, and stopping rule | Manifestation local | What is this pilot and what is it not? | Temporary validation scaffolding |
| Foundation interpretation record | State which Foundation meanings are inherited and how they are interpreted locally | Manifestation local, referencing Foundation owners | Can the pilot interpret without redefining? | Potentially reusable |
| Local semantic map | Show relations among question, hypothesis, experiment, observation, evidence, decision, and local domain terms | Manifestation local | Are concepts distinguishable in practice? | Temporary or reusable |
| Domain extension register | Record local quantitative concepts and why they remain local | Manifestation local | Which concepts are extensions rather than Foundation changes? | Reusable for domain Manifestations |
| Experiment record | Preserve the inquiry arrangement, assumptions, dataset boundary, and conditions | Manifestation local | What reality-facing investigation was performed? | Reusable |
| Observation record | Preserve what was observed, with context, provenance, scope, and limits | Manifestation local | What was measured or detected before interpretation? | Reusable |
| Evidence assessment | Interpret what observations bear on, with uncertainty and limitations | Manifestation local | What changed in credibility or uncertainty? | Reusable |
| Decision record | Preserve decision object, options, body of evidence, uncertainty, trade-offs, commitment, and review conditions | Manifestation local | What commitment or recommendation is justified? | Reusable |
| Design decision note | Record local implementation/design choices only when losing reasoning would matter | Manifestation local | Did Design guide without prescribing tools? | Reusable if lightweight |
| Semantic issue classification log | Classify validation findings using this report's model | Manifestation local with Foundation review input | Is this a defect, local need, implementation issue, extension, or clarification candidate? | Temporary validation scaffolding |
| Foundation feedback report | Summarize evidence relevant to Foundation review without automatic promotion | Manifestation local, submitted to Foundation review | What, if anything, should Foundation consider? | Temporary validation scaffolding |

Avoid separate artifacts when a single concise record can preserve the needed meaning. The required property is semantic visibility, not document count.

## 12. Feedback and Promotion Rules

A finding from one Manifestation must not automatically alter the Foundation.

Use this conservative rule:

1. Keep local when the concept, record, method, or convention is useful only for the pilot or its immediate domain.
2. Document as a domain extension when the concept is semantically meaningful in quantitative research but not obviously cross-domain.
3. Record as a candidate cross-Manifestation concern when the finding may recur outside quantitative research but lacks enough evidence.
4. Investigate through another Manifestation when the finding may be cross-domain but could be caused by the pilot's domain, tools, or research style.
5. Escalate as a probable Foundation defect when existing owners cannot resolve a legitimate use case without contradiction, silent redefinition, or missing ownership.
6. Reopen a closed Foundation semantic area only when evidence meets the M1 closure report's reopening criteria.

Promotion requires deliberate review. A local concept must survive abstraction from the Manifestation that produced it.

Before proposing promotion, ask:

1. Does the concept remain meaningful across materially different domains?
2. Can it guide reasoning or system evolution without prescribing implementation?
3. Would removing it create semantic fragmentation across Manifestations?
4. Is it mature enough to survive abstraction from the pilot?
5. Is there evidence from more than one context, or a severe single-context defect that existing owners cannot absorb?

## 13. Foundation Reopening Triggers

Foundation reopening should remain compatible with the M1 closure logic.

Open Foundation review when the pilot produces evidence of:

- a concrete semantic ownership gap;
- conflicting canonical interpretations;
- recurring or strongly predicted cross-domain semantic fragmentation;
- an intentionally distributed capability becoming incoherent in legitimate use;
- inability of existing semantic owners to absorb a clarification without distortion;
- a Foundation boundary that prevents local autonomy or permits silent redefinition;
- repeated collapse of distinct Foundation concepts after reasonable interpretation efforts.

Do not reopen M1 because of:

- desire for symmetry;
- aesthetic completeness;
- specialized quantitative terminology;
- one local team's preference;
- implementation pain;
- missing templates;
- missing workflow;
- a desire for central approval;
- success of the pilot;
- failure of the pilot caused by local design or tooling.

## 14. What Must Not Be Learned from a Single Pilot

The first pilot must not be treated as proof that:

- the Foundation is universally valid;
- quantitative research semantics should become Foundation semantics;
- all Manifestations should follow the same artifact set;
- the cognitive topology is a required lifecycle;
- the Design Methodology should prescribe tools or architecture;
- evidence records need a universal schema;
- local success justifies production VAKI Quant;
- a single domain's terminology is cross-domain language;
- every later Manifestation should begin with a quantitative research shape;
- absence of failure in one pilot means no Foundation defects exist.

The pilot can produce useful evidence. It cannot prove universal adequacy.

## 15. Recommended Execution Sequence

1. Freeze the Foundation reference state for the pilot by identifying the exact documents used.
2. Create the pilot charter with explicit scope and exclusions.
3. Create a Foundation interpretation record for only the relevant concepts.
4. Define the research question and inquiry context.
5. State one hypothesis and its relevant assumptions or expected observable consequences.
6. Bound the dataset or dataset slice.
7. Define the experiment or controlled investigation as an inquiry arrangement, not as a tool choice.
8. Run the local investigation using any appropriate local method.
9. Preserve observations with context before evidential interpretation.
10. Assess evidence against the question, hypothesis, uncertainty, and decision context.
11. Produce one decision recommendation or outcome with bounded commitment and review conditions.
12. Record local domain extensions and implementation problems separately.
13. Classify all validation findings.
14. Produce a Foundation feedback report.
15. Decide whether the next step is local iteration, another pilot, candidate clarification, or Foundation review.

This sequence is recommended for validation discipline. It must not be promoted into a universal Manifestation lifecycle.

## 16. Go / No-Go Criteria for Pilot Implementation

Go if:

- the pilot has exactly one primary research question;
- the hypothesis is explicit, provisional, and challengeable;
- the dataset boundary is defined;
- the pilot excludes production trading and platform infrastructure;
- local quantitative terms can be recorded as local extensions;
- the team accepts that Foundation concepts are semantic guides, not workflow gates;
- classification rules are in place before findings are produced;
- no Foundation edits are required before the pilot begins.

No-go or revise if:

- the pilot scope includes VAKI Quant infrastructure;
- the pilot requires live trading, execution, portfolio construction, or capital allocation;
- local domain terms are treated as Foundation concepts at the outset;
- implementation architecture is chosen before the research question is bounded;
- the pilot cannot distinguish Observation from Evidence in its planned records;
- the pilot treats Decision as automated action;
- the pilot requires central approval for local concepts;
- the pilot is designed to prove Foundation adequacy rather than discover failures.

## 17. Final Recommendation

Proceed with a first Manifestation validation pilot, but only under validation guardrails.

The pilot should be a minimal Research Manifestation: one quantitative research question, one explicit hypothesis, one bounded dataset, one controlled investigation, explicit observations, evidence reasoning, one decision recommendation, local design notes, local extension tracking, and a Foundation feedback report.

This is the best first pressure test because it exercises the M1 cognitive semantics and Foundation-Manifestation boundary while remaining small enough to classify failures responsibly.

Do not start M2. Do not implement VAKI Quant. Do not expand the Foundation in advance. Let the pilot create evidence, then decide what that evidence justifies.
