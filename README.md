# Claude Business Library

**Industry-specific AI plugin marketplace by [RationalEyes.ai](https://rationaleyes.ai)**

<!-- Add hero image: ![Claude Business Library](assets/hero.png) -->

A curated marketplace of plugins that bring regulatory compliance, domain expertise, and specialized workflows to Claude. Each plugin hardcodes the rules of its industry into the AI — so it works within the boundaries of your business, not against them.

## Available Plugins

| Plugin | Version | Industry | Handbook |
|--------|---------|----------|----------|
| [Marketing for Life Sciences](marketing-life-sciences/) | 1.0.0 | Pharma / Biotech / Medtech | [PDF](docs/marketing-life-sciences-handbook.pdf) · [Markdown](docs/marketing-life-sciences-handbook.md) |

## Add This Marketplace

### Claude Code

Add the marketplace, then browse and install plugins:

```bash
/plugin marketplace add RationalEyes/claude-business-library
```

Then install a plugin:

```bash
/plugin install marketing-life-sciences@claude-business-library
```

### Claude Cowork (Desktop)

**Option A — Add as marketplace:**
Plugins → Manage Plugins → Add marketplace from GitHub → enter `RationalEyes/claude-business-library` → browse and install plugins

**Option B — Install a single plugin directly:**
Download the plugin `.zip` from [Releases](https://github.com/RationalEyes/claude-business-library/releases) → Plugins → Manage Plugins → Upload Plugin → Approve

## How Plugins Work

Each plugin contains two types of capabilities:

- **Commands** (prefixed with `_`) — Explicit workflows you invoke with `/`. They only run when you call them. Example: `/_mlr-review` runs a medical-legal-regulatory review simulation.
- **Skills** (no prefix) — Context-triggered knowledge that Claude activates automatically when your conversation matches the skill's domain. Just describe what you need in plain language.

In Cowork, both appear in the same list when you tap `+` and select a plugin. The `_` prefix ensures commands sort to the top, giving you a visual separator: underscore = invoke explicitly; no underscore = Claude handles it automatically.

## Important Disclaimer

These plugins do not replace human review. There is no fully compliant AI running on autopilot in a regulated industry. These plugins act as a first-pass filter — they catch common errors so your compliance team is not wasting hours fixing generic AI output. They are a step toward making agentic AI more reliable in regulated environments.

## Request a Plugin

Have a specific industry or workflow that needs a customized plugin? Open an [issue](https://github.com/RationalEyes/claude-business-library/issues) describing your use case.

## Companion Resources

Handbooks covering Anthropic's built-in Cowork plugins (data, finance, legal, sales, productivity, and more):
[claude-cowork-plugin-handbooks](https://github.com/RationalEyes/claude-cowork-plugin-handbooks)

## About

Built by [RationalEyes.ai](https://rationaleyes.ai). The life sciences marketing plugin is derived from Anthropic's base marketing plugin under the Apache 2.0 license.

## License

Apache 2.0 — see [LICENSE](LICENSE).
