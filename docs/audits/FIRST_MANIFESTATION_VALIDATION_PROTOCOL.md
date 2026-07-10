# First Manifestation Validation Protocol

## 1. Purpose and Scope

This protocol defines the canonical validation contract for the first real VAKI Manifestation pilot.

It exists to make the first pilot falsifiable, bounded, and execution-ready before any pilot work begins. It does not implement the pilot, start M2, expand Foundation semantics, prescribe local technologies, or certify that a Manifestation is Foundation-conformant.

The protocol can establish whether one bounded real Manifestation can use the current Foundation with enough semantic clarity to proceed. It can reveal semantic friction, local extension needs, implementation problems, and possible Foundation review candidates.

The protocol cannot establish universal Foundation validity. One successful pilot does not prove that the Foundation works for all Manifestations, domains, scales, or future uses.

The pilot must test whether the Foundation can guide a bounded real Manifestation while preserving:

- semantic precision;
- domain autonomy;
- explicit interpretation;
- explicit extension;
- separation between Foundation meaning and local implementation;
- non-pipeline inquiry semantics;
- evidence-aware decision reasoning;
- feedback without automatic semantic promotion.

The protocol is a validation scaffold. It is not a new lifecycle model, compliance framework, maturity model, governance process, schema, repository template, or implementation architecture.

## 2. Pilot Boundary

The recommended pilot boundary follows the discovery report:

```text
Discovery and validation of one bounded quantitative hypothesis on one defined
dataset or bounded dataset slice.
```

The pilot enters scope only when it includes:

- one primary research Question;
- one explicit, provisional, challengeable Hypothesis;
- one bounded dataset or dataset slice;
- one Experiment or controlled investigation that creates or selects conditions for possible Observation;
- Observation records with provenance, selection boundaries, scope, and limits;
- Evidence assessment that states what the observations bear on and how uncertainty changes;
- one Decision recommendation or outcome under uncertainty;
- local Design and implementation decisions only where needed to make the pilot coherent;
- concept classification for significant local terms and structures;
- semantic friction logging;
- a final validation report.

The pilot explicitly excludes:

- live trading;
- capital allocation;
- broker, exchange, or execution integration;
- portfolio construction;
- risk engines;
- production market data infrastructure;
- generalized backtesting platforms;
- distributed orchestration;
- production observability;
- full VAKI Quant architecture;
- reusable quantitative research framework construction;
- Foundation document edits during execution;
- M2 planning or implementation.

Domain assumptions may remain local when they concern quantitative research method, dataset choice, sampling boundary, measurement convention, statistical approach, benchmark selection, hypothesis-generation practice, or local vocabulary. They must be visible when they affect interpretation, evidence, uncertainty, decision, or claims of Foundation alignment.

Implementation freedom remains unrestricted. The pilot may choose its own programming language, tools, notebooks, scripts, data formats, storage, statistical method, repository structure, execution style, visualization, and local artifact format. The only restriction is semantic honesty: implementation choices must not silently redefine Foundation meanings.

The pilot is narrow enough only if failures can be attributed meaningfully to one of these sources:

- Foundation semantic issue;
- local interpretation issue;
- domain extension need;
- implementation problem;
- scope control failure;
- evidence or observation quality failure.

## 3. Foundation Surfaces Under Validation

