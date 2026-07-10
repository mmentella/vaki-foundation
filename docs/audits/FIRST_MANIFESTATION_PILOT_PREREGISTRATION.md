# First Manifestation Pilot Preregistration

## 1. Executive Registration Status

ENTRY CRITERIA PARTIALLY MET.

All semantic, scope, validation, classification, success, failure, stop, and freeze criteria are registered in this document. Execution is not ready until the bounded dataset artifact is present with inspectable provenance.

Repository inspection found no existing VAKI Quant research context and no local dataset files in this repository. The pilot therefore selects a real minimal quantitative research case by frozen dataset identity and selection criteria, while preserving dataset artifact availability as the only execution blocker.

## 2. Pilot Identity

Pilot name: First Manifestation Pilot - SPY Short-Horizon Momentum Validation.

Pilot purpose: Test whether VAKI Foundation semantics can guide a bounded real quantitative research Manifestation without becoming prescriptive, losing semantic precision, or promoting local quantitative vocabulary into Foundation meaning.

Pilot type: Minimal quantitative research Manifestation validation pilot.

Validation objective: Exercise Foundation-to-Manifestation interpretation, Question and Inquiry, Hypothesis, Experiment, Observation, Evidence, Decision, Design Methodology, semantic friction logging, and no-automatic-promotion rules through one bounded research investigation.

Bounded domain context: Historical daily market data research on one liquid exchange-traded fund, SPY, using one pre-execution bounded daily price dataset slice. This is not VAKI Quant architecture and must not become a generic research platform.

## 3. Scope Declaration

Inside scope:

- one bounded research problem: whether a simple prior-return condition in SPY daily data is associated with a subsequent short-horizon return pattern in the registered historical slice;
- one Question;
- one primary Hypothesis;
- one bounded dataset slice: SPY daily adjusted close observations from 2015-01-01 through 2019-12-31, subject to provenance requirements in section 8;
- one controlled investigation boundary: compute the registered prior and forward return measurements and compare registered groups;
- one Evidence assessment;
- one resulting Decision recommendation.

Outside scope:

- live trading;
- broker or exchange integration;
- order execution;
- portfolio construction;
- production risk management;
- strategy orchestration;
- deployment architecture;
- large-scale symbolic discovery;
- generic research platform design;
- reusable backtesting framework construction;
- transaction-cost modeling;
- capital allocation;
- hyperparameter search;
- broad market-regime modeling;
- M2 Foundation work;
- Foundation semantic edits.

The scope is narrow enough for semantic friction to be attributed because it contains only one instrument, one time-bounded dataset slice, one fixed Hypothesis, one investigation arrangement, and one Decision recommendation.

## 4. Pilot Domain Selection

Selected case: SPY daily adjusted-close short-horizon momentum relationship.

Reason for selection:

- real quantitative research domain;
- bounded to one widely understood market instrument;
- can use an already available or easily attached archived historical dataset without live execution;
- falsifiable relationship;
- clear Observation provenance requirements;
- produces measurable observations without making metrics synonymous with Evidence;
- permits a genuine Decision recommendation: continue, reject, revise later, collect additional Observation, or stop due to insufficient Evidence;
- avoids production infrastructure.

This repository does not contain an existing VAKI Quant research context or dataset. The selected case is therefore not inherited from an existing local VAKI Quant artifact. This is recorded as a preregistration limitation, not hidden as readiness.

Commercial importance is irrelevant. The case is selected for Foundation validation value.

## 5. Frozen Research Question

Primary Question:

```text
Within the registered SPY daily adjusted-close dataset slice from 2015-01-01
through 2019-12-31, does a positive prior 20-trading-day return correspond to
a meaningfully different subsequent 5-trading-day return distribution than a
non-positive prior 20-trading-day return?
```

Why this is suitable:

- it identifies a domain-specific uncertainty;
- it does not encode the desired answer;
- it is not a task description;
- it is distinct from the Hypothesis;
- it can produce support, contradiction, qualification, or inconclusive Evidence;
- it stresses Data, Observation, Signal, Evidence, uncertainty, and Decision boundaries.

## 6. Frozen Primary Hypothesis

Primary Hypothesis:

```text
In the registered SPY daily adjusted-close dataset slice, observations with a
positive prior 20-trading-day return will have a higher average subsequent
5-trading-day return than observations with a non-positive prior
20-trading-day return.
```

