# Pitchpath — Project Context

## What This Is

Pitchpath (getpitchpath.com) is a **done-for-you quiz funnel service**. We custom-build interactive quiz funnels for clients — the quiz, the branching logic, the funnel architecture, and every follow-up email sequence. The client gets a complete conversion system. We do the work.

**This is NOT a SaaS product, NOT a tool, NOT a platform.** It is a premium service business. Every quiz funnel is custom-built from scratch — no templates, no third-party quiz builders.

## Critical Brand Rules

- Never use SaaS language: "platform," "tool," "software," "sign up," "free trial," "get started," "template," "drag-and-drop," "no-code"
- Never use consultant-speak: "implement," "onboard," "deploy," "solution," "stakeholders"
- Never use marketing clichés: "leverage," "unlock," "empower," "seamless," "revolutionary," "game-changing," "delight"
- CTAs are always service-oriented: "Book a Strategy Call," "Take the Scorecard," "See Our Work" — never "Learn More" alone
- Voice is direct-response operator: confident, numerical, plain-English, short sentences as hammers
- We position against DIY tools (Typeform, Interact, ScoreApp), not against other services
- Never justify the price or apologize for being a service

## Brand Foundation

All brand context lives in `./brand/`. Read these files before any marketing, copy, or creative work:

| File | What It Contains |
|------|-----------------|
| `voice-profile.md` | Complete voice DNA — tone, vocabulary, rhythm, platform adaptations, signature patterns |
| `positioning.md` | 5 positioning angles, competitive landscape, naming, downstream skill notes |
| `creative-kit.md` | Visual identity — colors (#0F172A base, #F97316 accent, #22C55E metrics), typography (Syne/DM Sans/JetBrains Mono), design rules |
| `stack.md` | Connected tools and MCP servers |
| `assets.md` | Registry of all created assets |
| `learnings.md` | Accumulated performance learnings (append-only) |

## Project Structure

```
./brand/                    Brand memory (read by all Vibe Marketing Skills)
./campaigns/                Campaign assets
  quiz-funnel-scorecard/    Lead magnet — the Quiz Funnel Scorecard
    lead-magnet.md          Full quiz: 11 questions, 5 result profiles, scoring logic, segment blueprints
    brief.md                Campaign brief
  getpitchpath-launch/      Main site launch
    landing-page.md         Landing page copy (control variant)
    brief.md                Campaign brief
./site/                     Website files
  index.html                Landing page for getpitchpath.com (single HTML, production-ready)
```

## Key Decisions Made

- **Name:** Pitchpath
- **Domain:** getpitchpath.com
- **Primary positioning:** "The Done-For-You Conversion Experience" — every competitor is a DIY tool, we are the service
- **Lead magnet:** The Quiz Funnel Scorecard — an interactive quiz that demonstrates the product (eat your own cooking)
- **Visual identity:** Dark-first design (Deep Navy #0F172A), Pitch Orange (#F97316) for CTAs, Proof Green (#22C55E) for metrics
- **Target niches for cold outreach:** Medspas (first), course creators, e-commerce (skincare/supplements), real estate, financial advisors, wedding industry
- **Dual CTA strategy:** Scorecard (soft/lead capture) + Strategy Call (hard/direct sales)

## Vibe Marketing Skills

The Vibe Marketing Skills v2 suite is installed globally at `~/.claude/skills/`. These skills read from `./brand/` for context. Available skills:

- `/start-here` — Orchestrator, project scan, routing
- `/brand-voice` — Voice profile extraction or building
- `/positioning-angles` — Market positioning and angles
- `/direct-response-copy` — Landing pages, emails, ads, sales copy
- `/keyword-research` — SEO keyword strategy
- `/seo-content` — Long-form SEO content
- `/email-sequences` — Email automations and nurture sequences
- `/lead-magnet` — Lead magnet ideation and building
- `/newsletter` — Newsletter design and editions
- `/content-atomizer` — Repurpose content across platforms
- `/creative` — AI image, video, ad creative generation (needs Replicate API token)

## What Still Needs Building

- Email follow-up sequences for the 5 scorecard result tiers (next: `/email-sequences`)
- Social content to drive traffic (next: `/content-atomizer`)
- The actual interactive quiz implementation (custom web build)
- Case studies and testimonials (replace industry benchmarks on landing page once available)
- Pricing structure (not yet defined)
