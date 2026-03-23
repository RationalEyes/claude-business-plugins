# Connectors

## How tool references work

Plugin files use `~~category` as a placeholder for whatever tool the user connects in that category. For example, `~~marketing automation` might mean HubSpot, Marketo, or any other marketing platform with an MCP server.

Plugins are **tool-agnostic** — they describe workflows in terms of categories (design, SEO, email marketing, etc.) rather than specific products. The `.mcp.json` pre-configures specific MCP servers, but any MCP server in that category works.

## Connectors for this plugin

| Category | Placeholder | Included servers | Other options |
|----------|-------------|-----------------|---------------|
| Chat | `~~chat` | Slack | Microsoft Teams |
| Design | `~~design` | Canva, Figma | Adobe Creative Cloud |
| Marketing automation | `~~marketing automation` | HubSpot | Marketo, Pardot, Mailchimp |
| Product analytics | `~~product analytics` | Amplitude | Mixpanel, Google Analytics |
| Knowledge base | `~~knowledge base` | Notion | Confluence, Guru |
| SEO | `~~SEO` | Ahrefs, Similarweb | Semrush, Moz |
| Email marketing | `~~email marketing` | Klaviyo | Mailchimp, Brevo, Customer.io |

<!-- Life Sciences Addition -->

## Life sciences connectors

| Category | Placeholder | Included servers | Other options |
|----------|-------------|-----------------|---------------|
| Biomedical literature | `~~biomedical literature` | PubMed (NCBI) | Embase, Cochrane Library, Google Scholar |
| Clinical trials data | `~~clinical trials data` | ClinicalTrials.gov | EU Clinical Trials Register, WHO ICTRP |
| Drug safety and labeling | `~~drug safety and labeling` | OpenFDA | DailyMed, EMA medicines database |
| CRM (life sciences) | `~~life sciences CRM` | Veeva CRM | IQVIA OCE, Salesforce Health Cloud |
| MLR review platform | `~~MLR review` | — | Veeva Vault PromoMats, Zinc Ahead |
| Prescribing data | `~~prescribing data` | — | IQVIA, Symphony Health, Komodo Health |
| Formulary data | `~~formulary data` | — | MMIT, Fingertip Formulary, Elsevier Gold Standard |
| Medical education | `~~medical education` | — | Medscape, DocCheck, Coliquio, Doximity |
| Competitive intelligence | `~~competitive intelligence` | — | EvaluatePharma, GlobalData, Citeline |
