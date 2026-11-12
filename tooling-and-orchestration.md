# Readiness, Orchestration and Exception Ownership

**Reusable design pattern informed by the [readiness experience case](financial-crime-readiness-case.md). This is a proposed specification, not a production system export.**

## Business rule

Do not send incomplete or unusable evidence into downstream analysis without an explicit, owned disposition. A readiness decision should be explainable at portfolio level and traceable to the relevant case and check.

| Check | Question | Proposed blocking condition | Resolution owner |
|---|---|---|---|
| Source completeness | Are required sources present for this case type? | A mandatory source is missing and no approved exception applies | Business/source owner |
| Extraction survival | Is required content readable after ingestion? | Required pages, tables or fields cannot be read | Ingestion team |
| Value consistency | Do critical extracted values match the source? | Material discrepancy in a required value | Data team with business validation |
| Masking conformance | Is sensitive information handled under the approved policy? | Required masking or retained entity relationships fail validation | Privacy/control owner with engineering |
| Decision traceability | Can the readiness result be reproduced? | Check version, evidence or disposition is missing | Workflow owner |

Define critical fields, tolerances and allowed exceptions with business and control owners before testing. “Missing” and “not applicable” are different states.

## Proposed states

- **Pending:** Checks have not completed.
- **Blocked:** A required check failed; record the reason and owner.
- **Ready:** Required checks passed for the agreed scope.
- **Approved exception:** A named owner accepted a specific deviation with rationale, scope and expiry.

Re-run affected checks after correction. Keep previous results and the rule version so a changed readiness decision remains explainable. A technical failure should not silently become a business approval.

## Minimum evaluation set

Include complete, missing-source, unreadable, contradictory-value, masking-failure, duplicate and approved-exception cases. Business experts label expected outcomes. Measure incorrectly accepted cases, unnecessary blocks and time to resolve a block separately; a high pass rate alone is not success.

## Operating metrics

Track ready/blocked/pending counts, block reasons, age by owner, repeat failures, resubmission rate, false-ready rate on reviewed samples and downstream rework. Use trends to fix upstream causes and keep investigators focused on usable case packages.

[Evaluation and guardrails](evaluation-and-guardrails.md) · [Adoption and operating model](adoption-and-operating-model.md)
