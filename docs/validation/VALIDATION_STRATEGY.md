# Foundation Validation Strategy

## 1. Purpose

Validation builds revisable confidence that Foundation semantics can guide real Manifestations while preserving semantic coherence, semantic ownership, Foundation/Manifestation boundaries, Manifestation autonomy, local interpretation and extension, traceability, contextual limits, and non-prescriptive Foundation guidance.

Validation is evidence concerning Foundation usability and adequacy within a declared scope. It is not proof of universal correctness.

This strategy defines the Foundation-level role of validation. It does not redefine Evidence, Proof, Question, Hypothesis, Experiment, Observation, Decision, or Design. Evidence semantics remain owned by the [Evidence Model](../thinking/EVIDENCE.md). Decision semantics remain owned by the [Decision Model](../method/DECISION_MODEL.md). Foundation/Manifestation boundary semantics remain owned by the [Foundation Specification](../FOUNDATION_SPEC.md) and [ADR-0001](../../decisions/ADR-0001-foundation-manifestation-boundary.md).

## 2. Validation Boundaries

Validation is not:

- mathematical proof;
- scientific proof;
- universal verification;
- proof of completeness;
- permanent closure of inquiry;
- guarantee of applicability to every domain;
- automatic authorization to modify Foundation semantics;
- automatic promotion of local Manifestation concepts.

Validation may use Evidence, but Validation and Evidence are not synonyms. Evidence is relational information that changes credibility in relation to a claim, hypothesis, model, uncertainty, question, or decision. Validation uses relevant Evidence to evaluate usability or adequacy for a declared purpose and scope.

Validation Evidence is not Proof. A validation claim should preserve the scope, assumptions, contextual limits, and remaining uncertainty that make the claim responsible.

## 3. Validation Sources

Validation Evidence may originate from different sources, including:

- semantic audits;
- consistency reviews;
- pilot Manifestations;
- independent Manifestations;
- cross-domain reuse;
- production experience;
- failure analysis.

These are possible sources, not a mandatory universal process. Different sources provide different strengths and limits of evidence. No single source is sufficient for every validation question.

## 4. Audit and Pilot Distinction

An audit primarily examines internal semantic coherence, semantic ownership, terminology consistency, boundary clarity, and compatibility across Foundation documents.

A pilot examines whether the Foundation can guide a bounded real Manifestation without becoming prescriptive, losing semantic clarity, or absorbing local concepts prematurely.

Audits and pilots answer different questions. Neither replaces the other. A Manifestation is not required by this strategy to conduct both.

## 5. Declared Scope

Every validation claim should state its scope.

A validation record should distinguish:

- exercised Foundation semantics;
- non-exercised Foundation semantics;
- assumptions;
- contextual limits;
- relevant Foundation version or commit;
- relevant Manifestation and artifact scope;
- observed outcomes;
- unresolved or non-blocking observations.

One pilot may provide strong evidence within its exercised scope. It must not be treated as universal validation of the Foundation, a domain, a method, or future Foundation revisions.

## 6. Negative Results

A failed or inconclusive pilot does not automatically invalidate the Foundation.

Failure may originate from:

- implementation defects;
- incorrect domain interpretation;
- unsuitable assumptions;
- insufficient or weak Evidence;
- domain-specific constraints;
- local extension defects;
- an actual Foundation limitation.

The source of failure should remain an inquiry question until the evidence supports a classification. Negative, inconclusive, and boundary-revealing results may still produce useful learning.

## 7. Foundation Evolution

Validation does not automatically modify the Foundation.

Foundation change requires explicit inquiry and an explicit decision under the repository's existing governance mechanisms. Local solutions remain local unless they are deliberately evaluated and explicitly integrated as Foundation semantics.

Recurring evidence across contexts may justify opening Foundation-level inquiry. It must not predetermine the result. The Foundation may learn from validation without accepting every repeated local practice as canonical.

This strategy does not introduce a numeric promotion threshold or a new milestone.

## 8. Learning from Validation

Validation contributes knowledge about the Foundation.

Many outcomes strengthen confidence in existing semantics. Some outcomes reveal local practices that should remain Manifestation-specific. Some outcomes may reveal recurring limitations suitable for Foundation-level inquiry. Validation may inform Foundation evolution, but it never determines Foundation evolution automatically.

Promotion from local extension to Foundation semantics requires deliberate evaluation and explicit integration. A local extension is not a Foundation extension merely because it worked, recurred, or proved useful in one Manifestation.

Validation learning should preserve the distinction between:

- Manifestation learning: what a Manifestation learns about its domain, implementation, local extensions, practices, and constraints;
- Foundation learning: what the Foundation learns about the usability, adequacy, clarity, or limits of its existing semantics;
- Foundation change: an explicit modification to canonical Foundation semantics after inquiry and decision.

These are related, but not identical.

Negative, inconclusive, and boundary-revealing outcomes may all be valuable. They can clarify contextual limits, expose weak assumptions, preserve negative knowledge, identify interpretation risks, or show that existing semantics remain sufficient.

## 9. Confidence and Revisability

Validation increases, decreases, or otherwise changes confidence within scope.

Confidence remains revisable in light of later Evidence. A successful validation does not permanently close inquiry. A later validation may strengthen, qualify, narrow, challenge, or supersede an earlier confidence judgment.

## 10. Non-Prescriptive Character

The Foundation defines semantics and boundaries. Manifestations retain implementation freedom.

An illustrative validation progression may be:

```text
internal semantic review
-> audit
-> pilot Manifestation
-> independent Manifestation
-> cross-domain validation
-> long-term production evidence
```

This progression is not a required lifecycle, maturity model, approval path, or validation pipeline. Manifestations may choose validation approaches appropriate to their domains, consequences, risks, and claims of Foundation alignment.

Validation records should serve understanding, traceability, and responsible confidence. They should not turn the Foundation into a certification system or impose domain-specific implementation requirements.