| Foundation surface | Useful guidance | Ambiguity signal | Excessive prescription signal | Missing ownership signal | Evidence to preserve |
|---|---|---|---|---|---|
| Principles | Principles guide scope, assumptions, evidence, autonomy, reversibility, and documentation without dictating implementation | Multiple principles appear to require incompatible local behavior | A principle is treated as requiring a specific method, tool, or process | A recurring cross-domain principle is needed but has no home | Which principles were used, how they shaped decisions, and where they created friction |
| Foundation-Manifestation relationship | Foundation meanings are inherited and interpreted locally while local extensions remain visible | Interpretation, extension, implementation choice, divergence, and silent redefinition are hard to distinguish | Foundation is treated as approving tools, layouts, or research methods | A needed boundary category cannot be classified using Foundation Specification or ADR-0001 | Interpretation map, concept ledger, extension register, divergence candidates |
| Question and Inquiry | A domain Question orients inquiry without becoming Hypothesis, uncertainty, evidence gap, or decision situation | Question scope, purpose, or relation to Inquiry cannot be stabilized | Question records become mandatory workflow gates unrelated to risk | A real inquiry relation cannot be represented by current Question/Inquiry semantics | Question record, Inquiry Context, evolution notes, unresolved or suspended aspects |
| Hypothesis | The local Hypothesis remains provisional, challengeable, and domain-specific | Hypothesis blurs with assumption, model, trading rule, answer, or parameter configuration | Every inquiry is forced to create a Hypothesis | A challengeable claim cannot be represented without new Foundation meaning | Hypothesis record, assumptions, possible weakening observations, relation to Question |
| Experiment | Experiment is an inquiry arrangement or controlled interaction, not merely software execution | Experiment, validation, prototype, and result are confused | Protocol appears to dictate experiment method, statistic, or runner | A legitimate reality-facing investigation cannot fit Experiment semantics | Experiment design, conditions, dataset boundary, intended possible observations |
| Observation | Dataset-derived records preserve what was measured or detected before stronger interpretation | Data, measurement, observation, signal, and conclusion blur | Observation format is treated as canonically required | Important observation provenance or boundary cannot be represented | Observation records, provenance, scope, selection, detection limits, corrections |
| Evidence | Evidence is relational, contextual, and changes uncertainty without becoming data, signal, or conclusion | Evidence relation to Question, Hypothesis, uncertainty, or Decision is unclear | Evidence is reduced to a mandatory score or threshold | A necessary evidential relation has no owner | Evidence assessment, body of evidence, quality dimensions, alternatives, uncertainty changes |
| Decision | Decision reasoning consumes evidence without becoming deterministic rule execution | Decision, action, choice, signal, and recommendation blur | A universal decision template, score, or approval workflow appears required | A commitment-relevant concept cannot be handled by Decision Model | Decision object, options, body of evidence, uncertainty, consequences, reversibility, commitment, review conditions |
| Design Methodology | Design guidance keeps the pilot small, observable, and evidence-shaped while implementation remains local | Design is confused with architecture only, or with the whole research process | Methodology is treated as a required linear lifecycle | A domain-independent design concern cannot be expressed | Design notes, scope decisions, implementation choices with rationale where material |
| Feedback and reopening rules | Pilot feedback is converted into observations, classified, and reviewed without automatic Foundation change | Feedback, friction, Foundation defect, and local preference blur | Any friction triggers central review or immediate Foundation edits | Repeated serious friction cannot be classified under closure criteria | Semantic friction log, final validation report, classification of findings, reopening assessment |

## 4. Pre-Registered Validation Questions

The pilot must answer these questions after execution. They must be frozen before execution begins.

1. Can a domain Question be formed without redefining canonical Question semantics?
2. Can Inquiry remain directed and revisable without becoming a mandatory research workflow?
3. Can a local Hypothesis remain domain-specific while preserving Foundation Hypothesis meaning?
4. Can the pilot distinguish Hypothesis from assumption, model, parameter setting, trading rule, and answer?
5. Can an Experiment create or select conditions for possible Observation without being modeled as an Evidence-producing pipeline?
6. Can the Experiment remain distinguishable from software execution, validation, prototype, and result?
7. Can Observation provenance, selection boundaries, measurement limits, and corrections be represented adequately?
8. Can Data, Observation, Signal, Evidence, Knowledge, and Decision remain distinguishable in the pilot records?
9. Can Evidence change uncertainty without becoming synonymous with data, signal, metric, result, conclusion, or proof?
10. Can inconclusive, qualifying, contradicting, or negative evidence be preserved without being treated as pilot failure?
11. Can Decision reasoning consume evidence without collapsing into deterministic rule execution, confidence threshold, or automated action?
12. Can Commitment remain bounded by evidence, uncertainty, consequences, reversibility, optionality, and cost of delay?
13. Can domain-specific concepts be classified without premature Foundation expansion?
14. Can local Design decisions remain autonomous while still being traceable to Foundation reasoning?
15. Can semantic friction be preserved as evidence for review without modifying Foundation documents during execution?
16. Can the final report distinguish Foundation defects from local interpretation errors, implementation problems, and domain extensions?