This Hypothesis is provisional, challengeable, domain-specific, and frozen before execution.

Fixed before execution:

- instrument: SPY;
- date slice: 2015-01-01 through 2019-12-31;
- prior-return window: 20 trading days;
- forward-return window: 5 trading days;
- grouping rule: positive prior 20-trading-day return versus non-positive prior 20-trading-day return;
- primary comparison: average subsequent 5-trading-day return between the two groups.

Inherited from prior research context: none found in this repository.

Post-registration adaptation:

- changing windows;
- changing instrument;
- changing date range;
- changing grouping threshold;
- adding filters after inspecting results;
- adding additional hypotheses;
- optimizing parameter values.

Any such change requires a separately registered investigation or must be recorded as a protocol deviation. It cannot be treated as validation of this frozen Hypothesis.

## 7. Experiment Boundary

The Experiment is the controlled investigation arrangement that creates conditions under which relevant Observations may become possible.

Created conditions:

- use only the registered SPY dataset slice;
- compute prior 20-trading-day returns for eligible observation dates;
- compute subsequent 5-trading-day returns for the same eligible dates;
- assign observations to the registered positive and non-positive prior-return groups;
- compare the registered subsequent-return measurements across groups.

Dataset exposed to investigation:

- one SPY daily adjusted-close dataset slice from 2015-01-01 through 2019-12-31;
- rows without enough prior or forward trading days are excluded from eligible observations.

Allowed transformations:

- date parsing and ordering;
- adjusted-close numeric parsing;
- trading-day indexing;
- prior 20-trading-day return calculation;
- subsequent 5-trading-day return calculation;
- group assignment using the frozen threshold;
- descriptive summaries required for Observation records.

Planned comparisons:

- average subsequent 5-trading-day return for positive prior-return observations;
- average subsequent 5-trading-day return for non-positive prior-return observations;
- difference between group averages;
- group counts and missing/excluded row counts;
- optional distribution summaries only to understand Observation context, not to create new hypotheses.

Measurements that may become Observations:

- eligible observation count;
- excluded count and reason;
- prior 20-trading-day return per eligible observation;
- group assignment per eligible observation;
- subsequent 5-trading-day return per eligible observation;
- group-level average subsequent return;
- difference in group averages;
- missingness or data irregularity observations.

Invalidation conditions:

- dataset provenance cannot be established;
- adjusted-close field is unavailable or ambiguous;
- date ordering cannot be trusted;
- duplicate or missing records cannot be resolved without discretionary judgment;
- dataset slice materially differs from the registered boundary;
- leakage is introduced by using post-result information to alter parameters;
- transformations exceed the allowed list.

The Experiment does not produce Evidence by itself. It creates conditions under which Observations may become possible.

## 8. Dataset Boundary and Provenance Requirements

Dataset identity or selection criteria:

- instrument: SPY ETF daily historical price data;
- required fields: date and adjusted close;
- optional fields: open, high, low, close, volume;
- required date slice: 2015-01-01 through 2019-12-31 inclusive;
- required artifact form: a bounded local dataset artifact available before execution, such as CSV or another simple tabular file;
- source: a named historical market data source recorded before execution.

Inclusion rules:

- SPY observations with valid date and adjusted close;
- dates within the registered slice;
- rows with enough prior 20 trading days and subsequent 5 trading days for registered measurements.

Exclusion rules:

- rows outside the registered slice;
- rows with missing or nonnumeric adjusted close;
- rows with duplicate dates unless a deterministic pre-execution rule is recorded;
- rows lacking enough prior or forward trading days for the registered measurement.

Required provenance:

- data source name;
- retrieval or export date;
- file name or artifact identifier;
- field definitions, especially adjusted close;
- timezone or market-calendar assumption if available;
- any known adjustment policy;
- checksum or stable file fingerprint if available.

Known limitations:

- one instrument only;
- one historical period only;
- adjusted close may encode vendor-specific adjustment assumptions;
- no transaction costs, slippage, taxes, or execution constraints;
- no live market data;
- no claim of future tradability;
- no portfolio-level conclusion.

Contamination and leakage risks:

- the generic momentum idea is prior domain knowledge, not discovered from this registered dataset in this task;
- if this exact dataset slice was previously used to choose the 20-day and 5-day windows, that must be recorded before execution;
- if the dataset artifact was inspected for outcomes before execution, the pilot may still run as a semantic validation but the research evidence must be marked contaminated.

Current availability status:

- no dataset artifact is present in this repository at preregistration time;
- execution must not begin until the dataset artifact and provenance record are supplied.

Data availability, Observation creation, and Evidence assessment remain distinct. A dataset being present is not an Observation. A computed measurement is not Evidence until interpreted in relation to the Hypothesis, Question, uncertainty, or Decision.

## 9. Observation Plan

| Observation class | What is being observed | Source | Provenance expectations | Measurement boundary | Contextual limits | Absence/non-observation handling | Invalidation conditions |
|---|---|---|---|---|---|---|---|
| Dataset eligibility | Count and identity of rows eligible for measurement | Registered dataset artifact | Source, slice, file identity, field definitions | Date and adjusted close availability plus window sufficiency | Only this instrument and date slice | Missing eligibility is recorded as excluded, not absence of market behavior | Unknown provenance, ambiguous adjusted close, unresolved duplicates |
| Prior-return condition | Prior 20-trading-day return and group assignment | Allowed transformation on adjusted close | Formula, window, row linkage | Prior window only; no future data | Does not itself imply signal or evidence | Rows lacking prior window are non-observations for this class | Formula or grouping changed after execution |
| Forward-return measurement | Subsequent 5-trading-day return | Allowed transformation on adjusted close | Formula, window, row linkage | Forward window only | Not an outcome of a tradable strategy | Rows lacking forward window are excluded, not treated as negative returns | Formula changed or forward data unavailable |
| Group summary | Average subsequent return by registered group | Computed eligible observations | Group counts and included row identities | Descriptive summary of registered groups | Average may hide distributional variation | Empty group means insufficient Observation, not Evidence of no effect | Group membership changed post-registration |
| Data irregularity | Missing, duplicate, stale, or malformed records | Dataset artifact inspection | Exact affected rows and handling | Data quality only | Data issue is not evidence against Hypothesis by itself | Unobserved irregularity is not evidence of clean data | Irregularity cannot be resolved without discretionary judgment |

The Observation plan does not decide what observations mean evidentially. Measurements are not Evidence merely because they are computed.

## 10. Evidence Assessment Plan

Evidence will be assessed by interpreting registered Observations in relation to the frozen Hypothesis.

Potentially supporting pattern:

- positive prior-return group has a higher average subsequent 5-trading-day return than the non-positive prior-return group;
- the difference is not wholly explained by obvious data irregularity, extreme missingness, or invalid measurement context;
- remaining uncertainty is explicitly preserved.

Potentially challenging pattern:

- positive prior-return group has equal or lower average subsequent 5-trading-day return than the non-positive group;
- group comparison is dominated by invalid measurement context or contamination;
- results contradict the expected direction under registered conditions.

Ambiguous pattern:

- difference exists but is very small relative to data quality limits;
- group counts are highly imbalanced;
- data irregularities affect comparability;
- results are sensitive to assumptions that were not part of the registered Hypothesis;
- observations support a narrower claim than the Hypothesis states.

Insufficient pattern:

- dataset provenance missing;
- too few eligible observations;
- adjusted close unavailable or ambiguous;
- exclusion rate makes the observation set unrepresentative for this registered slice;
- leakage or contamination prevents responsible interpretation.

Contextual limitations:

- one instrument;
- one date slice;
- no out-of-sample claim beyond registered period;
- no execution realism;
- no transaction costs;
- no portfolio inference;
- no claim of causal mechanism;
- no claim that a tradable strategy exists.

Uncertainty that remains after assessment:

- transferability to other instruments or periods;
- robustness to different windows;
- sensitivity to source adjustments;
- relevance to executable strategy design;
- whether any observed relation is stable, accidental, or proxy-specific.

Evidence must not be reduced to a single score. Quantitative metrics participate in Evidence assessment, but Evidence remains the interpreted relation between Observations and the Hypothesis, Question, uncertainty, or Decision.

## 11. Decision Boundary

The pilot informs one narrow Decision recommendation:

```text
What commitment, if any, is justified after this pilot regarding further
investigation of the registered SPY short-horizon momentum Hypothesis?
```

Decision space:

