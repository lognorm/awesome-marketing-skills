# Awesome Marketing Skills

> A curated list of awesome marketing skills, resources, and tools for getting marketing, copy, and distribution done through any LLM - Claude, ChatGPT, Manus, Codex, and similar agents.

[![Awesome](https://awesome.re/badge-flat.svg)](https://github.com/sindresorhus/awesome)
[![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat-square)](CONTRIBUTING.md)
[![License: MIT](https://img.shields.io/badge/license-MIT-yellow.svg?style=flat-square)](LICENSE)
[![Link check](https://github.com/mikiarlo3/awesome-marketing-skills/actions/workflows/link-check.yml/badge.svg)](https://github.com/mikiarlo3/awesome-marketing-skills/actions/workflows/link-check.yml)

**This is a selective catalog, not a directory dump.** Every listed entry has a canonical source, a clear marketing use case, and an explicit note about portability or external side effects. A `SKILL.md` package may be portable across Agent Skills-compatible hosts, but a host-specific plugin, MCP connector, installer, or script bundle must be assessed separately.[11] [12] [13] [14]

## Contents

- [Start here](#start-here)
- [Install safely](#install-safely)
- [Skills and collections](#skills-and-collections)
  - [Full-stack marketing](#full-stack-marketing)
  - [Copy and messaging](#copy-and-messaging)
  - [Content, SEO, and AI search](#content-seo-and-ai-search)
  - [Campaigns and measurement](#campaigns-and-measurement)
  - [Social and distribution](#social-and-distribution)
  - [Advanced automation](#advanced-automation)
- [Platforms, formats, and tools](#platforms-formats-and-tools)
- [Help make this list better](#help-make-this-list-better)
- [Safety and responsible use](#safety-and-responsible-use)
- [References](#references)

## Start here

If you want a practical default stack, start with **Marketing Skills for AI Agents** for broad strategy, copy, SEO, CRO, analytics, and growth work. Add **AI Copywriter** for a portable, focused copy workflow, then add **Social Media Skills** or **Claude Blog** only when you need channel-specific production. Use a connector-heavy package only after you understand what it can read, write, send, publish, or schedule.[2] [3] [5] [6]

| Need | Recommended starting point | Why it is useful |
|---|---|---|
| General marketing operating system | [Marketing Skills for AI Agents](https://github.com/coreyhaines31/marketingskills) | Broad library for product context, conversion, copy, search, analytics, and growth work.[2] |
| Claude-native marketing workflows | [Anthropic Marketing Plugin](https://github.com/anthropics/knowledge-work-plugins/tree/main/marketing) | Official role plugin for content, campaigns, brand, research, and performance work.[1] |
| Copy and brand voice | [AI Copywriter](https://github.com/mikiarlo3/ai-copywriter) | User-nominated portable copywriting skill with explicit Claude, ChatGPT, and Manus setup paths.[3] |
| Blog production and search visibility | [Claude Blog](https://github.com/AgriciDaniel/claude-blog) | End-to-end blog, SEO, GEO, quality, and repurposing workflow suite.[6] |
| Social distribution | [Social Media Skills](https://github.com/blacktwist/social-media-skills) | Focused social strategy, creation, repurposing, and analytics skills.[5] |
| AI-search and SEO work | [GEO SEO Claude](https://github.com/zubair-trabzada/geo-seo-claude) | Specialist collection for AI-search visibility, citability, schema, and technical SEO.[4] |

## Install safely

> **Read the complete skill folder before you install it.** A skill is not always just Markdown: it can include scripts, assets, APIs, MCP configurations, credentials, web access, telemetry, or publication tools. Manus explicitly warns that community skills can contain code and shell commands, while the Agent Skills standard permits optional scripts, references, and assets.[11] [14]

Use the following sequence before activating a new package:

1. **Verify the canonical source.** Prefer the project linked from this list rather than a fork, mirror, or repost.
2. **Read `SKILL.md`, installation files, scripts, and configuration.** Do not run `curl | bash` installers or grant credentials until you understand their scope.
3. **Install the smallest useful unit.** Prefer one skill over a full bundle, especially when it includes sending, publishing, advertising, CRM, or browser automation.
4. **Start in a non-production workspace.** Use sample or non-sensitive data first, and confirm that outputs match your brand and factual standards.
5. **Keep external actions human-approved.** Publishing, sending messages, changing ad spend, importing contacts, and modifying CRM records should require a deliberate review step.

### Compatibility at a glance

| Host or format | What to expect | Practical advice |
|---|---|---|
| **Claude** | Claude supports Agent Skills-style `SKILL.md` folders across its documented surfaces. Claude plugins can additionally include commands, agents, and connector configuration.[12] | Treat a plugin with connectors as more than a portable instruction skill. Review its permissions before install. |
| **ChatGPT and Codex** | Codex documents Agent Skills and broader plugins. A ChatGPT workflow may instead be distributed as Custom GPT instructions or uploaded reference material, as the package author documents.[3] [13] | Do not assume a Claude plugin will import unchanged. Follow the package's host-specific instructions. |
| **Manus** | Manus supports skills through its Skills UI, local folder/ZIP/`.skill` upload, official library, and GitHub import, and it recognizes the Agent Skills format.[14] | Inspect every included script and install a test copy first. |
| **Agent Skills-compatible hosts** | The open format is built around `SKILL.md` with optional scripts, references, and assets.[11] | Treat portability as likely only when the target host supports the format and the package has no host-specific dependencies. |
| **MCP and connectors** | MCP is an external integration pattern, not a passive instruction skill. Tools may read data or take actions in connected services.[17] | Evaluate it separately, grant least privilege, and require approval for side effects. |

## Skills and collections

### Full-stack marketing

| Project | What it helps with | Format and documented hosts | Review note |
|---|---|---|---|
| [Anthropic Marketing Plugin](https://github.com/anthropics/knowledge-work-plugins/tree/main/marketing) | Content drafting, campaign planning, brand review, competitive briefs, performance reports, SEO audits, and email sequences.[1] | Official Claude role plugin for Cowork and Claude Code. It can use integrations such as HubSpot, Amplitude, Notion, Ahrefs, Similarweb, Klaviyo, Slack, Canva, and Figma.[1] | **Connector-capable.** Install only integrations you need and review OAuth or tool permissions. |
| [Marketing Skills for AI Agents](https://github.com/coreyhaines31/marketingskills) | Product marketing context, CRO, copy, SEO and AI SEO, analytics, retention, RevOps, GTM, launch, research, pricing, and distribution workflows.[2] | MIT-licensed Agent Skills collection documented for Claude Code, Codex, Cursor, Windsurf, and compatible hosts.[2] | **Best broad starting point.** Review optional tools and do not let a workflow act on ads, CRM, or websites without approval. |
| [Marketing Team Skills Collection](https://github.com/alirezarezvani/claude-skills/tree/main/marketing-skill) | Content production, demand generation, product marketing strategy, app-store optimization, social analysis, and campaign analytics.[7] | Multi-agent bundle with published install paths for Claude Code, Cursor, VS Code, Copilot, Goose, Amp, and Codex.[7] | Includes Python tooling. Test data sources and do not treat upstream performance benchmarks as independently verified. |
| [Running Marketing Campaigns](https://github.com/SpillwaveSolutions/running-marketing-campaigns-agent-skill) | Campaign planning, UTM governance, content, email, social, brand voice, SEO/GEO, and measurement.[8] | Portable Agent Skill with documented installer and manual routes for Claude Code, Codex, OpenCode, Gemini, and other listed hosts.[8] | Small, focused project with local Python utilities. Inspect before running and validate tracking output against your analytics conventions. |

### Copy and messaging

| Project | What it helps with | Format and documented hosts | Review note |
|---|---|---|---|
| [AI Copywriter](https://github.com/mikiarlo3/ai-copywriter) | Headlines, short descriptions, microcopy, subject lines, LinkedIn posts, editing, humanizing text, and brand-voice calibration.[3] | Portable `SKILL.md` package with a Claude plugin directory. Its README describes routes for Claude Code, Claude Projects, ChatGPT Custom GPT instructions, and Manus attachment/import workflows.[3] | **User-nominated entry.** It is an early-stage project, so inspect its scripts and supporting files before installation. |
| [Marketing Skills for AI Agents - copywriting and copy editing](https://github.com/coreyhaines31/marketingskills/tree/main/skills) | Marketing-page copywriting, editing, cold email, email, social, video, and image-related workflows.[2] | Individual Agent Skills inside the broader collection.[2] | Start with product-marketing context, then install only the relevant writing skills. |

### Content, SEO, and AI search

| Project | What it helps with | Format and documented hosts | Review note |
|---|---|---|---|
| [GEO SEO Claude](https://github.com/zubair-trabzada/geo-seo-claude) | AI-search visibility, citability, crawler checks, `llms.txt`, brand mentions, schema, technical audits, content audits, reports, and proposal workflows.[4] | MIT-licensed Agent Skills collection with a primary skill, sub-skills, agents, scripts, templates, and tests.[4] | Its upstream installer uses a remote shell pipeline and the project may retain working data locally. Prefer manual review and a disposable test environment. |
| [Claude Blog](https://github.com/AgriciDaniel/claude-blog) | Blog strategy, outlines, writing, rewrites, SEO, AI-citation readiness, schema, quality review, topic clusters, localization, decay detection, assets, and repurposing.[6] | Claude Code skill suite with an orchestrator, sub-skills, agents, scripts, tests, and optional integrations.[6] | Advanced package. Inspect installers, dependencies, external integrations, and publishing flows before use. |
| [OpenClaudia - SEO and content skills](https://github.com/OpenClaudia/openclaudia-skills) | SEO audit, keyword and SERP research, schema, programmatic SEO, content writing, landing-page copy, briefs, gap analysis, and repurposing.[10] | CLI and modular skill library.[10] | Install individual skills instead of the whole suite when practical. Some entries require API keys or external data providers. |

### Campaigns and measurement

| Project | What it helps with | Format and documented hosts | Review note |
|---|---|---|---|
| [Running Marketing Campaigns](https://github.com/SpillwaveSolutions/running-marketing-campaigns-agent-skill) | GA4-aligned UTM creation and validation, brand checking, marketing calendar planning, launch frameworks, and ROI/attribution references.[8] | A single Agent Skill with local Python utilities.[8] | Good fit when you want a smaller, inspectable campaign workflow. Validate any CSV or URL output before production use. |
| [AI Marketing Skills](https://github.com/ericosiu/ai-marketing-skills) | Growth experiments, revenue intelligence, conversion work, content operations, SEO operations, pipeline analysis, and reporting.[9] | Script-heavy coding-agent workflows with `SKILL.md` files, Python dependencies, API-key setup, optional telemetry, and security utilities.[9] | **Advanced automation.** Use least-privilege credentials, evaluate telemetry, and keep data handling and execution under human control. |
| [OpenClaudia - analytics and research skills](https://github.com/OpenClaudia/openclaudia-skills) | GA4, Search Console, Ads reporting, YouTube, brand and competitive research, and AI-citation reporting.[10] | API-backed modular skills.[10] | Review API scope, costs, and data retention. Use test accounts where possible. |

### Social and distribution

| Project | What it helps with | Format and documented hosts | Review note |
|---|---|---|---|
| [Social Media Skills](https://github.com/blacktwist/social-media-skills) | Social context, content strategy, calendars, platform strategy, posts, threads, carousel scripts, captions, repurposing, hooks, performance analysis, and growth tracking.[5] | MIT Agent Skills collection with Skills CLI, manual, Claude Cowork ZIP, and multi-agent installation guidance.[5] | In advisory mode it generates guidance. With its optional BlackTwist MCP it can publish, schedule, fetch analytics, and manage drafts. Keep live publishing disabled until each action is reviewed. |
| [Marketing Skills for AI Agents - distribution skills](https://github.com/coreyhaines31/marketingskills/tree/main/skills) | Social, video, images, community, influencer, referrals, co-marketing, lead magnets, directory submissions, launches, and outbound-supporting workflows.[2] | Individual skills from the broad collection.[2] | Use authentic, consent-respecting distribution practices. Do not automate spam, fake engagement, or deceptive reviews. |
| [AI Marketing Skills - content and media operations](https://github.com/ericosiu/ai-marketing-skills) | Podcast repurposing, video captions, video clips, long-form social content, and YouTube competitive analysis.[9] | Script-backed skill directories.[9] | Review external accounts, source rights, and data processing before execution. |
| [OpenClaudia - social and outreach skills](https://github.com/OpenClaudia/openclaudia-skills) | Social content, LinkedIn, threads, community channels, email sequences, marketing automation, CRM, and outreach workflows.[10] | Modular skills plus live API integrations.[10] | **Potentially high impact.** Do not enable sending, posting, contact enrichment, or CRM changes without explicit human approval and compliance review. |

### Advanced automation

These packages are worthwhile for experienced technical marketers, but they are **not** default installations because they can use API keys, ingest business data, send messages, publish posts, modify records, or automate multi-step operations.

| Project | Why it is here | Why it needs additional review |
|---|---|---|
| [AI Marketing Skills](https://github.com/ericosiu/ai-marketing-skills) | Complete workflows for experiment design, content operations, revenue intelligence, conversion, analytics, and pipeline support.[9] | It includes Python dependencies, environment variables, optional telemetry, and workflows that may touch prospect or revenue data.[9] |
| [OpenClaudia](https://github.com/OpenClaudia/openclaudia-skills) | Large open marketing toolkit spanning search, content, ads, social, analytics, CRM, outreach, assets, and growth.[10] | It documents numerous external APIs and write-capable functions such as email, social publishing, webhooks, and CRM access.[10] |

## Platforms, formats, and tools

| Resource or tool | Why it belongs in this list |
|---|---|
| [Agent Skills Specification](https://agentskills.io/specification) | The open `SKILL.md` package model behind many portable skills. It explains the core directory structure and optional scripts, references, and assets.[11] |
| [Claude Agent Skills Documentation](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview) | Canonical documentation for Claude skill architecture and deployment surfaces.[12] |
| [OpenAI Codex Skills Documentation](https://developers.openai.com/codex/skills) | Explains the distinction between portable skills and broader plugins in Codex.[13] |
| [Manus Skills Documentation](https://manus.im/docs/features/skills) | Covers discovery, installation, GitHub import, management, and safety considerations for Manus skills.[14] |
| [Vercel Skills CLI](https://github.com/vercel-labs/skills) | A maintained tool for finding and adding Agent Skills-compatible packages. Inspect an upstream package before executing its installation command.[15] |
| [Composio Marketing Skills Overview](https://composio.dev/content/best-marketing-skills) | Useful discovery map for marketing categories and potential connected workflows. Follow links to the canonical project and review each integration individually.[16] |
| [MCP Tools Specification](https://modelcontextprotocol.io/specification/2025-06-18/server/tools) | Helps distinguish an MCP integration with external-service access from an instruction-only skill.[17] |

## Help make this list better

**Contributions are welcome.** The list gets better when practitioners add a real skill they have tested, report an unsafe installer, correct a stale compatibility claim, or explain a concrete marketing workflow that an LLM can perform well.

A strong contribution is specific. It identifies the canonical source, says what the skill actually helps a marketer do, names the packaging format and documented host(s), and calls out scripts, credentials, MCP connections, live publishing, or other side effects. Please do not submit a generic prompt collection, a cloned duplicate, a paywalled tool without a meaningful skill layer, or a project that encourages spam, deception, fake engagement, or unauthorized scraping.

### Fast contribution path

1. Fork this repository and create a focused branch, such as `add-social-analytics-skill`.
2. Add the entry to the most relevant table in `README.md`, keeping entries concise and linked to their canonical source.
3. Include a numeric reference in the References section. For a new source, explain its quality, licensing, documented host compatibility, and any installation or side-effect risks in your pull request.
4. Add or update a row in [`catalog-validation.csv`](catalog-validation.csv) so reviewers can audit the selection.
5. Run `git diff --check`, make sure links work, and open a pull request using the repository template.
6. In the pull request description, state whether you personally tested the skill, on which host, and whether it read data, wrote data, sent messages, published content, used paid APIs, or required credentials.

If you have a promising project but need help deciding where it belongs, open a [new entry request](.github/ISSUE_TEMPLATE/new-entry.md). Small documentation fixes and safety corrections are especially welcome.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the complete standard.

## Safety and responsible use

This repository links to third-party packages and does **not** execute, audit, endorse, or guarantee them. Marketing agents should preserve human accountability for factual claims, brand voice, consent, privacy, deliverability, advertising rules, and customer data. Keep a reviewer in the loop for anything that sends, posts, purchases, changes budgets, creates public content, writes to a CRM, or processes personal information.

> A marketing skill should make good work faster, not make irresponsible automation easier.

## References

[1]: https://github.com/anthropics/knowledge-work-plugins/tree/main/marketing "Anthropic Marketing Plugin"
[2]: https://github.com/coreyhaines31/marketingskills "Marketing Skills for AI Agents"
[3]: https://github.com/mikiarlo3/ai-copywriter "AI Copywriter"
[4]: https://github.com/zubair-trabzada/geo-seo-claude "GEO SEO Claude"
[5]: https://github.com/blacktwist/social-media-skills "Social Media Skills"
[6]: https://github.com/AgriciDaniel/claude-blog "Claude Blog"
[7]: https://github.com/alirezarezvani/claude-skills/tree/main/marketing-skill "Marketing Team Skills Collection"
[8]: https://github.com/SpillwaveSolutions/running-marketing-campaigns-agent-skill "Running Marketing Campaigns"
[9]: https://github.com/ericosiu/ai-marketing-skills "AI Marketing Skills"
[10]: https://github.com/OpenClaudia/openclaudia-skills "OpenClaudia"
[11]: https://agentskills.io/specification "Agent Skills Specification"
[12]: https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview "Claude Agent Skills Documentation"
[13]: https://developers.openai.com/codex/skills "OpenAI Codex Skills Documentation"
[14]: https://manus.im/docs/features/skills "Manus Skills Documentation"
[15]: https://github.com/vercel-labs/skills "Vercel Skills CLI"
[16]: https://composio.dev/content/best-marketing-skills "Composio Marketing Skills Overview"
[17]: https://modelcontextprotocol.io/specification/2025-06-18/server/tools "MCP Tools Specification"
