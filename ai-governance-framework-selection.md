# Choosing AI Governance Frameworks

**Christopher D. Cole | Reusable governance design reference**

Use applicable law to establish obligations, then combine risk methods, management standards and technical guidance to implement them. These instruments complement one another; selecting a framework does not establish compliance.

This guide synthesizes the topics in a supplied framework-selection reference into original portfolio guidance. It is not a claim of certification, legal advice or implementation of every framework in my employment. Source review: **15 November 2026**. Recheck current legal text and application dates before a deployment decision.

## A practical selection method

1. **Define the use:** business purpose, affected people, operating countries, data, model provider and whether the system recommends or acts.
2. **Identify obligations:** have the responsible legal/compliance owner assess jurisdiction, organizational role, sector rules, exceptions and application dates.
3. **Choose a risk backbone:** use NIST AI RMF to organize risk work; add its GenAI Profile for generative systems.
4. **Add the needed depth:** ISO/IEC 42001 for a management system, 23894 for risk guidance, 42005 for impact assessment, and OWASP for LLM security.
5. **Make controls testable:** assign owners, acceptance criteria, evidence, review dates and escalation paths.
6. **Review throughout operation:** revisit the assessment when users, geography, data, model versions, autonomy or intended use change.

For an enterprise assistant, my suggested starting combination is **applicability review + NIST AI RMF + GenAI Profile + OWASP**, adding ISO management-system and impact-assessment guidance where organizational needs justify it. This is a proposed design approach, not a universal requirement.

## Laws and treaty instruments: screen for applicability

The questions below identify topics for review, not automatic legal conclusions. The list is not exhaustive; privacy, employment, consumer protection, sector and other laws may also apply.