- continue investigation with a separately registered follow-up;
- reject the Hypothesis for this dataset slice;
- revise the Hypothesis in a future investigation;
- collect additional Observation before deciding;
- do not proceed based on insufficient Evidence;
- record negative knowledge and stop.

The outcome is not pre-registered. Only the decision space and reasoning requirements are frozen.

Decision reasoning must preserve:

- decision object;
- options considered;
- body of evidence;
- uncertainty remaining;
- consequence of being wrong;
- reversibility;
- learning value;
- cost of delay if relevant;
- bounded commitment;
- review conditions.

The Decision must not become deterministic rule execution, trading action, or confidence threshold.

## 12. Pre-Registered Validation Questions

Foundation-Manifestation:

1. Was canonical meaning preserved?
2. Were local interpretations explicit?
3. Did implementation autonomy remain intact?
4. Were domain extensions distinguishable from Foundation meaning?

Question and Inquiry:

5. Could the domain uncertainty be expressed without redefining Question semantics?
6. Did inquiry remain non-pipeline and revisable?

Hypothesis:

7. Could the Hypothesis remain provisional and challengeable?
8. Was it kept distinct from Experiment, Evidence, and conclusion?

Experiment:

9. Could the Experiment be modeled as condition creation for possible Observation rather than as an Evidence-producing machine?

Observation:

10. Could provenance, boundaries, context, limitations, and absence be represented adequately?

Evidence:

11. Could Evidence be assessed as a relation affecting uncertainty rather than as raw data, signal, metric, or conclusion?

Decision:

12. Could the Decision consume Evidence and uncertainty without collapsing into deterministic rule execution?

Design Methodology:

13. Could implementation and design decisions remain locally autonomous while being traceable to reasoning?

Feedback:

14. Could semantic friction be preserved without automatic Foundation modification?

These questions are frozen before execution.

## 13. Foundation Surface Validation Matrix

| Foundation surface | Expected useful guidance | Evidence to preserve | Ambiguity signal | Excessive-prescription signal | Missing-ownership signal |
|---|---|---|---|---|---|
| Principles | Guide explicit assumptions, reality contact, evidence proportionality, negative knowledge, reversibility, and documentation | Principle references in records and friction notes | Principles appear to conflict in local use | Principles are treated as requiring a method or tool | A needed cross-domain principle has no home |
| Foundation-Manifestation relationship | Keep Foundation meaning, local interpretation, local extension, implementation choice, and divergence separate | Interpretation map and concept ledger | Boundary categories blur | Foundation approval appears required for local choices | Boundary case cannot be classified |
| Question and Inquiry | Keep the research Question explicit, bounded, and revisable | Question record and Inquiry Context | Question becomes Hypothesis or task | Question artifact treated as process gate | Inquiry relation cannot be represented |
| Hypothesis | Keep the claim provisional and challengeable | Hypothesis record and deviation log | Hypothesis becomes parameter set or answer | Every inquiry forced into hypothesis form | Challengeable claim lacks semantic home |
| Experiment | Treat investigation as condition creation for possible Observation | Experiment record and allowed transformations | Experiment confused with result or Evidence | Tooling or runner appears prescribed | Legitimate investigation does not fit Experiment semantics |
| Observation | Preserve what was measured or detected with context | Observation records and provenance | Data, measurement, Observation, Signal blur | Required observation format appears canonical | Provenance or absence boundary lacks owner |
| Evidence | Interpret observations relationally and preserve uncertainty | Evidence assessment and uncertainty notes | Metric becomes Evidence by itself | Score or threshold appears mandatory | Evidential relation lacks owner |
| Decision | Convert evidence and uncertainty into bounded recommendation | Decision record | Decision becomes action or rule | Universal decision template appears required | Commitment-relevant concept lacks owner |
| Design Methodology | Keep design small, observable, and locally autonomous | Design notes | Design reduced to architecture only | Methodology treated as lifecycle | Design concern lacks semantic home |
| Feedback and reopening | Preserve friction and post-pilot review path | Friction log and final report | Friction becomes immediate change request | Any issue triggers Foundation edit | Repeated serious issue cannot be classified |

## 14. Initial Domain Interpretation Map

