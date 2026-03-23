# Marketing Plugin — Life Sciences Edition

A life sciences adaptation of the marketing plugin, primarily designed for [Cowork](https://claude.com/product/cowork), Anthropic's agentic desktop application — though it also works in Claude Code. Extends the full general marketing toolkit with pharmaceutical, biotech, and medtech capabilities: regulatory compliance (FDA/EMA), MLR review workflows, HCP engagement, KOL strategy, congress marketing, and pharma-specific KPIs.

This plugin preserves all functionality from the base marketing plugin and adds life sciences-specific content marked with `<!-- Life Sciences Addition -->` comments throughout.

## Installation

### Via Marketplace (recommended)

Add the marketplace first, then install this plugin:

```bash
/plugin marketplace add RationalEyes/claude-business-library
/plugin install marketing-life-sciences@claude-business-library
```

### Claude Cowork (Desktop)

**Plugins → Manage Plugins → Add marketplace from GitHub** → enter `RationalEyes/claude-business-library` → install Marketing for Life Sciences

Or upload the plugin `.zip` directly: **Plugins → Manage Plugins → Upload Plugin → Approve**

## Handbook

Full documentation: [PDF](../docs/marketing-life-sciences/handbook.pdf) · [Markdown](../docs/marketing-life-sciences/handbook.md)

## Commands and Skills — How They Differ

This plugin contains two types of capabilities: **commands** (prefixed with `_`) and **skills** (no prefix). They appear in the same list when you tap `+` in Cowork, but they work very differently:

- **Commands** (`_name`) — Explicit workflows you invoke with `/`. They only run when you call them. Think of them as saved prompts that execute a specific task.
- **Skills** (plain name) — Context-triggered knowledge that Claude activates automatically when your conversation matches the skill's domain. You *can* invoke them with `/`, but you don't need to — just describe what you need in plain language.

The `_` prefix ensures commands sort to the top of the list and gives you a visual cue: underscore = you must invoke it; no underscore = Claude handles it automatically.

## Commands

### Base Marketing Commands

| Command | Description |
|---|---|
| `/_draft-content` | Draft blog posts, social media, email newsletters, landing pages, press releases, and case studies |
| `/_campaign-plan` | Generate a full campaign brief with objectives, channels, content calendar, and success metrics |
| `/_brand-review` | Review content against your brand voice, style guide, and messaging pillars |
| `/_competitive-brief` | Research competitors and generate a positioning and messaging comparison |
| `/_performance-report` | Build a marketing performance report with key metrics, trends, and optimization recommendations |
| `/_seo-audit` | Run a comprehensive SEO audit — keyword research, on-page analysis, content gaps, technical checks, and competitor comparison |
| `/_email-sequence` | Design and draft multi-email sequences for nurture flows, onboarding, drip campaigns, and more |

<!-- Life Sciences Addition -->

### Life Sciences Commands

| Command | Description |
|---|---|
| `/_mlr-review` | Simulate medical-legal-regulatory review of promotional content — check fair balance, reference annotation, off-label compliance, and ISI completeness |
| `/_congress-plan` | Plan conference and congress marketing activities — booth strategy, KOL engagement, data dissemination, competitive intelligence, and post-congress content |
| `/_kol-strategy` | Develop a KOL engagement strategy — identification, tiering, engagement planning, advisory boards, speaker programs, and measurement |

## Skills

### Base Marketing Skills

| Skill | Description |
|---|---|
| `content-creation` | Content type templates, writing best practices by channel, SEO fundamentals, headline formulas, CTA guidance, plus life sciences content types (detail aids, MOA content, formulary dossiers, patient education) and MLR review preparation |
| `campaign-planning` | Campaign frameworks, channel selection, content calendar creation, budget allocation, success metrics, plus life sciences campaign types (disease awareness, congress marketing, P2P, patient support), HCP segmentation, and regulatory review workflow integration |
| `brand-voice` | Brand voice documentation, voice attributes, tone adaptation, style guide enforcement, terminology management, plus pharma brand voice rules (fair balance, ISI placement, claim substantiation, drug naming conventions, prohibited language) |
| `competitive-analysis` | Competitive research methodology, messaging comparison, content gap analysis, positioning, battlecard creation, plus formulary positioning analysis, clinical trial comparison, label comparison, and pipeline intelligence |
| `performance-analytics` | Key metrics by channel, reporting templates, trend analysis, attribution modeling, optimization frameworks, plus pharma KPIs (NRx/TRx, market share, SOV, prescriber adoption, congress engagement, payer and patient metrics) |

<!-- Life Sciences Addition -->

### Life Sciences Skills

| Skill | Description |
|---|---|
| `regulatory-compliance` | Promotional material classification, MLR review simulation, fair balance checker, off-label restriction compliance, FDA OPDP rules, and EMA advertising requirements |
| `medical-affairs-liaison` | MSL engagement planning, KOL mapping and tiering, advisory board planning, congress strategy, and the bridge between medical affairs and commercial marketing |

### Life Sciences Reference Documents

| Reference | Location | Description |
|---|---|---|
| FDA Promotional Rules | `skills/regulatory-compliance/references/fda-promotional-rules.md` | US FDA regulations governing pharmaceutical promotional materials, OPDP enforcement, digital guidance |
| EMA Requirements | `skills/regulatory-compliance/references/ema-requirements.md` | EU EMA advertising requirements, member state variations (Germany, France, UK, Italy, Spain), EFPIA Code |
| KOL Tier Framework | `skills/medical-affairs-liaison/references/kol-tier-framework.md` | Scoring methodology for KOL identification, evaluation, and tiering across 7 dimensions |
| Congress Planning Guide | `skills/medical-affairs-liaison/references/congress-planning-guide.md` | Detailed congress calendar, planning timeline, booth strategy, satellite symposium planning, competitive intelligence |

## Example Workflows

### Simulating an MLR Review

```
> /_mlr-review
[paste your promotional content]
Product: KEYTRUDA (pembrolizumab)
Market: US
```

Claude will classify the content, run medical, legal, and regulatory review checks, score fair balance, verify references, and provide a detailed findings report with severity ratings and compliant revision suggestions.

### Planning a Congress

```
> /_congress-plan
Congress: ASCO 2026
Product: KEYTRUDA (pembrolizumab), new adjuvant data
Objectives: Data dissemination, KOL engagement, competitive intelligence
Team size: 15 (5 MSLs, 6 commercial, 4 medical/leadership)
```

Claude will produce a complete congress plan covering booth strategy, KOL meeting schedule, satellite symposium outline, competitive intelligence assignments, social media plan, content repurposing plan, and post-congress activities — all with a week-by-week timeline.

### Developing a KOL Strategy

```
> /_kol-strategy
Therapeutic area: Non-small cell lung cancer (NSCLC)
Objective: Pre-launch market shaping for new IO combination
Geography: US national
Timeline: 18-month plan
```

Claude will identify KOLs through publication and clinical trial research, apply the tiering framework, and deliver an engagement plan covering advisory boards, speaker programs, MSL deployment, congress engagement, and measurement metrics.

### Drafting Compliant Promotional Content

```
> /_draft-content
Type: branded sales aid
Product: TECENTRIQ (atezolizumab) for NSCLC
Audience: Oncologists
Key messages: PFS improvement in first-line setting, manageable safety profile
```

Claude will draft an MLR-ready detail aid with properly annotated claims, fair-balanced efficacy and safety presentation, ISI section, and reference list — ready for internal review before formal MLR submission.

## Configuration

Configure your brand voice, style guide, product information, and target HCP personas in a local settings file for personalized output. For life sciences use, also configure:
- Approved indication statements
- ISI text (Important Safety Information)
- Approved claims library with reference annotations
- KOL target lists and tier assignments
- Congress calendar and priorities

## MCP Integrations

> If you see unfamiliar placeholders or need to check which tools are connected, see [CONNECTORS.md](CONNECTORS.md).

### Base Marketing Integrations

- **Slack** — Share drafts, reports, and briefs with your team
- **Canva** — Create and edit design assets
- **Figma** — Access design files and brand assets
- **HubSpot** — Pull campaign data, manage contacts, and track marketing automation
- **Amplitude** — Pull product analytics and user behavior data for performance reporting
- **Notion** — Access briefs, style guides, and campaign documents
- **Ahrefs** — SEO keyword research, backlink analysis, and site audits
- **Similarweb** — Competitive traffic analysis and market benchmarking
- **Klaviyo** — Draft and review email marketing sequences and campaigns

<!-- Life Sciences Addition -->

### Life Sciences Integrations

- **PubMed** — Search biomedical literature for reference verification, KOL publication analysis, and competitive intelligence
- **ClinicalTrials.gov** — Search clinical trial registrations for competitive pipeline intelligence, KOL identification, and trial comparison
- **OpenFDA** — Access drug labeling, adverse event data, and regulatory action history
- **Veeva** — CRM integration for HCP engagement tracking, approved email, and content management (requires Veeva CRM license)