## 5. Concept Classification Protocol

Every significant concept introduced during the pilot must be classified before it is used in a way that affects interpretation, evidence, decision, extension, or Foundation feedback.

Significant means the concept changes how the pilot frames the Question, states the Hypothesis, designs the Experiment, records Observation, interprets Evidence, makes a Decision, defines scope, names a domain extension, or claims Foundation alignment.

| Classification | Meaning | Admissibility | Required documentation | Foundation modification permitted? | M1 reopening may be considered? |
|---|---|---|---|---|---|
| Foundation-owned concept | A concept already owned by a canonical Foundation document | Always admissible when used according to its owner | Reference owner and preserve canonical meaning | No during pilot | No, unless use exposes contradiction or ownership failure |
| Foundation interpretation | Local explanation of Foundation meaning in the quantitative research context | Admissible when canonical meaning is preserved | Interpretation map: concept, owner, local interpretation, assumptions, boundary | No during pilot | Only if repeated ambiguity cannot be resolved by owner |
| Domain extension | Local quantitative research concept not owned by Foundation | Admissible when visibly local and not presented as Foundation meaning | Extension register: term, local meaning, why needed, relation to Foundation concepts | No during pilot | Not from one use; consider only after cross-context evidence |
| Implementation concept | Tooling, code, data handling, storage, orchestration, method, or architecture construct | Admissible as local implementation | Implementation note only if semantically material | No | No, unless implementation exposes genuine semantic ownership gap |
| Operational artifact | Local record, output, report, metric, notebook, run result, chart, or file used by the pilot | Admissible when not confused with Foundation semantics | Artifact index or local note when needed for traceability | No | No |
| Explicit divergence candidate | A visible departure from inherited Foundation meaning that may be temporary, bounded, or domain-required | Admissible only if named before it affects claims of alignment | Divergence note: canonical meaning, local departure, reason, scope, risk, affected records | No during pilot | Yes, only after post-pilot review if existing semantics cannot absorb it |
| Unresolved ownership question | A concept appears domain-independent or cross-cutting but no canonical owner is clear | Admissible only as quarantined friction, not as local redefinition | Friction log entry and final review classification | No during pilot | Yes, if evidence meets M1 closure reopening criteria |

Classification procedure:

1. Name the concept in local language.
2. Check whether the Glossary or an owning document already defines it.
3. If Foundation-owned, reference the owner and use the canonical meaning.
4. If local, decide whether it is interpretation, domain extension, implementation concept, or operational artifact.
5. If the local use changes canonical meaning, mark it as explicit divergence candidate.
6. If ownership cannot be determined, mark it as unresolved ownership question.
7. Record the classification before relying on the concept for evidence or decision reasoning.
8. Reclassify only by preserving the reason for the change.

This protocol does not create promotion machinery. A concept classified as useful, repeated, or important remains local unless a later deliberate Foundation review decides otherwise.

## 6. Validation Artifacts

The pilot must produce minimal semantic and traceability artifacts. Formats are local. The protocol does not prescribe technology, serialization, programming language, database, workflow engine, or repository structure.

Required artifacts:

| Artifact | Required content | Purpose |
|---|---|---|
| Pilot scope declaration | Pilot question, dataset boundary, exclusions, Foundation reference state, stop conditions | Prevents scope drift and preserves attribution |
| Domain interpretation map | Foundation surfaces used, owner references, local interpretations, assumptions, boundaries | Tests interpretation without redefinition |
| Concept classification ledger | Significant concepts and their classifications | Prevents automatic promotion and silent drift |
| Question record | Question, Inquiry Context, purpose, scope, assumptions, relation to uncertainty and decision relevance | Tests Question and Inquiry semantics |
| Hypothesis record | Provisional claim, conditions, assumptions, challengeability, possible supporting or weakening observations | Tests Hypothesis boundary |
| Experiment design record | Inquiry relation, conditions arranged or selected, dataset boundary, expected possible observations, limits | Tests Experiment boundary |
| Observation record | What was observed, provenance, selection boundary, measurement context, known limits, corrections | Tests Observation semantics |
| Evidence assessment | Evidence relation, body of evidence, support/contradiction/qualification/inconclusive status, uncertainty change, contextual validity | Tests Evidence semantics |
| Decision record | Decision situation, decision object, options, evidence, uncertainty, consequences, reversibility, optionality, cost of delay, commitment, review conditions | Tests Decision semantics |
| Design/implementation decision notes | Local design or implementation decisions where losing reasoning would affect interpretation, evidence, or decision | Tests Design Methodology without prescribing architecture |
| Semantic friction log | Ambiguity, insufficiency, overbreadth, restrictiveness, terminology conflict, ownership uncertainty | Preserves review evidence without changing Foundation |
| Final validation report | Answers to pre-registered questions, artifact summary, finding classifications, exit classification, recommended next step | Converts pilot output into reviewable validation evidence |

Optional implementation artifacts:

- scripts;
- notebooks;
- charts;
- dataset manifests;
- run logs;
- local schemas;
- statistical outputs;
- environment notes;
- reproducibility instructions;
- visualizations.

Optional implementation artifacts become semantically relevant only when needed to inspect Observation, Evidence, Decision, or implementation-failure classification.

## 7. Semantic Friction Logging

The pilot must record semantic friction when any of the following occurs:

- Foundation terminology seems insufficient for a needed meaning;
- multiple canonical interpretations appear plausible;
- Foundation wording seems too broad for responsible local use;
- Foundation wording seems too restrictive for legitimate local use;
- local terminology conflicts with canonical terminology;
- a domain concept appears recurrently useful but has no clear owner;
- a local implementation choice is mistaken for a semantic requirement;
- a local concept appears to require central approval;
- a Foundation concept is difficult to preserve without hidden assumptions;
- an explicit divergence candidate appears.

Each friction entry must preserve:

- friction identifier;
- date or pilot phase;
- affected Foundation surface;
- local context;
- exact concept or wording at issue;
- observed difficulty;
- classification candidate;
- whether pilot execution is blocked;
- local mitigation used;
- evidence needed for post-pilot review;
- whether the issue is quarantined for Foundation review.

The friction log is evidence, not a change request. It must not automatically trigger Foundation modification, M1 reopening, or local canonization.

## 8. Failure Signal Taxonomy

| Failure signal | Meaning | Expected response |
|---|---|---|
| Pilot implementation failure | Code, data handling, tooling, environment, performance, or local architecture prevents execution | Fix locally or classify as pilot failure unrelated to Foundation; do not reopen M1 |
| Poor local interpretation | Pilot misuses a Foundation concept despite clear canonical ownership | Correct local interpretation; record in friction log only if likely to recur |
| Accidental semantic drift | Local use gradually changes Foundation meaning without naming divergence | Pause affected work, classify concept, repair records, and decide whether divergence is explicit |
| Excessive Foundation prescription | Pilot treats Foundation as requiring a tool, method, format, workflow, or architecture | Remove prescription, restore local autonomy, record source of pressure |
| Ambiguous canonical semantics | Current Foundation wording supports multiple plausible interpretations in legitimate use | Log friction, continue only with explicit local interpretation, evaluate post-pilot |
| Missing canonical ownership | A domain-independent concept required for legitimate use has no coherent owner | Quarantine as unresolved ownership question; continue only if local workaround is honest |
| Premature local abstraction | A local concept is generalized before evidence shows cross-domain need | Keep local, mark as domain extension or implementation concept, block promotion |
| Legitimate domain divergence | Domain conditions require a visible departure from inherited meaning | Record explicit divergence candidate, bound its scope, avoid claiming unchanged alignment |
| Evidence trace failure | Observations, evidence, or decisions cannot be traced enough for review | Pause; repair trace if possible; terminate if irrecoverable |
| Scope attribution failure | Pilot expands until failures cannot be attributed meaningfully | Pause and reduce scope; terminate if attribution cannot be restored |

