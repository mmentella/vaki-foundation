# M1.2 Observation-Evidence Boundary Audit

## 1. Scope

This audit reviews the boundary between:

- `docs/thinking/OBSERVATION_MODEL.md`
- `docs/thinking/EVIDENCE.md`

Reference documents consulted for coherence:

- `docs/thinking/README.md`
- `docs/method/DECISION_MODEL.md`
- `docs/method/DESIGN_METHODOLOGY.md`
- `docs/GLOSSARY.md`
- `docs/philosophy/PRINCIPLES.md`
- `decisions/ADR-0001-foundation-manifestation-boundary.md`

This audit does not modify the Observation Model or Evidence Model. It identifies what should remain as boundary language, what should be shortened or referenced, and what semantic ownership should guide a later refactoring pass.

## 2. Executive Assessment

The Observation-Evidence boundary is **coherent with targeted corrections**.

`OBSERVATION_MODEL.md` now clearly owns observation semantics. `EVIDENCE.md` still contains deep observation-side definitions because it was written before the Observation Model existed. These definitions are mostly compatible, not contradictory. The main correction needed is refactoring ownership: Evidence Model should retain minimal boundary language and reference Observation Model for deeper observation semantics.

No critical architectural inconsistency was found.

## 3. Current Boundary Architecture

The current documents express this architecture:

```text
Interaction with Reality
  -> Data, perception, measurement, experience, or detection
  -> Observation
  -> possible Signal
  -> Evidence relation
  -> changed state of uncertainty
```

`OBSERVATION_MODEL.md` defines observation as a reality-constrained, selective, contextual, preservable account of something perceived, measured, experienced, or detected.

`EVIDENCE.md` defines evidence as relational information that changes the credibility of a claim, hypothesis, model, uncertainty, or decision.

The transition is coherent:

- observation preserves what was encountered and under what conditions;
- signal marks possible relevance;
- evidence exists when information bears on something under consideration;
- interpretation establishes evidential relevance and changes uncertainty.

The main redundancy is that `EVIDENCE.md` still performs detailed observation work in its `Data`, `Observation`, `Supporting, Contradicting, Absent, and Inconclusive Evidence`, and traceability sections.

## 4. Responsibility Map

| Concept | Observation Model Responsibility | Evidence Model Responsibility | Current Overlap | Recommended Ownership |
|---|---|---|---|---|
| Observation | Primary definition, context, selection, preservation, limits | Boundary reference and source for evidence | Ownership duplication | Observation Model |
| Data | Boundary with observation; no full Data Model | Current local definition and observation transition | Benign overlap with ownership ambiguity | Evidence may keep short boundary; no new owner needed |
| Measurement | Measurement as possible observation source, not truth | Measurement quality as evidence interpretation factor | Boundary duplication | Observation owns measurement-observation; Evidence owns evidence use |
| Interpretation | Observation-side distinction from description/inference | Evidence-facing interpretation and synthesis | Benign overlap | Layered ownership |
| Observation Context | Conditions needed to understand observation | Evidence context used for relevance and interpretation | Ownership duplication in older Evidence language | Observation Model |
| Provenance | Origin-side provenance | Provenance as input to evidential relevance/quality | Boundary duplication | Layered ownership |
| Signal | Boundary reference only | Possible relevance layer between observation and evidence | Minimal overlap | Evidence Model |
| Evidence | Out of scope except boundary | Primary definition and relation to objects of evaluation | None | Evidence Model |
| Evidence Strength | Explicitly out of scope | Multidimensional evidence quality/strength | None | Evidence Model |
| Observation Quality | Multidimensional observation-side quality | May affect evidence quality but not equivalent | Boundary duplication risk | Observation Model |
| Contextual Validity | Not owner | Validity horizon of evidence | Low overlap | Evidence Model |
| State of Uncertainty | Not owner | Changed by evidence; used by decision reasoning | None | Evidence Model |
| Correction | Observation correction | Evidence revision when meaning changes | Benign overlap | Layered ownership |
| Revision | Observation correction boundary | Evidence, interpretation, knowledge revision | Benign overlap | Layered ownership |
| Supersession | Mentions better observation account | Evidence supersession and historical rationality | Minor wording risk | Evidence Model for supersession |
| Feedback | Feedback-to-observation boundary | Evidence from operational feedback when related to object | Low overlap | Observation owns conversion; Evidence owns relevance |
| Traceability | Origin-side and forward observation trace | Evidence relationship trace | Boundary duplication | Layered ownership |

