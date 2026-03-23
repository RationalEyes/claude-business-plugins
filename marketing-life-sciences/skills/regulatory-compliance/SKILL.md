---
name: regulatory-compliance
description: Pharmaceutical and medical device regulatory compliance for marketing materials. Use when reviewing promotional content for FDA or EMA compliance, preparing materials for MLR review, checking fair balance requirements, classifying promotional materials by type, simulating medical-legal-regulatory review, ensuring off-label restrictions are met, or navigating life sciences advertising regulations.
---

# Regulatory Compliance Skill

<!-- Life Sciences Addition -->

Frameworks and checklists for ensuring life sciences marketing materials comply with FDA, EMA, and local regulatory requirements. This skill covers promotional material classification, MLR review simulation, fair balance enforcement, and off-label restriction compliance.

## Promotional Material Classification

Classify every piece of marketing content before production begins. The classification determines the review pathway, required disclosures, and permissible content.

### Classification Matrix

| Type | Definition | Product Named | Claims Made | Review Required |
|------|-----------|---------------|-------------|-----------------|
| Branded promotional | Presents product with efficacy or safety claims | Yes | Yes | Full MLR |
| Unbranded disease awareness | Discusses condition without naming product | No | Disease-level only | Medical + Legal |
| Reminder advertising | Product name, dosage form, cost — no claims | Yes | No | Abbreviated MLR |
| Help-seeking advertisement | Describes disease, directs to physician — no product | No | No | Medical + Legal |
| Scientific exchange | Balanced data presentation, peer-to-peer | Varies | Scientific data | Medical review |
| Institutional advertising | Corporate reputation, no product claims | No (company only) | No product claims | Legal + Corporate |
| Patient labeling | FDA-approved patient information | Yes | Approved labeling only | Regulatory |

### Classification Decision Tree

1. Does the material name a specific product? If NO: unbranded or help-seeking
2. Does it make efficacy, safety, or superiority claims? If NO: reminder advertising
3. Is it intended for scientific exchange between peers? If YES: scientific exchange
4. Otherwise: branded promotional (full MLR review required)

## MLR Review Simulation

Use this framework to simulate a Medical-Legal-Regulatory review before submitting content to the actual MLR committee. This pre-review catches common issues and reduces revision cycles.

### Medical Review Checklist

| Check | Pass/Fail | Notes |
|-------|-----------|-------|
| All efficacy claims match approved labeling | | |
| Clinical data accurately represents published results | | |
| Statistical context included (CI, p-value, HR) | | |
| Study limitations acknowledged | | |
| Patient population described for each cited study | | |
| No extrapolation beyond approved indication | | |
| Mechanism of action description is scientifically accurate | | |
| Adverse event profile is complete and accurate | | |
| No off-label implications (explicit or implied) | | |
| References are complete and from approved sources | | |

### Legal Review Checklist

| Check | Pass/Fail | Notes |
|-------|-----------|-------|
| No unsubstantiated comparative claims | | |
| No superlatives without substantiation | | |
| Trademark and registration symbols used correctly | | |
| Copyright compliance for all images and content | | |
| No misleading presentations of data | | |
| Competitor references are accurate and fair | | |
| Testimonials include required disclosures | | |
| No implied guarantees of outcomes | | |
| Sunshine Act/EFPIA disclosure requirements met | | |
| Privacy and data protection compliance (HIPAA, GDPR) | | |

### Regulatory Review Checklist

| Check | Pass/Fail | Notes |
|-------|-----------|-------|
| Indication statement matches approved labeling exactly | | |
| Fair balance maintained (risk/benefit prominence) | | |
| ISI is complete and prominently placed | | |
| Black box warning displayed (if applicable) | | |
| PI/SmPC attached or linked (branded materials) | | |
| Material coded with unique job number for tracking | | |
| Expiration date or review date assigned | | |
| Distribution channel is appropriate for content type | | |
| OPDP/EMA filing requirements identified (if applicable) | | |
| Local country-specific requirements met (for ex-US materials) | | |