Not every failure should reopen M1. M1 reopening is considered only when post-pilot evidence demonstrates a concrete semantic ownership gap, conflicting canonical interpretation, recurrent cross-domain fragmentation, incoherent distributed capability, or inability of existing owners to absorb clarification without distortion.

## 9. Guardrails During Execution

During pilot execution:

- no Foundation semantic documents may be edited to help the pilot proceed;
- no success criteria may be redefined after observing pilot results;
- no local concept may be promoted merely because it is useful once;
- no implementation difficulty may be treated as proof of Foundation failure without semantic evidence;
- no repeated Foundation ambiguity may be dismissed as implementation friction without review evidence;
- no local interpretation may silently replace canonical meaning;
- no domain extension may be presented as Foundation-owned;
- no pilot artifact format may be treated as a universal Foundation requirement;
- no pilot result may certify universal Foundation validity;
- no M2 planning may be attached to pilot execution.

Possible Foundation-change observations must be quarantined:

1. Record the issue in the semantic friction log.
2. Continue with an explicit local interpretation or bounded divergence only if honest execution remains possible.
3. Do not edit Foundation documents during pilot execution.
4. Include the issue in the final validation report.
5. Evaluate it only during the post-pilot decision procedure.

## 10. Go / No-Go Entry Criteria

The pilot may begin only when all entry criteria are satisfied.

Go criteria:

- scope is bounded to one primary research Question, one Hypothesis, one dataset or dataset slice, and one controlled investigation;
- validation questions are frozen;
- required Foundation surfaces are identified;
- Foundation reference state is recorded;
- required artifacts are known;
- concept classification rules are explicit;
- semantic friction log structure is ready;
- stop conditions are defined;
- exclusions are accepted;
- implementation freedom is confirmed;
- no Foundation edits are required before execution;
- pilot owner accepts that the goal is failure discovery, not proof of Foundation adequacy.

No-go criteria:

- the pilot includes production Quant architecture;
- the pilot requires live trading or capital allocation;
- scope cannot be bounded enough for attribution;
- required artifacts are rejected as too burdensome or too vague to preserve meaning;
- local concepts are assumed to be Foundation candidates before execution;
- validation questions remain negotiable after results;
- Foundation semantic edits are requested as a precondition;
- Observation and Evidence cannot be represented separately in the planned records;
- Decision is planned as rule execution rather than commitment reasoning.

## 11. Stop Conditions

Pause the pilot when:

- scope expands enough to threaten attribution;
- local concepts begin to appear as Foundation concepts;
- semantic drift is detected;
- canonical ambiguity blocks honest interpretation;
- observation provenance is incomplete but repairable;
- evidence assessment becomes detached from the Question, Hypothesis, uncertainty, or Decision;
- implementation difficulty is being argued as Foundation failure without classification;
- success criteria are being renegotiated after results.

Terminate the pilot when:

- scope expansion cannot be reversed;
- the pilot becomes a full VAKI Quant architecture project;
- canonical ambiguity prevents meaningful interpretation and no bounded local interpretation is possible;
- implementation records have silently redefined Foundation concepts and cannot be repaired;
- evidence collection becomes invalid or irrecoverably untraceable;
- the dataset boundary becomes unknowable or materially changes without trace;
- the final validation questions can no longer be answered from preserved evidence.