## 5. Required Boundary Duplication

The following language should remain in both documents in some form:

- observation is not automatically evidence;
- measurement is not automatically observation or evidence;
- signal is possible relevance, not evidence;
- evidence is relational;
- observation context and provenance matter to evidence interpretation;
- absence of observation is not automatically evidence of absence;
- feedback must become observation before it can support evidence reasoning;
- traceability should connect decision, evidence, observation, and origin context.

This repetition is useful boundary duplication. It lets each document remain understandable without forcing the reader through every model.

## 6. Ownership Duplication

`EVIDENCE.md` currently contains deep ownership-level observation semantics in:

- `## 5. Data`
- `## 6. Observation`
- parts of `## 14. Supporting, Contradicting, Absent, and Inconclusive Evidence`
- parts of `## 18. Traceability`

These are compatible with the Observation Model, but they should no longer be primary definitions. In a later refactor, they should be shortened and explicitly reference `OBSERVATION_MODEL.md`.

## 7. Reference Candidates

| Current Section | Current Semantic Responsibility | Preferred Owner | Minimal Boundary Language to Retain |
|---|---|---|---|
| Evidence `## 3. Epistemic Layers` | Defines data-observation-signal-evidence distinctions | Shared boundary, with Observation semantics owned by Observation Model | Keep layer distinctions and non-pipeline warning; reference Observation Model for observation semantics. |
| Evidence `## 5. Data` | Defines data and data-observation transition | Observation Model for observation boundary; Evidence Model may keep data as pre-evidence role | Shorten to "data may become observation when contextualized as defined by Observation Model." |
| Evidence `## 6. Observation` | Deep definition of observation, context, limits | Observation Model | Replace most content with reference; keep "Evidence uses observations but does not own observation semantics." |
| Evidence `## 7. Signal` | Defines signal | Evidence Model | Retain. Maybe mention Observation Model owns observation, Signal is possible relevance. |
| Evidence `## 8. Evidence` | Defines relational evidence | Evidence Model | Retain. |
| Evidence `## 9. Interpretation` | Defines evidence-facing interpretation | Evidence Model | Retain, but avoid wording that could imply ownership of observation-side interpretation. |
| Evidence `## 14. Supporting, Contradicting, Absent, and Inconclusive Evidence` | Mixes absence semantics with evidential interpretation | Observation Model for absence/non-observation boundary; Evidence Model for evidential absence | Keep evidence-of-absence logic; reference Observation Model for absence of observation vs observation of absence. |
| Evidence `## 18. Traceability` | Decision -> Evidence -> Observation -> origin trace | Layered | Keep evidence relationship trace; reference Observation Model for origin-side trace. |

## 8. Semantic Conflicts

No semantic conflicts were found.

Differences are differences of depth and ownership, not incompatible meanings. `EVIDENCE.md` defines observation more deeply than it should after creation of `OBSERVATION_MODEL.md`, but its definitions are compatible with the new primary owner.

## 9. Missing Boundary Language

The boundary is mostly complete. Missing or under-emphasized language:

- Evidence Model does not yet explicitly say that Observation Model is the primary owner of observation semantics.
- Evidence Model does not yet distinguish Observation Context from Contextual Validity by name.
- Evidence Model traceability does not yet present the layered ownership model: Observation origin trace, Evidence relationship trace, Decision reasoning trace.
- Evidence Model absence section would benefit from a compact three-layer distinction: no observation exists; observation records absence; observed absence bears evidentially on a claim.

## 10. Traceability Assessment

Origin trace is now owned clearly by Observation Model:

```text
Observation
  -> provenance
  -> interaction, operation, experience, experiment, measurement, or detection context
```

Evidence relationship trace is owned by Evidence Model:

```text
Evidence
  -> Observation or other relevant source
  -> relationship to claim, hypothesis, model, uncertainty, or decision
```

Decision trace is owned by Decision Model:

```text
Decision
  -> Body of Evidence
  -> reasoning context
  -> Commitment
```

The forward trace from Observation to affected evidence and decisions is represented in Observation Model and compatible with Evidence Model, but Evidence Model should later acknowledge this layered structure explicitly.

## 11. Failure-Mode Coverage

The current boundary can recognize the tested collapse errors:

- Observation mistaken for Evidence: recognized by both documents.
- Measurement mistaken for Evidence: recognized by both documents.
- Interpretation mistaken for Observation: recognized strongly by Observation Model and Evidence Model.
- Signal mistaken for Evidence: recognized by Evidence Model.
- Data volume mistaken for Evidence Strength: recognized indirectly through evidence quality and no-score language.
- High observation precision mistaken for strong evidential relevance: recognized by Observation Quality and Evidence Quality separation.
- Poor provenance ignored during Evidence evaluation: recognized by both documents, though ownership should be layered.
- Observation Context mistaken for Contextual Validity: mostly recognizable, but Evidence Model should sharpen this boundary.
- Absence of Observation mistaken for Evidence of Absence: recognized by both documents, but Evidence Model should defer the observation-side distinction.
- Observation correction not propagated to affected Evidence: recognized by Observation traceability, less explicit in Evidence Model.
- Evidence revision incorrectly rewriting original Observation: recognized by Evidence revision/supersession and Observation correction distinction.
- Evidence conflict treated as observation error without justification: recognized by Evidence Model's contradictory evidence section.
- Feedback recorded but not contextualized as Observation: recognized by Observation Model and Thinking Model.
- Observation collected but never connected to a reasoning object: recognized by Signal/Evidence relation boundary.

No tested failure mode exposes a critical boundary failure.

## 12. Domain-Independence Assessment

The boundary remains domain-independent across software, physical machines, vessels, scientific research, quantitative research, markets and trading, products, organizational processes, and infrastructure.

The documents do not require:

- quantitative data;
- human perception only;
- sensors;
- scientific experimentation;
- user feedback;
- metadata systems;
- digital storage;
- source code or logs.

Evidence relation does not depend on formal scientific experimentation. Observation preservation does not require a particular technology.

## 13. Findings

### M1.2-OE-001

ID: M1.2-OE-001  
Severity: MAJOR  
Documents: `docs/thinking/OBSERVATION_MODEL.md`, `docs/thinking/EVIDENCE.md`  
Sections: Evidence `## 6. Observation`; Observation `## 4. Observation`, `## 5. Observation Context`, `## 6. Selection and Boundaries`  
Duplication class: OWNERSHIP DUPLICATION  
Issue: Evidence Model still contains a full observation definition and context/limits language now owned by Observation Model.  
Why it matters: Future manifestations may treat Evidence Model as co-owner of observation semantics, weakening the clean Observation -> Evidence boundary.  
Recommended correction: Shorten Evidence `Observation` to boundary language and reference Observation Model for full semantics.  
Preferred semantic owner: Observation Model  
Dependency: None

### M1.2-OE-002

ID: M1.2-OE-002  
Severity: MINOR  
Documents: `docs/thinking/EVIDENCE.md`, `docs/thinking/OBSERVATION_MODEL.md`  
Sections: Evidence `## 5. Data`; Observation `## 9. Observation and Data`  
Duplication class: REFERENCE CANDIDATE  
Issue: Evidence Model defines Data and the data-observation transition in more detail than needed after Observation Model.  
Why it matters: Data does not have a dedicated model, and too much detail in Evidence may imply Evidence owns the raw-data-to-observation boundary.  
Recommended correction: Retain minimal Data language in Evidence, but refer to Observation Model for when data becomes observation.  
Preferred semantic owner: No separate Data owner; Observation Model owns data-observation boundary.  
Dependency: M1.2-OE-001

### M1.2-OE-003