| Instrument | When to investigate | Important qualification and source |
|---|---|---|
| EU AI Act | AI placed on the EU market, used in the EU, or otherwise within its territorial scope | Duties depend on role and use classification. Entry into force in August 2024 was not the date every obligation applied. Check the [Commission's current timeline](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai). |
| GDPR Article 22 | Solely automated decisions with legal or similarly significant effects on individuals within GDPR scope | Review exceptions, safeguards and the actual role of human intervention. This is not a blanket prohibition on AI. [GDPR text](https://eur-lex.europa.eu/legal-content/EN/ALL/?uri=celex%3A32016R0679). |
| South Korea AI Basic / Framework Act | AI products and services connected to the Korean market | Effective 22 January 2026; assess the applicable categories and duties, including high-impact and generative AI. [Library of Congress overview](https://www.loc.gov/item/global-legal-monitor/2026-02-20/south-korea-comprehensive-ai-legal-framework-takes-effect/). |
| China Interim Measures for Generative AI Services | Generative AI services offered to the public in mainland China | Effective 15 August 2023. Public-service scope matters; do not assume every internal AI experiment has identical obligations. [Official measures, Articles 2 and 24](https://www.cac.gov.cn/2023-07/13/c_1690898327029107.htm). |
| Japan AI Act | AI development and use connected to Japan | Promotion-oriented legislation; promulgated and partly effective 4 June 2025, fully effective 1 September 2025. Do not equate it with the EU's risk-tier regime. [Cabinet Office](https://www8.cao.go.jp/cstp/ai/ai_act/ai_act.html). |
| California SB 53 | Frontier-model development within the law's scope | Distinguish frontier developers from large frontier developers and check the actual definitions and duties; compute alone is not a complete applicability test. [Governor's signed-law summary](https://www.gov.ca.gov/2025/09/29/governor-newsom-signs-sb-53-advancing-californias-world-leading-artificial-intelligence-industry/). |
| Texas TRAIGA, HB 149 | AI development or deployment within the statute's scope in Texas | Effective 1 January 2026. Includes prohibited uses and disclosures for specified contexts; not a universal certification requirement. [Texas Legislature summary](https://capitol.texas.gov/billlookup/BillSummary.aspx?Bill=HB149&LegSess=89R). |
| Utah AI disclosure legislation | Consumer-facing GenAI and relevant regulated activities | The original 2024 provision, Section 13-2-12, was repealed in 2025. Consult the updated disclosure framework and amendments in [Title 13, Chapter 77](https://le.utah.gov/xcode/Title13/Chapter77/C13-77_2025050820250508.pdf), rather than relying on the infographic's original date. |
| NYC Local Law 144 | Covered automated tools substantially assisting hiring or promotion decisions | Covered use requires a recent independent bias audit, publication of audit information and required notices. Not every AI hiring tool automatically meets the definition. [DCWP guidance](https://www.nyc.gov/site/dca/about/automated-employment-decision-tools.page). |
| Council of Europe AI Framework Convention | Human-rights governance and obligations arising through participating jurisdictions | Opened for signature 5 September 2024. Signature is not equivalent to entry into force or a directly applicable corporate duty; check ratification and domestic implementation. [Council of Europe](https://www.coe.int/en/web/artificial-intelligence/the-framework-convention-on-artificial-intelligence). |

## Standards, principles and technical guidance

These are different types of instruments. A technical risk list is not a certifiable management standard. Voluntary guidance may also become relevant through contracts, procurement or organizational policy.

| Reference | Best use | Suggested evidence or output |
|---|---|---|
| [NIST AI RMF 1.0](https://www.nist.gov/itl/ai-risk-management-framework) — 2023 | Organize AI risk work across Govern, Map, Measure and Manage | Owners, use context, risk register, evaluation results and treatment decisions |
| [NIST GenAI Profile, AI 600-1](https://doi.org/10.6028/NIST.AI.600-1) — 2024 | Extend the RMF to generative AI risks | GenAI-specific evaluation and mitigation plan |
| [ISO/IEC 42001](https://www.iso.org/standard/42001) — 2023 | Establish a certifiable AI management system | Management-system scope, policies, responsibilities and improvement records; no certification is claimed here |
| [ISO/IEC 23894](https://www.iso.org/sectors/it-technologies/ai) — 2023 | Add AI-specific risk-management guidance | Risk assessment and treatment records |
| [ISO/IEC 42005](https://www.iso.org/sectors/it-technologies/ai) — 2025 | Structure AI system impact assessments | Affected-person analysis, impact assessment and review record |
| [OECD AI Principles](https://www.oecd.org/en/about/news/press-releases/2024/05/oecd-updates-ai-principles-to-stay-abreast-of-rapid-technological-developments.html) — 2019, updated 2024 | Establish an internationally aligned policy baseline | Principles translated into accountable practices |
| [G7 Hiroshima Code of Conduct](https://www.oecd.org/content/dam/oecd/en/publications/reports/2025/09/how-are-ai-developers-managing-risks_fbaeb3ad/658c2ad6-en.pdf) — 2023 | Guide organizations developing advanced AI systems | Lifecycle testing, risk mitigation and transparency practices |
| [Singapore Model AI Governance Framework for GenAI](https://www.imda.gov.sg/-/media/imda/files/news-and-events/media-room/media-releases/2024/05/annex-a-nine-dimensions-of-the-model-ai-governance-framework-for-generative-ai.pdf) — 2024 | Translate GenAI governance into practical areas of responsibility | Accountability, data, testing, incident handling and provenance practices |
| [UNESCO Recommendation on AI Ethics](https://www.unesco.org/en/legal-affairs/recommendation-ethics-artificial-intelligence) — 2021 | Consider human rights and wider societal impacts | Documented stakeholder and ethical-impact considerations |
| [OWASP Top 10 for LLM Applications](https://genai.owasp.org/resource/owasp-top-10-for-llm-applications-2025/) — 2025 edition | Guide application threat modeling and security testing | Tests and mitigations for prompt injection, information exposure and unsafe tool actions |

The evidence column is a suggested implementation aid, not an authoritative clause-by-clause compliance mapping. ISO summaries here rely on public descriptions, not reproduction of licensed standards.

## Connect framework selection to idea screening

Extend the [employee idea-screening pattern](ai-governance-idea-screening.md) with these proposed fields:

| Intake field | Why it matters | Route when unknown |
|---|---|---|
| Operating jurisdictions and affected people | Helps determine which legal reviews are needed | Applicability review |
| Provider, deployer and business-owner roles | Clarifies who is responsible for which decisions | Ownership clarification |
| Intended decision and level of autonomy | Separates drafting support from consequential actions | Human-oversight review |
| Data categories, provenance and access | Identifies privacy, permission and quality questions | Data-owner review |
| Model/service and public vs internal exposure | Helps select relevant GenAI and security checks | Architecture/security review |
| Candidate obligations and supporting sources | Makes the basis for a recommendation reviewable | Legal/compliance validation |
| Selected guidance, controls and evidence | Turns a framework name into delivery requirements | Control-owner assessment |

An intake agent can collect facts, identify gaps and suggest candidate references. It should not declare a law inapplicable, issue a compliance certification, accept residual risk or approve production.

## From principles to delivery controls

This is an illustrative design mapping, not a claim that any row completely satisfies a standard or law.

| Concern | Example control | Evidence | Accountable role |
|---|---|---|---|
| Unsupported answers | Require source support and an explicit insufficient-evidence outcome | Grounding tests and reviewer corrections | Product owner |
| Unauthorized data use | Enforce approved access and data boundaries outside the prompt | Access tests and data approvals | Data/security owner |
| Prompt injection and unsafe actions | Separate untrusted content from instructions; constrain tool permissions | Adversarial tests and action logs | Engineering/security |
| Harmful or unequal outcomes | Evaluate affected groups and provide an appropriate review path | Impact assessment and evaluation results | Risk/business owner |
| Unclear decision authority | Require authorized approval for consequential actions | Approval records and escalation tests | Business owner |
| Model or workflow changes | Version configurations and rerun relevant evaluations | Change log and regression evidence | Delivery owner |

Use [agent configuration and validation](agent-configuration-and-validation.md) to translate these controls into instructions, runtime restrictions and tests, and [evaluation and guardrails](evaluation-and-guardrails.md) to assess behavior.

## Fictional example: internal service-request summarizer

A proposed assistant drafts summaries for staff and cannot send messages, approve requests or change customer records.

- **Review applicability:** record operating countries, personal-data use and whether outputs influence significant decisions. Internal use does not automatically remove legal obligations.
- **Select guidance:** use NIST AI RMF and the GenAI Profile as the risk structure; use OWASP for application security. Consider ISO/IEC 42005 for impact assessment and ISO/IEC 42001 if an organizational management system is needed.
- **Require evidence:** approved data access, grounded-summary tests, injection tests, representative error review and documented human responsibilities.
- **Record the decision:** the authorized owner decides whether to pilot, remediate or reject, with unresolved risks and review dates recorded.

This is a synthetic design example, not an employer implementation or measured outcome.

## Reusable decision record

| Field | Complete for each use case |
|---|---|
| Use case / owner / version | Name, accountable owner, model and workflow version |
| Scope | Users, affected people, countries, data and autonomy |
| Legal assessment | Candidate obligations, applicability rationale, reviewer and source date |
| Selected references | Framework versions and why each is needed |
| Controls and evidence | Requirement, owner, test, result and evidence location |
| Gaps and residual risk | Unresolved issues, remediation owner and due date |
| Decision | Pilot / remediate / reject; authorized approver and rationale |
| Reassessment triggers | Model, data, geography, purpose, autonomy or law changes |

Maintain one control-and-evidence register with multiple framework mappings where appropriate. Reuse evidence only when it actually supports each requirement.

[Portfolio overview](README.md) · [Idea screening](ai-governance-idea-screening.md) · [Evaluation and guardrails](evaluation-and-guardrails.md)