Termination may still produce useful negative knowledge. It should be classified rather than hidden.

## 12. Exit Criteria

| Exit classification | Criteria |
|---|---|
| Validation success | All pre-registered questions can be answered; Foundation meanings remained distinguishable; local concepts were classified; evidence and decision reasoning are traceable; no blocking semantic defect appears |
| Validation success with non-blocking friction | Pilot completes and answers questions, but friction log contains candidate clarifications, local interpretation problems, or domain extension pressure that do not block use |
| Inconclusive result | Pilot completes partially or produces insufficient evidence to answer key validation questions, without proving Foundation inadequacy |
| Foundation review required | Evidence indicates ambiguous canonical semantics, missing ownership, excessive prescription, or boundary failure that existing local interpretation cannot responsibly resolve |
| M1 reopening candidate | Evidence meets M1 closure reopening criteria: concrete ownership gap, conflicting canonical interpretation, recurrent or strongly evidenced cross-domain fragmentation, incoherent distributed capability, or inability of existing owners to absorb clarification |
| Pilot failure unrelated to Foundation adequacy | Failure is attributable to implementation, dataset access, tooling, local design, scope control, or invalid evidence collection rather than Foundation semantics |

No exit classification may automatically modify Foundation documents.

## 13. Post-Pilot Decision Procedure

After execution, use this sequence:

1. Assess the pilot result against the frozen scope, stop conditions, and exit criteria.
2. Review the semantic friction log.
3. Classify all findings as Foundation-owned use, Foundation interpretation, domain extension, implementation concept, operational artifact, explicit divergence candidate, unresolved ownership question, local interpretation issue, implementation problem, or probable Foundation defect.
4. Determine local corrections needed in the Manifestation.
5. Determine whether any finding should become a candidate Foundation clarification.
6. Evaluate any serious finding against M1 reopening criteria.
7. Make an explicit decision before any Foundation semantic modification.
8. If Foundation review is opened, preserve the pilot evidence and the exact classification path that led to review.

The pilot itself never modifies canonical Foundation semantics.

## 14. Repository Integration Recommendation

Minimum repository integration is:

- keep this protocol in `docs/audits/` as validation governance for the first pilot;
- add a README link only if the repository wants root-level discoverability for pre-pilot validation materials;
- avoid broad restructuring, new directories, schemas, or artifact templates;
- do not add this protocol to canonical semantic owner lists as if it defines new Foundation concepts;
- reference it from future pilot planning documents rather than embedding its rules into Foundation semantic documents.

Focused consistency review:

- Consistent with `M1_CLOSURE_REPORT.md`: the protocol does not reopen M1, add M1.6, or introduce new cognitive owners; it uses Manifestation experience as evidence for future review.
- Consistent with `FIRST_MANIFESTATION_VALIDATION_DISCOVERY.md`: the protocol operationalizes the `READY WITH VALIDATION GUARDRAILS` verdict and preserves the recommended quantitative research pilot boundary.
- Consistent with `FOUNDATION_SPEC.md`: the protocol preserves Foundation ownership, Manifestation autonomy, explicit interpretation, local extension, implementation freedom, explicit divergence, and no automatic promotion.
- Consistent with canonical Thinking documents: the protocol preserves non-pipeline topology and keeps Question, Hypothesis, Experiment, Observation, Evidence, and Decision under their existing owners.

## 15. Protocol Verdict

READY FOR FIRST PILOT EXECUTION AFTER ENTRY CRITERIA ARE MET.

The protocol is strict enough to make the first Manifestation pilot capable of falsifying Foundation usability, but lightweight enough to avoid turning validation into bureaucracy or implementation prescription.

The next step is to prepare the pilot scope declaration and freeze the pre-registered validation questions before any Manifestation implementation begins.