| Foundation concept | Expected pilot appearance | Local interpretation | Redefinition? |
|---|---|---|---|
| Question | Registered SPY momentum research Question | Domain-specific orientation toward insufficient understanding | No |
| Inquiry | Directed investigation of the Question through one controlled comparison | Research activity may revise understanding but not the preregistered Question history | No |
| Hypothesis | Frozen claim about prior 20-day positive return and subsequent 5-day average return | Domain claim exposed to Observation and Evidence | No |
| Experiment | Controlled arrangement using the registered dataset slice and transformations | Condition creation for possible Observation, not proof | No |
| Observation | Preserved computed measurements and data-quality records | Measurements become Observations only with provenance and context | No |
| Data | Registered SPY daily adjusted-close artifact | Recorded source material, not automatically Observation or Evidence | No |
| Signal | Possible observed pattern in group-level return difference | Possible relevance marker, not Evidence or outcome | No |
| Evidence | Interpreted relation between Observations and Hypothesis/uncertainty/Decision | Assessment of support, challenge, ambiguity, or insufficiency | No |
| Uncertainty | Limits around the Hypothesis, dataset, transferability, and decision | Preserved limits of current knowledge | No |
| Decision | Recommendation about further investigation commitment | Bounded commitment under uncertainty, not trading action | No |
| Design | Local choices keeping investigation small and inspectable | Implementation remains local and non-prescriptive | No |

Where no local interpretation is needed beyond the canonical meaning, the pilot records the owner and uses the concept directly.

## 15. Initial Concept Classification Ledger

| Concept | Classification | Rationale | Foundation promotion? |
|---|---|---|---|
| Question | Foundation-owned concept | Owned by Questions and Inquiry Model | No |
| Inquiry | Foundation-owned concept | Owned by Questions and Inquiry Model | No |
| Hypothesis | Foundation-owned concept | Owned by Hypothesis and Experiment Model | No |
| Experiment | Foundation-owned concept | Owned by Hypothesis and Experiment Model | No |
| Observation | Foundation-owned concept | Owned by Observation Model | No |
| Data | Foundation-owned concept | Defined in Glossary and bounded by Observation/Evidence models | No |
| Signal | Foundation-owned concept | Owned by Evidence Model | No |
| Evidence | Foundation-owned concept | Owned by Evidence Model | No |
| Uncertainty | Foundation-owned concept | Owned by Evidence Model | No |
| Decision | Foundation-owned concept | Owned by Decision Model | No |
| SPY | Domain extension | Local market instrument identifier | No |
| Adjusted close | Domain extension | Market data field needed for local measurement | No |
| Prior 20-trading-day return | Domain extension | Local quantitative measurement convention | No |
| Subsequent 5-trading-day return | Domain extension | Local quantitative measurement convention | No |
| Positive prior-return group | Domain extension | Local grouping convention for this Hypothesis | No |
| Non-positive prior-return group | Domain extension | Local grouping convention for this Hypothesis | No |
| Dataset artifact | Operational artifact | Local file or data artifact required for execution | No |
| Computation script or notebook | Implementation concept | Local execution mechanism if used later | No |
| Group-average difference | Domain extension | Quantitative summary used as Observation input | No |

No speculative future concepts are classified.

## 16. Frozen Success Criteria

Research outcome success:

- Hypothesis receives supporting Evidence under the registered assessment plan.

Research outcome failure:

- Hypothesis is challenged, qualified, unsupported, or cannot be responsibly assessed.

Pilot execution validity:

- registered scope is preserved;
- dataset provenance is adequate;
- transformations follow the Experiment boundary;
- Observation records preserve context and limits;
- Evidence assessment follows the registered plan;
- Decision record is produced.

Pilot execution invalidity:

- dataset provenance is irrecoverable;
- leakage or contamination invalidates assessment;
- transformations depart materially from registration;
- scope expands beyond attribution;
- records cannot distinguish Data, Observation, Evidence, and Decision.

Foundation validation success:

- Foundation concepts guide the pilot without silent redefinition;
- local interpretations are explicit;
- domain extensions remain local;
- implementation autonomy remains intact;
- non-pipeline inquiry semantics are preserved;
- Evidence is relational and uncertainty-aware;
- Decision reasoning remains distinct from rule execution;
- semantic friction is logged without automatic Foundation change.

Foundation validation failure:

- canonical meanings cannot be preserved in legitimate use;
- local domain concepts cannot be distinguished from Foundation meaning;
- implementation autonomy is undermined by Foundation prescription;
- current ownership cannot classify necessary concepts;
- semantic drift cannot be repaired.