### Common MLR Rejection Reasons

| Rejection Reason | How to Avoid |
|-----------------|--------------|
| Claim not supported by reference | Annotate every claim before submission; verify against PI/SmPC |
| Misleading data presentation | Include all relevant context: sample size, confidence intervals, p-values |
| Insufficient fair balance | Check that risk information has equal visual weight to benefit claims |
| Off-label implication | Review for any language suggesting use outside approved indication |
| Missing ISI | Include complete ISI; verify against current PI/SmPC version |
| Outdated references | Verify all references are current; replace retracted or superseded publications |
| Unapproved comparative claim | Ensure all comparisons use published, peer-reviewed head-to-head data |
| Inconsistent with current labeling | Cross-check against the most recent PI/SmPC — labels get updated |

## Fair Balance Checker

Apply this framework to evaluate whether a piece of content maintains fair balance between efficacy and risk information.

### Fair Balance Scoring

For each piece of content, score these dimensions:

| Dimension | Score (1-5) | Criteria |
|-----------|-------------|----------|
| Prominence | | 5 = equal visual weight; 1 = risk buried or minimized |
| Completeness | | 5 = all material risks included; 1 = significant risks omitted |
| Readability | | 5 = risk info equally readable; 1 = smaller font, lighter color, dense text |
| Placement | | 5 = risk near associated benefit claims; 1 = risk segregated at end only |
| Language | | 5 = clear, direct risk language; 1 = euphemistic or minimizing language |

**Scoring guidance:**
- Average score of 4-5: Fair balance likely adequate
- Average score of 3: Fair balance at risk — revise before MLR submission
- Average score below 3: Fair balance inadequate — major revision required

### Fair Balance by Content Format

| Format | Fair Balance Requirements |
|--------|------------------------|
| Print detail aid | ISI in same font size as body text; risk pages comparable in number to efficacy pages |
| Digital banner ad | Brief summary or link to full PI; major risks visible without scrolling |
| Email (HCP) | ISI below body copy; must be visible before recipient needs to scroll significantly |
| Video/Audio | Major statement of risks must be presented with comparable prominence to benefits |
| Social media | ISI link in every branded post; risk summary in post text for platforms allowing it |
| Website | Sticky ISI footer or persistent link; ISI accessible from every branded page |
| Conference poster | ISI panel of comparable size to efficacy panels |

## Off-Label Restriction Compliance

Off-label promotion — promoting a drug for uses not approved in the labeling — is prohibited in the United States and most other jurisdictions. This section provides guardrails to prevent off-label violations.

### Off-Label Red Flags

Flag content for review if it contains any of the following:

- References to patient populations not in the approved indication
- Discussion of dosing regimens different from approved labeling
- Presentation of data from trials in unapproved indications without clear labeling context
- Testimonials describing use outside the approved indication
- Comparisons to products approved for a different indication
- Language suggesting efficacy in a broader population than the studied population
- Links to publications describing off-label use without appropriate context

### Permissible Scientific Exchange

Distinguish between prohibited off-label promotion and permissible scientific exchange:

| Permissible | Not Permissible |
|-------------|-----------------|
| Responding to unsolicited HCP requests for information | Proactively sharing off-label data in promotional context |
| Presenting balanced, peer-reviewed data through medical affairs | Cherry-picking off-label data to support commercial messaging |
| Distributing reprints of peer-reviewed articles (with appropriate context) | Using reprints as promotional tools targeted to drive off-label prescribing |
| MSL discussions of published scientific data | Sales rep discussions of unapproved uses |
| Formulary dossier including comprehensive clinical data | Payer presentations emphasizing off-label benefits |

## Regulatory Framework References

For detailed regulatory guidance, consult the reference documents:
- `references/fda-promotional-rules.md` — US FDA promotional advertising regulations and OPDP enforcement
- `references/ema-requirements.md` — EU EMA advertising requirements and member state variations
