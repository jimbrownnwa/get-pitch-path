# Campaign: Scorecard Follow-Up Sequences

## Goal
Convert Quiz Funnel Scorecard leads into booked strategy calls. Primary metric: call bookings per 100 scorecard completions by tier. Secondary: reply rate on sequence (signals engagement even when a call isn't booked yet).

## Sequence Type
5 parallel sequences — one per scorecard result tier. Each receives a different cadence, tone, and CTA strategy.

| Tier | Score | Emails | Length | Tone | Primary CTA |
|------|-------|--------|--------|------|-------------|
| Goldmine | 40-50 | 6 | 10 days | Urgency + math | Book Strategy Call |
| Ready Launcher | 30-39 | 6 | 10 days | Confident + direct | Book Strategy Call |
| Segmentation Opportunity | 22-29 | 6 | 14 days | Educational + ROI | See How It Works |
| Foundation Builder | 15-21 | 6 | 30 days | Nurture + patient | Reply with Question |
| Early Explorer | 10-14 | 6 | 30 days | Curious + low pressure | Keep Reading |

Total: 30 emails across 5 sequences.

## Angle
The Done-For-You Conversion Experience. Every sequence reinforces that Pitchpath is a service, not a tool — and that the quiz funnel being used to capture these leads IS the demo.

## Audience Segment
Course creators, coaches, e-commerce/DTC brands, local service businesses (medspa/dental/salons), and agencies. Q1 of the scorecard segments these by tag: `segment:creator | segment:ecom | segment:local | segment:coach | segment:agency`. Each email uses dynamic segment variables where relevant.

## Lead Magnet
The Quiz Funnel Scorecard — 11 questions, 5 result tiers, segment-specific blueprints. Scorecard delivered immediately at quiz completion; these sequences fire from that moment.

## Paid Offer
Pitchpath done-for-you quiz funnel build — custom quiz, branching logic, 3-5 result paths, full follow-up email sequences, integrated ESP wiring. 10 business days from strategy call to live. Pricing: premium service, TBD (strategy call scopes it).

## Bridge Logic
The scorecard quantifies the gap (projected revenue lost to weak conversion). The sequences walk the lead from "I saw the gap" → "I understand what would close it" → "I want to talk about having someone build it." The quiz itself is the proof that Pitchpath knows what it's doing.

## Timeline per Tier

**Goldmine (high urgency — ready to buy):**
Day 0 → Day 1 → Day 3 → Day 5 → Day 7 → Day 10

**Ready Launcher (same cadence, less urgency):**
Day 0 → Day 1 → Day 3 → Day 5 → Day 7 → Day 10

**Segmentation Opportunity (stretched for education):**
Day 0 → Day 2 → Day 4 → Day 6 → Day 9 → Day 14

**Foundation Builder (longer nurture):**
Day 0 → Day 2 → Day 5 → Day 9 → Day 16 → Day 30

**Early Explorer (patience + curiosity):**
Day 0 → Day 3 → Day 6 → Day 10 → Day 18 → Day 30

## ESP
HubSpot (MCP connected). Sequences deployable via HubSpot workflows using segment/tier/frustration tags set at quiz completion. Segment-variant logic handled in HubSpot conditional content or separate workflows per segment.

## Segmentation Tags Required at Quiz Completion
- `segment:{creator|ecom|local|coach|agency}`
- `tier:{goldmine|ready|segmentation|foundation|explorer}`
- `frustration:{leads|conversion|attribution|time|tools}`
- `ltv:{low|mid|high|premium|enterprise}`
- `spend:{zero|low|mid|high|heavy}`
- `diy:{never|considered|started|failed|working}`

## Dynamic Variables Used Throughout
- `{{first_name}}` — from opt-in
- `{{traffic}}` — Q2 answer (mapped to range label)
- `{{conversion_rate}}` — Q3 answer (mapped to %)
- `{{current_leads}}` — calculated: traffic × rate
- `{{projected_leads}}` — traffic × 18% (midpoint of 15-30%)
- `{{projected_revenue}}` — (projected_leads − current_leads) × ltv
- `{{ltv}}` — Q9 answer (mapped to dollar range)
- `{{segment_label}}` — e.g., "medspa," "course creator," "agency"
- `{{segment_noun}}` — e.g., "medspa owner," "creator," "founder"
- `{{segment_example}}` — one-line example of a similar business
- `{{frustration_verbatim}}` — Q7 answer, quoted
- `{{frustration_topic}}` — e.g., "lead quality," "conversion," "attribution"

## Status
draft — all 5 tiers written (30 emails total). Pending voice review, HubSpot workflow build, and deploy.

## Voice Notes
Direct-response operator per brand voice profile. Sentences as hammers. Numerical specificity in every email (dollar amounts, conversion rates, day counts). No SaaS language, no consultant-speak, no marketing clichés. CTAs service-oriented: "Book a Strategy Call," "See Our Work." Signed by "Jim" — edit to preferred sender name before deploying.

Never fake social proof. Pitchpath is new — no testimonials, case studies, or client names yet. Emails that would normally feature case studies instead use illustrative framing ("Picture a {{segment_example}} with your profile…") and industry-benchmark data. Landing page does the same — stay consistent.

## Next Steps
1. Review Goldmine tier for voice fit
2. Build remaining 4 tiers (Ready Launcher, Segmentation, Foundation, Explorer)
3. Wire HubSpot workflows with tag-based branching
4. Replace illustrative examples with real case studies once they exist (see brand/learnings.md)