A negative or inconclusive quantitative result may still be Foundation validation success.

## 17. Frozen Failure Signals

| Failure signal | Handling |
|---|---|
| Implementation failure | Classify locally; repair if possible; do not treat as Foundation defect |
| Poor local interpretation | Correct local record; log if likely to recur |
| Semantic drift | Pause; classify affected concept; repair or record explicit divergence |
| Excessive Foundation prescription | Remove prescription; preserve autonomy; log source |
| Canonical ambiguity | Log friction; continue only with explicit local interpretation |
| Missing ownership | Quarantine as unresolved ownership question; assess post-pilot |
| Premature abstraction | Keep concept local; block promotion |
| Legitimate divergence | Record explicit divergence candidate and bound scope |
| Invalid research execution | Pause or terminate depending on recoverability |
| Dataset contamination | Mark Evidence assessment contaminated or terminate if severe |
| Observation/Evidence collapse | Pause and repair records before proceeding |
| Decision/action collapse | Repair Decision record; prohibit trading/action framing |

## 18. Stop Conditions

Pause and review:

- scope expands beyond the registered vertical slice but can be reduced;
- implementation begins building general Quant infrastructure;
- local concepts start appearing as Foundation concepts;
- canonical ambiguity blocks interpretation but a bounded local interpretation may be possible;
- dataset provenance has gaps that may be repaired;
- Experiment conditions diverge but can be restored;
- classification disputes threaten meaningful continuation.

Pilot invalidation:

- dataset provenance becomes irrecoverable;
- leakage or contamination invalidates the investigation;
- Experiment conditions materially diverge from registration and cannot be restored;
- success criteria are changed after seeing results;
- Data, Observation, Evidence, and Decision cannot be reconstructed separately;
- the pilot becomes a generic platform or VAKI Quant architecture project.

Foundation review candidate:

- canonical semantics are ambiguous after reasonable owner-based interpretation;
- necessary concept ownership cannot be resolved;
- Foundation wording appears to force implementation prescription;
- legitimate divergence from Foundation meaning appears unavoidable.

## 19. Semantic Friction Log Schema

Each semantic friction entry must preserve:

- identifier;
- date or investigation phase;
- affected Foundation surface;
- local context;
- observed friction;
- competing interpretations, if any;
- current local handling;
- classification;
- severity;
- recurrence status;
- post-pilot review required;
- statement that Foundation change is prohibited during execution.

No serialization technology is prescribed.

## 20. Required Artifact Checklist

Before execution:

- pilot scope declaration;
- preregistration;
- validation questions;
- interpretation map;
- initial classification ledger;
- dataset provenance record and artifact availability confirmation.

During execution:

- Question record;
- Hypothesis record;
- Experiment record;
- Observation records;
- semantic friction log;
- relevant design or implementation decision notes.

After execution:

- Evidence assessment;
- Decision record;
- final validation report;
- post-pilot semantic review.

The system should remain lightweight. A single local document may satisfy multiple artifact roles when semantic visibility is preserved.

## 21. Entry Criteria Assessment

| Criterion | Current status | Evidence in this preregistration | Unresolved blocker |
|---|---|---|---|
| Scope bounded to one Question, one Hypothesis, one dataset slice, and one investigation | Met | Sections 3, 5, 6, 7 | None |
| Validation questions frozen | Met | Section 12 | None |
| Required Foundation surfaces identified | Met | Section 13 | None |
| Foundation reference state recorded | Met | Sections 1, 12, 13, 14 and referenced protocol/discovery documents | None |
| Required artifacts known | Met | Section 20 | None |
| Concept classification rules explicit | Met | Section 15 and protocol alignment | None |
| Semantic friction log structure ready | Met | Section 19 | None |
| Stop conditions defined | Met | Section 18 | None |
| Exclusions accepted | Met | Section 3 | None |
| Implementation freedom confirmed | Met | Sections 2, 7, 14, 16 | None |
| No Foundation edits required before execution | Met | Sections 16, 18, 22 | None |
| Goal is failure discovery, not proof of adequacy | Met | Sections 2, 16 | None |
| Dataset artifact and provenance available before execution | Not met | Section 8 defines requirements | Bounded dataset artifact and provenance record are not present in this repository |