ID: M1.2-OE-003  
Severity: MINOR  
Documents: `docs/thinking/EVIDENCE.md`, `docs/thinking/OBSERVATION_MODEL.md`  
Sections: Evidence `## 14. Supporting, Contradicting, Absent, and Inconclusive Evidence`; Observation `## 10. Absence and Non-Observation`  
Duplication class: REFERENCE CANDIDATE  
Issue: Evidence Model contains observation-side absence semantics that now belong to Observation Model.  
Why it matters: Absence semantics has three layers: no observation exists; observation records absence; observed absence bears evidentially on a claim. Evidence should own only the third layer.  
Recommended correction: Preserve evidence-of-absence reasoning, but reference Observation Model for absence of observation vs observation of absence.  
Preferred semantic owner: Observation Model for absence/non-observation boundary; Evidence Model for evidential meaning.  
Dependency: M1.2-OE-001

### M1.2-OE-004

ID: M1.2-OE-004  
Severity: MINOR  
Documents: `docs/thinking/EVIDENCE.md`, `docs/thinking/OBSERVATION_MODEL.md`  
Sections: Evidence `## 9. Interpretation`; Observation `## 8. Observation and Interpretation`  
Duplication class: BENIGN OVERLAP  
Issue: Both models discuss interpretation, but at different layers.  
Why it matters: This is appropriate if kept layered: Observation handles selection, description, mediation, and inference boundary; Evidence handles evidential relevance and synthesis.  
Recommended correction: In future Evidence edits, clarify that its interpretation section concerns evidential interpretation, not observation-side mediation.  
Preferred semantic owner: Observation Model for observation-side boundary; Evidence Model for evidential interpretation.  
Dependency: None

### M1.2-OE-005

ID: M1.2-OE-005  
Severity: MINOR  
Documents: `docs/thinking/EVIDENCE.md`, `docs/thinking/OBSERVATION_MODEL.md`  
Sections: Evidence `## 18. Traceability`; Observation `## 17. Traceability`  
Duplication class: BOUNDARY DUPLICATION  
Issue: Both documents describe traces involving observation, provenance, and evidence.  
Why it matters: The overlap is necessary but should remain layered to avoid inventing one universal traceability abstraction.  
Recommended correction: Evidence traceability should preserve decision/evidence relationship trace and reference Observation Model for origin-side trace.  
Preferred semantic owner: Layered ownership.  
Dependency: M1.2-OE-001

### M1.2-OE-006

ID: M1.2-OE-006  
Severity: NOTE  
Documents: `docs/thinking/EVIDENCE.md`, `docs/thinking/OBSERVATION_MODEL.md`  
Sections: Evidence `## 7. Signal`; Observation `## 15. Boundary with Signal and Evidence`  
Duplication class: BOUNDARY DUPLICATION  
Issue: Signal is correctly primary-owned by Evidence Model and referenced by Observation Model as boundary language.  
Why it matters: The relationship "Observation -> possible Signal -> Evidence relation" is useful if it remains non-mandatory.  
Recommended correction: Retain Signal in Evidence. No model change required except avoiding workflow wording in future edits.  
Preferred semantic owner: Evidence Model  
Dependency: None

### M1.2-OE-007

ID: M1.2-OE-007  
Severity: NOTE  
Documents: `docs/thinking/EVIDENCE.md`, `docs/thinking/OBSERVATION_MODEL.md`  
Sections: Evidence `## 13. Evidence Quality`; Observation `## 16. Observation Quality`  
Duplication class: BENIGN OVERLAP  
Issue: Observation Quality and Evidence Quality/Evidence Strength are distinct and currently compatible.  
Why it matters: High observation quality must not imply strong evidential relevance, and imperfect observations may still be evidence within limits.  
Recommended correction: No immediate change. Future Evidence edits may add one sentence clarifying that evidence quality may use but does not equal observation quality.  
Preferred semantic owner: Observation Model for Observation Quality; Evidence Model for Evidence Quality.  
Dependency: None

### M1.2-OE-008

