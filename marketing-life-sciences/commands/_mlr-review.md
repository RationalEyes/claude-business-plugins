---
description: Simulate medical-legal-regulatory review of promotional content
argument-hint: "<content to review>"
---

# MLR Review

<!-- Life Sciences Addition -->

> If you see unfamiliar placeholders or need to check which tools are connected, see [CONNECTORS.md](../CONNECTORS.md).

Simulate a Medical-Legal-Regulatory (MLR) review of pharmaceutical or medical device promotional content. Identify compliance issues, flag unsubstantiated claims, check fair balance, and provide a reviewable assessment before formal MLR submission.

## Trigger

User runs `/mlr-review` or asks to review promotional content for regulatory compliance, check fair balance, simulate MLR review, or prepare content for medical-legal-regulatory submission.

## Inputs

1. **Content to review** — accept content in any of these forms:
   - Pasted directly into the conversation
   - A file path or ~~knowledge base reference
   - A URL to a digital promotional asset
   - Multiple pieces for batch review

2. **Content classification** — determine or ask:
   - Branded promotional
   - Unbranded disease awareness
   - Reminder advertising
   - Scientific exchange
   - Patient-facing material
   - Congress material
   - Social media content

3. **Target market** (optional) — US (FDA), EU (EMA), or specific country. If not specified, default to US FDA rules.

4. **Product context** (optional but recommended):
   - Product name (brand and INN)
   - Approved indication(s)
   - Key safety information
   - Whether the product has a black box warning or REMS

## Review Process

### Step 1: Content Classification

Classify the content using the regulatory-compliance skill classification matrix. Confirm the classification with the user if ambiguous. The classification determines which review checks apply.

### Step 2: Medical Review

Evaluate the content from the perspective of a medical reviewer:

- **Clinical accuracy** — do all clinical statements accurately reflect published data and approved labeling?
- **Reference verification** — is every efficacy and safety claim annotated with a specific, verifiable reference?
- **Data presentation** — are clinical data presented completely and without misleading emphasis?
- **Statistical context** — do data presentations include appropriate statistical measures (CI, p-value, HR)?
- **Off-label check** — does any language suggest or imply use outside the approved indication?
- **Study context** — is the study design, population, and methodology described for cited data?

### Step 3: Legal Review

Evaluate the content from the perspective of a legal reviewer:

- **Unsubstantiated claims** — are there superlatives, comparatives, or absolute statements without adequate support?
- **Comparative claims** — do any comparisons to competitors use adequate direct comparative data?
- **Trademark compliance** — are brand names, trademarks, and registration symbols used correctly?
- **Copyright** — are all images, figures, and third-party content properly licensed or attributed?
- **Testimonials** — do any patient or HCP testimonials include required disclosures?
- **Sunshine Act/EFPIA** — are transparency reporting obligations addressed?

### Step 4: Regulatory Review

Evaluate the content from the perspective of a regulatory reviewer:

- **Indication statement** — does it match the approved labeling exactly?
- **Fair balance** — is risk information presented with comparable prominence to benefit information?
- **ISI completeness** — is Important Safety Information complete and current?
- **PI/SmPC reference** — is the full Prescribing Information attached or linked?
- **Black box warning** — if applicable, is it prominently displayed?
- **Material classification** — is the content correctly classified for regulatory purposes?
- **Expiration/review date** — is a review date assigned for the material?

### Step 5: Fair Balance Assessment

Apply the fair balance scoring framework from the regulatory-compliance skill:

| Dimension | Score (1-5) | Assessment |
|-----------|-------------|------------|
| Prominence | | |
| Completeness | | |
| Readability | | |
| Placement | | |
| Language | | |
| **Average** | | |

## Output Format

### MLR Review Summary

- **Content type:** [classification]
- **Target market:** [US/EU/other]
- **Overall assessment:** APPROVE / APPROVE WITH REVISIONS / REVISE AND RESUBMIT / REJECT
- **Fair balance score:** [average score] / 5.0
- **Critical issues:** [count]
- **Major issues:** [count]
- **Minor issues:** [count]

### Detailed Findings

For each issue found, provide:

| # | Issue | Review Function | Severity | Location | Recommendation |
|---|-------|----------------|----------|----------|---------------|

Where severity is:
- **Critical** — regulatory violation; would likely trigger FDA/EMA enforcement action
- **Major** — significant compliance risk; must be resolved before distribution
- **Minor** — best practice improvement; should be resolved but not blocking

### Annotated Content

For the top issues, provide a before/after showing the original text and a compliant revision.

### Reference Verification

| Claim | Reference Cited | Reference Valid | Notes |
|-------|----------------|----------------|-------|
| | | Yes/No/Missing | |

### Compliance Checklist Summary

| Check | Status | Notes |
|-------|--------|-------|
| Indication matches labeling | | |
| Fair balance maintained | | |
| ISI complete and current | | |
| PI/SmPC attached or linked | | |
| All claims referenced | | |
| No off-label implications | | |
| Black box warning displayed (if applicable) | | |
| Material properly classified | | |

## After Review

Ask: "Would you like me to:
- Revise the content to address all identified issues?
- Focus on resolving only the critical and major issues?
- Generate a compliant alternative version from scratch?
- Review additional content against the same standards?
- Prepare a summary of changes for the MLR committee?"