Entry criteria are partially met because dataset artifact availability is a concrete unresolved blocker.

## 22. Freeze Declaration

After execution begins:

- the primary Question is frozen;
- the primary Hypothesis is frozen;
- success criteria are frozen;
- validation questions are frozen;
- scope exclusions are frozen;
- Foundation semantics cannot be modified as part of execution;
- material Experiment changes must be recorded as protocol deviations or require a separately registered investigation;
- post-result reinterpretation must not rewrite preregistration history.

Clerical errors may be corrected only when the correction does not change semantic meaning, scope, Hypothesis, validation questions, success criteria, or decision space. Corrections must preserve the original text or record the change reason.

## 22A. Entry-Gate Reassessment - 2026-07-09

ENTRY CRITERIA MET.

This dated reassessment preserves the original preregistration record above and updates only the execution entry-gate status after closing the previously recorded data blocker.

Dataset artifact and provenance availability:

- bounded dataset artifact exists at `data/pilot/spy_short_horizon_momentum/bounded/SPY_2015-01-01_2019-12-31_daily_adjusted_close.csv`;
- source artifact exists at `data/pilot/spy_short_horizon_momentum/source/SPY_yahoo_chart_2015-01-01_2019-12-31_daily.json`;
- provenance record exists at `docs/audits/FIRST_MANIFESTATION_PILOT_DATASET_PROVENANCE.md`;
- lightweight manifest exists at `data/pilot/spy_short_horizon_momentum/manifest.json`.

Integrity reassessment:

- the bounded artifact matches the frozen dataset boundary: SPY daily adjusted close, 2015-01-01 through 2019-12-31 inclusive where observations exist;
- the bounded artifact contains 1258 rows;
- first available observation date is 2015-01-02;
- last available observation date is 2019-12-31;
- schema, date parseability, chronological ordering, duplicate-date rejection, missing adjusted-close check, non-finite numeric check, boundary check, and empty-dataset check passed;
- NYSE expected-session coverage check found 1258 expected sessions, 1258 observed sessions, no missing expected sessions, and no unexpected observed sessions;
- bounded artifact SHA-256 is `591c3f8e654e611923ad46935f6c41724a24756b60dc3d6d2c3d9298c40406f7`.

Boundary preservation:

- no registered Experiment was executed;
- no 20-trading-day prior returns were calculated;
- no 5-trading-day forward returns were calculated;
- no group labels, group comparisons, research results, Hypothesis assessment, Evidence conclusion, or Decision recommendation were created;
- the dataset remains Data until later registered investigation work creates measurements that may become Observations under the Observation model;
- integrity validation is not Evidence.

The previously recorded blocker, "Bounded dataset artifact and provenance record are not present in this repository," is resolved. No unresolved data blocker currently invalidates pilot execution.

## 23. Execution Handoff

The next execution task should receive:

- this preregistration document;
- the validation protocol;
- the discovery report;
- the Foundation reference documents listed in the protocol;
- a bounded SPY daily adjusted-close dataset artifact for 2015-01-01 through 2019-12-31;
- a provenance record satisfying section 8.

The next task may create a minimal Manifestation pilot scaffold using this preregistration as its contract. It must not create a generic Quant platform, expand Foundation semantics, or alter the registered Question, Hypothesis, success criteria, validation questions, exclusions, or stop conditions.

## 24. Repository Integration and Consistency Review

Minimum navigation integration: this preregistration should be linked from the repository README alongside the first validation discovery and protocol documents. No broader restructuring is required.

Focused consistency review:

- Consistent with `FIRST_MANIFESTATION_VALIDATION_DISCOVERY.md`: preserves the minimal quantitative research pilot boundary and guardrails.
- Consistent with `FIRST_MANIFESTATION_VALIDATION_PROTOCOL.md`: evaluates each entry criterion and refuses full readiness until dataset artifact provenance is available.
- Consistent with `M1_CLOSURE_REPORT.md`: does not reopen M1, does not add semantic owners, and preserves evidence-driven reopening logic.
- Consistent with `FOUNDATION_SPEC.md`: keeps Foundation meaning, local interpretation, local extension, implementation freedom, and no automatic promotion distinct.
- Consistent with canonical Thinking documents: preserves non-pipeline semantics and separates Question, Hypothesis, Experiment, Observation, Evidence, and Decision.