ID: M1.2-OE-008  
Severity: MINOR  
Documents: `docs/thinking/EVIDENCE.md`, `docs/thinking/OBSERVATION_MODEL.md`  
Sections: Evidence `## 17. Evidence Lifetime and Contextual Validity`; Observation `## 5. Observation Context`  
Duplication class: REFERENCE CANDIDATE  
Issue: Observation Context and Contextual Validity are compatible but not explicitly contrasted in Evidence Model.  
Why it matters: Manifestations may confuse conditions needed to understand an observation with the validity horizon of evidential interpretation.  
Recommended correction: Add concise boundary language in Evidence Model: Observation Context is owned by Observation Model; Contextual Validity is evidence-side applicability.  
Preferred semantic owner: Observation Model for Observation Context; Evidence Model for Contextual Validity.  
Dependency: M1.2-OE-001

### M1.2-OE-009

ID: M1.2-OE-009  
Severity: NOTE  
Documents: `docs/thinking/EVIDENCE.md`, `docs/thinking/OBSERVATION_MODEL.md`  
Sections: Evidence `## 15. Contradictory Evidence`; Observation `## 13. Correction and Revision`  
Duplication class: BENIGN OVERLAP  
Issue: Contradictory evidence may involve observation error, but Evidence Model does not collapse conflict into observation correction.  
Why it matters: This preserves contradiction as information while allowing observation correction when warranted.  
Recommended correction: No immediate change.  
Preferred semantic owner: Evidence Model for contradiction; Observation Model for observation correction.  
Dependency: None

## 14. Refactoring Specification

### Changes to OBSERVATION_MODEL.md

No required changes.

Optional future precision only:

- Consider replacing "superseded by a better preserved account" with "replaced by a better preserved account" if future audits find that "supersession" should remain strictly evidence-side. This is not currently a conflict.

### Changes to EVIDENCE.md

#### Section `## 2. Position in the Thinking Model`

Keep:

- Evidence may arise from direct observation, operational feedback, experience, comparison, deliberate experiment, or other interactions with reality.
- Evidence is a boundary layer.

Shorten:

- Any language that implies Evidence Model owns reality-facing observation.

Boundary language to preserve:

- Evidence uses observations and other reality-facing information only when connected to a question, claim, hypothesis, model, uncertainty, or decision.

#### Section `## 3. Epistemic Layers`

Keep:

- Layer distinctions.
- Non-mandatory process warning.
- "A measurement is not automatically an observation. An observation is not automatically a signal. A signal is not automatically evidence."

Replace with reference:

- Add reference that observation semantics are defined in `OBSERVATION_MODEL.md`.

Boundary language to preserve:

- These are roles, not required pipeline states.

#### Section `## 5. Data`

Keep:

- Data can be useful, misleading, incomplete, duplicated, corrupted, stale, biased, or irrelevant.
- Same artifact may participate in several roles.

Shorten:

- Detailed data-to-observation contextualization, provenance, and limitation language.

Replace with reference:

- Reference Observation Model for when data becomes observation.

Boundary language to preserve:

- Data is not automatically observation or evidence.

#### Section `## 6. Observation`

Keep:

- Minimal statement that Evidence Model uses observations as possible sources of evidence.
- Observation is not explanation.
- Observation is not automatically evidence.

Remove after reference:

- Full definition of observation.
- Detailed observation context list.
- Mistaken/incomplete/measurement error/coverage detail, except as a compact boundary reminder.

Replace with reference:

- "Observation semantics are defined in the Observation Model."

Boundary language to preserve:

- Evidence interpretation depends on observation context and limits.

#### Section `## 7. Signal`

Keep:

- Signal as relevance layer.
- Signal is not automatically evidence.
- Connection to observation and possible misleadingness.

Boundary language to preserve:

- Signal remains optional and non-mandatory.

#### Section `## 8. Evidence`

Keep:

- Evidence is relational.
- Same observation may be strong evidence for one claim, weak for another, irrelevant for another.
- Evidential relevance constrained by provenance, conditions, measurement quality, scope, alternatives, and limitations.

No removal needed.

#### Section `## 9. Interpretation`

Keep:

- Evidential interpretation responsibility.

Shorten or clarify:

- If needed, specify that this section concerns evidence-facing interpretation, while Observation Model owns observation-side mediation and description/inference boundary.

#### Section `## 13. Evidence Quality`

Keep:

- Evidence Quality dimensions.
- No universal confidence score.

Boundary language to preserve:

- Evidence Quality may consider observation quality/provenance but is not identical to observation quality.

#### Section `## 14. Supporting, Contradicting, Absent, and Inconclusive Evidence`

Keep:

- Supporting, contradicting, qualifying, null, inconclusive evidence distinctions.
- Evidence-of-absence caution.

Shorten:

- Observation-side absence definitions.

Replace with reference:

- Reference Observation Model for absence of observation versus observation of absence.

Boundary language to preserve:

- Non-observation becomes evidentially meaningful only under detection conditions and interpretive constraints.

#### Section `## 17. Evidence Lifetime and Contextual Validity`

Keep:

- Evidence validity horizon.
- Applicability depends on current question and conditions.

Add boundary language:

- Observation Context is origin-side; Contextual Validity is evidence-side applicability.

#### Section `## 18. Traceability`

Keep:

- Decision -> Evidence -> Observation trace.

Shorten:

- Origin-side provenance details.

Replace with reference:

- Reference Observation Model for origin-side observation trace.

Boundary language to preserve:

- Traceability remains conceptual and non-tooling.

#### Section `## 19. Revision and Supersession`

Keep:

- Evidence, interpretation, and knowledge revision.
- Later evidence may supersede earlier evidence without erasing historical rationality.

Boundary language to preserve:

- Observation correction is distinct from evidence revision.

### Changes to THINKING_MODEL

No required changes. The existing link from Observation section to Observation Model is sufficient.

### Changes to GLOSSARY

Do not apply in this refactor.

Future candidates:

- Observation Context
- Provenance
- Signal boundary refinement, only if repeated misuse appears

## 15. Recommended Refactoring Order

1. Add an Evidence Model reference to Observation Model in `## 3. Epistemic Layers`.  
   This establishes ownership before reducing local content.

2. Shorten Evidence `## 6. Observation`.  
   This is the main ownership correction and should happen before smaller boundary edits.

3. Shorten Evidence `## 5. Data`.  
   This depends on the observation ownership reference.

4. Refine Evidence `## 14. Supporting, Contradicting, Absent, and Inconclusive Evidence`.  
   This should preserve evidence-of-absence reasoning while deferring observation-side absence semantics.

5. Add a small Observation Context vs Contextual Validity distinction in Evidence `## 17`.

6. Layer Evidence `## 18. Traceability` by referencing Observation Model for origin trace.

7. Optionally clarify Evidence `## 9. Interpretation` and `## 13. Evidence Quality` with one boundary sentence each.

No new model or abstraction is required.

## 16. Final Architectural Judgment

1. Observation is now clearly owned by Observation Model?  
   Yes.

2. `EVIDENCE.md` contains deep observation semantics that should be reduced?  
   Yes. Especially `Data`, `Observation`, absence semantics, and traceability origin language.

3. Signal has clear ownership and boundary?  
   Yes. Signal should remain primary-owned by Evidence Model. Observation Model uses it only as boundary language.

4. Interpretation is correctly layered?  
   Yes. Observation Model owns observation-side mediation and inference boundary; Evidence Model owns evidential interpretation. Future wording can make this sharper.

5. Provenance is correctly layered?  
   Yes. Observation Model owns origin-side provenance; Evidence Model uses provenance for evidential interpretation and quality.

6. Observation Quality and Evidence Strength are distinct?  
   Yes.

7. Observation Context and Contextual Validity are distinct?  
   Yes conceptually, but Evidence Model should make the distinction explicit in a later refactor.

8. Correction, Revision, and Supersession are distinct?  
   Yes. Observation correction, evidence revision, and evidence supersession are compatible and separable.

9. Absence semantics is correctly separated between Observation and Evidence?  
   Mostly. Observation Model is clear; Evidence Model should reduce observation-side absence wording and retain evidential interpretation.

10. Traceability is complete from reality interaction to Decision?  
   Yes, through layered traceability across Observation, Evidence, and Decision Models.

11. The boundary can be corrected with targeted refactoring?  
   Yes.

12. Is a new model or abstraction needed?  
   No.
