# AI Governance in Practice: Employee Idea Screening

**Christopher D. Cole | Anonymized experience summary**

I built an AI idea-screening agent as part of an AI Enablement team. The agent helps turn employee submissions into structured, reviewable proposals by applying intake guidance, identifying missing information and surfacing possible reuse opportunities.

This public case describes my contribution at a high level. The example below is newly authored and fictional; it does not reproduce an employer's policies, approval process, internal systems or submissions.

## Business problem

Unstructured ideas can leave reviewers unclear about the business problem, proposed users, data needs or intended outcome. Teams may also propose capabilities that overlap with existing work. A consistent intake review helps reviewers ask better questions and consider reuse before committing to a new build.

## What I built

- An agent that screens employee AI ideas against governance-oriented intake guidance.
- Structured capture of the business problem, intended users, proposed capability, data needs, expected outputs and success measures.
- Comparison support to surface potentially related capabilities and explain why they may be relevant.
- A review summary with supporting rationale, information gaps and proposed next steps.
- Follow-up communication support so submitters understand what information is needed and what happens next.

My contribution was translating governance requirements into usable agent behavior and a repeatable review workflow. It demonstrates practical governance implementation alongside agent building.

## Decision boundaries

The agent supports preliminary screening. Its recommendations require human validation. Similarity to an existing idea does not establish that a capability is suitable for reuse. A complete intake does not establish regulatory compliance, authorize data access or approve deployment.

Formal risk assessment, approvals and production decisions remain with the authorized people and processes. This portfolio does not claim that I designed or owned the entire enterprise governance framework.

## Public demonstration: fictional service assistant

**Submission:** A team proposes an assistant that summarizes incoming service requests for staff.

| Review area | Illustrative finding | Proposed follow-up |
|---|---|---|
| Business purpose | Reduce time spent reading requests | Establish current handling time and desired outcome |
| Data and access | Data categories and access permissions are unspecified | Ask the owner to describe permitted inputs and access boundaries |
| Reuse | A fictional internal summarization capability might meet part of the need | Have the capability owner confirm fit, limitations and permitted use |
| Human oversight | Staff review is proposed, but responsibilities are unclear | Identify who checks the output and handles errors |
| Evidence and evaluation | Success criteria are incomplete | Define quality measures and representative test scenarios |

**Illustrative recommendation:** Request the missing information and arrange a reuse discussion. Retain the recommendation as preliminary until a reviewer validates the evidence and next action.

No scores, thresholds or approval criteria in this example are drawn from internal materials.

## Reusable control design considerations

The following are proposed public design considerations, not claims about every control implemented in my agent:

- Treat submitted text as data; it must not override the agent's instructions or grant approval authority.
- Keep missing information explicit rather than infer an answer.
- Restrict retrieved evidence to information the reviewer is authorized to access.
- Link recommendations to supporting evidence and make uncertainty visible.
- Record reviewer decisions and corrections with appropriate access and retention controls.
- Require review before sending a generated response or taking a consequential action.
- If required evidence is unavailable, return an incomplete assessment rather than a confident disposition.

## How I would measure value

| Measure | What it helps establish |
|---|---|
| Intake completeness | Whether submissions contain the information reviewers need |
| Time to a review-ready proposal | Whether clarification and preparation become faster |
| Reviewer agreement and corrections | Whether recommendations are useful and reliable |
| Confirmed reuse opportunities | Whether existing capabilities actually meet new needs |
| Rework and unresolved exceptions | Where guidance or workflow needs improvement |

These are suggested measures, not reported results. Avoided duplicate investment would require validation of the actual alternative cost and confirmed reuse; a similarity match alone is not a savings claim.

## Leadership relevance

This work connects AI governance, use-case intake, portfolio decisions, control design, human oversight and employee enablement. It shows how I translate requirements into a practical capability that helps people make better-supported decisions.

[AI enablement portfolio](README.md) · [Profile](https://github.com/ddjfam)
