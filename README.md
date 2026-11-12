# SEO Skills for Claude and AI Agents

**25 SEO and Local SEO skills built from real client work.** Technical SEO, on-page, keyword research, content, Google Business Profile, reviews, citations, link building, Search Console analysis, reporting and AI search (GEO / AEO).

Built for Claude Code, Claude, Codex, Cursor and any agent that supports the Agent Skills (`SKILL.md`) format.

![Skills](https://img.shields.io/badge/skills-25-blue) ![License: MIT](https://img.shields.io/badge/license-MIT-green) ![Focus](https://img.shields.io/badge/focus-Local%20SEO-orange)

---

## Why this repo is different

Most SEO skill packs look impressive until you point them at a real website. These skills are written the way a senior SEO actually works with clients:

- **No invented data.** Skills never make up traffic, rankings, search volumes or authority scores. Unknown means "not measured".
- **Evidence first.** Every finding must show the URL and what was seen.
- **Bot-block aware.** If a site returns a bot check, CAPTCHA or 403, the skill stops and asks for an export instead of writing a fake audit.
- **First-party data first.** Google Search Console, GA4 and GBP data beat third-party estimates.
- **Token friendly.** Skills sample page templates instead of crawling everything and do not start sub-agents unless you ask.
- **Guideline safe.** No keyword-stuffed GBP names, fake reviews, doorway pages or bought links.
- **Local SEO depth.** Built for local service businesses (roofing, HVAC, plumbing, junk removal, real estate and more), and it works for any website.

---

## How the skills work together

```
                 ┌───────────────────────────┐
                 │    seo-client-context     │
                 │(read by every skill first)│
                 └─────────────┬─────────────┘
       ┌───────────────┬───────┴───────┬────────────────┬───────────────┐
       ▼               ▼               ▼                ▼               ▼
  Audit & Tech    Keywords &      On-page &        Local SEO       Data, Links
                  Strategy        Content                          & AI Search
  seo-audit       keyword-        on-page-seo      local-seo-      search-console-
  technical-seo   research        content-brief    audit           analysis
  site-           keyword-        seo-content-     google-business seo-reporting
  architecture    cannibalization writing          -profile        link-building
  schema-markup   competitor-     content-refresh  service-pages   ai-search-
  site-migration  analysis        internal-linking location-pages  optimization
                  content-strategy                 local-citations
                                                   review-management
```

Run `seo-client-context` once per website. It creates `.agents/seo-context.md` with the business details (NAP, services, cities, competitors, goals, data access). Every other skill reads it, so you never repeat yourself and nothing is guessed.

---

## Available skills

### Foundation
| Skill | What it does |
|---|---|
| [seo-client-context](skills/seo-client-context/SKILL.md) | Creates the business context file every other skill reads |

### Audit and Technical SEO
| Skill | What it does |
|---|---|
| [seo-audit](skills/seo-audit/SKILL.md) | Full SEO audit with an evidence-based, prioritized fix list |
| [technical-seo](skills/technical-seo/SKILL.md) | Crawling, indexing, canonicals, redirects, rendering, Core Web Vitals |
| [site-architecture](skills/site-architecture/SKILL.md) | Page tree, URL structure, hubs, navigation, redirect maps |
| [schema-markup](skills/schema-markup/SKILL.md) | Valid JSON-LD for LocalBusiness subtypes, Service, Breadcrumb, Article |
| [site-migration](skills/site-migration/SKILL.md) | Redesigns, platform and domain changes without losing rankings |

### Keywords and Strategy
| Skill | What it does |
|---|---|
| [keyword-research](skills/keyword-research/SKILL.md) | Intent, clustering and keyword-to-page mapping, local keywords |
| [keyword-cannibalization](skills/keyword-cannibalization/SKILL.md) | Finds pages competing for the same intent and fixes them |
| [competitor-analysis](skills/competitor-analysis/SKILL.md) | SERP and map pack competitor gaps, turned into actions |
| [content-strategy](skills/content-strategy/SKILL.md) | Topical maps, clusters and a content calendar that drives leads |

### On-page and Content
| Skill | What it does |
|---|---|
| [on-page-seo](skills/on-page-seo/SKILL.md) | Page-level optimization with exact title, meta and heading rewrites |
| [content-brief](skills/content-brief/SKILL.md) | Writer-ready briefs based on SERP analysis |
| [seo-content-writing](skills/seo-content-writing/SKILL.md) | Human, expert, people-first content with no AI filler |
| [content-refresh](skills/content-refresh/SKILL.md) | Finds decaying pages and brings them back |
| [internal-linking](skills/internal-linking/SKILL.md) | Link suggestions with anchors, placement and confidence scores |

### Local SEO
| Skill | What it does |
|---|---|
| [local-seo-audit](skills/local-seo-audit/SKILL.md) | Map pack audit: GBP, reviews, citations, local pages, competitors |
| [google-business-profile](skills/google-business-profile/SKILL.md) | GBP optimization, ready-to-paste description, services and posts |
| [service-pages](skills/service-pages/SKILL.md) | Money pages that rank for "service + city" and convert |
| [location-pages](skills/location-pages/SKILL.md) | City pages with real local value, not doorway pages |
| [local-citations](skills/local-citations/SKILL.md) | NAP standard, citation audit and listing tracker |
| [review-management](skills/review-management/SKILL.md) | Compliant review generation and reply templates |

### Data, Links and AI Search
| Skill | What it does |
|---|---|
| [search-console-analysis](skills/search-console-analysis/SKILL.md) | Quick wins, CTR gaps, declines and indexing issues from GSC |
| [seo-reporting](skills/seo-reporting/SKILL.md) | Monthly client reports in plain language, focused on leads |
| [link-building](skills/link-building/SKILL.md) | Local and earned link opportunities plus outreach templates |
| [ai-search-optimization](skills/ai-search-optimization/SKILL.md) | Visibility in AI Overviews, ChatGPT, Perplexity, Gemini and Claude |

---

## Installation

### Option 1: Skills CLI (recommended)

```bash
# Install all skills
npx skills add AmmarBabbar/seo-skills

# Install for Claude Code specifically
npx skills add AmmarBabbar/seo-skills -a claude-code

# Install only some skills
npx skills add AmmarBabbar/seo-skills --skill seo-audit local-seo-audit
```

### Option 2: Claude Code plugin

```bash
/plugin marketplace add AmmarBabbar/seo-skills
/plugin install seo-skills@ammarbabbar-seo
```

### Option 3: Clone and copy

```bash
git clone https://github.com/AmmarBabbar/seo-skills.git
# For all your projects
cp -r seo-skills/skills/* ~/.claude/skills/
# Or for one project only
cp -r seo-skills/skills/* .claude/skills/
```

### Option 4: Claude app (claude.ai)

Zip a skill folder (for example `skills/local-seo-audit`) and upload it in Claude under **Customize > Skills > Upload a skill**. Code execution must be enabled for your account.

---

## Usage

Just describe the task. The right skill loads automatically:

```
"Audit example.com and tell me what to fix first"            → seo-audit
"Why is my roofing client not in the map pack in Plano?"      → local-seo-audit
"Write a service page for AC repair in Dallas"               → service-pages
"Here is my Search Console export, find quick wins"          → search-console-analysis
"Which cities should get their own location page?"           → location-pages
"Write this month's SEO report for my client"                → seo-reporting
```

Or call a skill directly in Claude Code: `/seo-audit`, `/local-seo-audit`, `/keyword-research`.

---

## Better data = better results

These skills work without paid tools, but real data makes them much stronger:

- **Google Search Console**: export data every 7 days, or connect it with an MCP server such as [mcp-gsc](https://github.com/AminForou/mcp-gsc) (needs a Google Cloud project, the Search Console API and OAuth credentials).
- **Keyword and backlink data**: Ahrefs, Semrush, or pay-as-you-go APIs like DataForSEO.
- **Local rank grids**: Local Falcon, BrightLocal or similar.

Always double-check AI output before you send it to a client. The skills are built to be honest about what they do not know, but you are still the SEO.

---

## Contributing

Found a better way to do something, or want to add a skill? Open an issue or a pull request. Each skill lives in `skills/{skill-name}/SKILL.md` with YAML frontmatter (`name`, `description`) followed by the instructions.

---

## About the author

**Ammar Babbar** is a Senior SEO Expert with 5+ years of hands-on experience, specializing in Local SEO for roofing, AC repair, junk removal, real estate and other local service businesses. BS Computer Science (NCBA&E Lahore).

- LinkedIn: [in/ammar-babbar](https://www.linkedin.com/in/ammar-babbar)
- YouTube: [Ammar Babbar Tips](https://www.youtube.com/@AmmarBabbarTips)
- GitHub: [@AmmarBabbar](https://github.com/AmmarBabbar)

If these skills help you, please give the repo a star.

## License

[MIT](LICENSE). Use them however you want.
