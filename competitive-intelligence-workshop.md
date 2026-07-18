---
name: pmm-workshop-competitive-intelligence
description: Run an ongoing competitive intelligence workshop for product marketers. Use this skill whenever the user wants to monitor the competitive landscape, understand how competitors are positioned, build a competitive overview for new employees or sales teams, create a comparison chart across competitors, or produce kill sheets for specific competitors. Trigger on phrases like "competitive landscape", "monitor competitors", "competitive overview", "kill sheet", "comp intel", "competitive intelligence", or any request to understand how the company stacks up against competitors on an ongoing basis.
---

# Competitive Intelligence Workshop

> **Before You Start**: We recommend completing this competitive intelligence workshop before you do your positioning work. If you've already crafted a positioning statement, you can revisit it after your competitive intel is complete.

A guided workshop that produces five outputs, always delivered as a combined PDF plus in-chat formats:
1. **Competitive Landscape Overview** — education-ready summary of the market, with threat tiers
2. **Comparison Chart** — your company vs. top competitors across key dimensions
2a. **Feature & Capability Matrix** — specific features/capabilities vs. competitors, marked ✓ ◐ ✕
2b. **De-Positioning Guide** — turns each competitor's claimed strength into a liability (Todd Irwin framework)
3. **Kill Sheets** — per-competitor, sales-ready one-pagers (user selects which to produce)

---

## Workshop Flow

Work through these phases in order. Ask one question at a time. Do not front-load the user with a list of questions.

---

### Phase 1: Company Context

Start here:

> "Let's build your competitive intelligence overview. To make sure I'm working from accurate, up-to-date information about your company, can you share any of the following?
> - **Documents**: sales decks, pitch decks, one-pagers, product briefs, or internal positioning docs (upload directly)
> - **Your website URL** — only if it's current and reflects how you actually position today
>
> If your website is out of date, skip it and rely on uploaded documents instead. The more accurate the source, the better the outputs."

**If documents are uploaded**: Read and extract positioning, ICP, differentiators, value props, and product framing. Use these as the primary source of truth throughout the workshop. Do not override document content with website content.

**If a website URL is provided**: Fetch it, but flag to the user if the messaging seems generic, inconsistent, or dated — and ask them to confirm it reflects current positioning before relying on it.

**If neither is provided**: Proceed conversationally. Ask:

> "No problem — tell me about your company: what you sell, who you sell to, and how you typically describe what makes you different."

After gathering company context (via docs, site, or conversation), ask:

> "What are the top 2–3 outcomes your customers say they get from your product?"

---

### Phase 2: Competitor Scoping

Ask:

> "Which competitors are you already tracking? List as many as you'd like — established players, up-and-comers, whatever's on your radar."

After they respond, ask:

> "Which of these come up most often during sales calls or in deals?"

Then ask:

> "Is there a 'status quo' competitor — meaning, the thing prospects are doing instead of buying your product? (Could be a spreadsheet, an internal process, a legacy tool, or doing nothing.)"

---

### Phase 3: Web Research + Competitor Suggestions

Now run web research in parallel:

1. **Research each named competitor** — homepage positioning, product messaging, pricing signals, recent news, G2/review themes, job postings for strategic signals
2. **Search for additional competitors** the user may have missed — up-and-coming players in the space, VC-backed entrants, adjacent category players moving in

After research, present:

> "Based on your list and my research, here are the competitors I suggest including — along with a few you may not have mentioned:"

Present a table like:

| Competitor | Why Include | Suggested Threat Tier |
|------------|-------------|----------------------|
| [Named by user] | Mentioned in sales calls | 🔴 High |
| [Named by user] | Established player | 🔴 High |
| [Found via research] | VC-backed, growing fast | 🟡 Moderate |
| [Found via research] | Niche overlap, early | 🟢 Low / Watch |
| Status quo (e.g., spreadsheets) | Default alternative | 🟡 Moderate |

**Threat Tier Criteria:**
- 🔴 **High** — appears frequently in deals, directly competitive, well-resourced
- 🟡 **Moderate** — partial overlap, growing, or indirect but notable
- 🟢 **Low / Watch** — early stage, niche, or not yet a direct threat but worth monitoring

Ask:
> "Does this list look right? Want to add, remove, or re-tier anyone before I build the full analysis?"

---

### Phase 4: Dimension Selection

Ask:

> "What dimensions matter most when your buyers are evaluating options? I'll suggest some defaults, but add anything specific to your market:"

Suggest:
- Primary use cases
- Key outcomes / results claimed
- Core capabilities
- Standout features
- Pricing model
- Deployment / implementation model (e.g. self-serve vs. sales-led, cloud vs. on-prem)
- Customer segment served (SMB / mid-market / enterprise)
- Integrations / ecosystem
- Support & services model
- Recent momentum (funding, launches, hires)

> "Which of these should I include in the comparison chart? Or just confirm and I'll use all of them."

---

### Phase 5: Chart Format Preference

Ask:

> "How would you like the comparison chart delivered?"
> - **Rendered visual** — an interactive HTML table in this chat
> - **Markdown table** — easy to copy into a doc or slide
> - **Both**

Note: Regardless of this choice, all outputs will also be compiled into a single downloadable PDF at the end.

---

### Phase 6: Build the Outputs

#### Output 1: Competitive Landscape Overview

Write a 400–600 word narrative overview covering:

- **The Market** — what category this is, how buyers think about it, what problem they're solving
- **The Competitive Set** — who the major players are, how they're grouped, what each stands for
- **Threat Map** — a summary of the threat tier breakdown with brief rationale for each tier
- **Status Quo** — what inaction or the default alternative looks like, and why it matters
- **Key Trends** — 2–3 market-level shifts affecting the competitive dynamics
- **So What** — a brief PMM synthesis: what this means for positioning and sales conversations

Label this clearly: *"Competitive Landscape Overview — [Date]"*

Format note: This should be readable by a new employee on day one or usable as the intro section of a battlecard deck.

---

#### Output 2: Comparison Chart

Build the chart using the dimensions confirmed in Phase 4.

Format per user preference (Phase 5):
- **Rendered visual**: Use an HTML artifact with clean table styling. Include threat tier badge (🔴🟡🟢) next to each competitor name. Highlight your company's column.
- **Markdown table**: Clean, copy-ready format. Add a row for threat tier at the top.
- **Both**: Render HTML first, then provide the markdown below.

---

#### Output 2a: Feature & Capability Matrix

Immediately after the Comparison Chart, produce a Feature & Capability Matrix as a separate table.

**Structure:**
- Features/capabilities listed down the left column
- Your company + each competitor across the top (highlight your company's column)
- Each cell marked with:
  - ✓ — full support
  - ◐ — partial support or manual workaround required
  - ✕ — not supported

**Group features into logical sections**, for example:
- Core Capability (primary job-to-be-done features)
- Data & Quality
- Reporting & Analytics
- Adoption & Fit (onboarding, ease of use signals, support)
- Adjacent Capabilities (integrations, API, extensibility)

Adapt section names to fit the actual product category. Use research and uploaded docs to populate accurately. Use "?" where data is genuinely unavailable rather than guessing.

**Include features the company does NOT have but competitors do.** The matrix should be a complete picture of the competitive feature landscape — not just where the company wins. Rows where competitors have ✓ and the company has ✕ are as important as the reverse. Do not omit capabilities just because they reflect a gap.

Render the matrix as a styled HTML table in chat, and include it in the final PDF.

---

#### Output 2b: De-Positioning Guide

Based on Todd Irwin's De-Positioning framework: don't just differentiate — take each competitor's own claimed strength and show how it fails to solve the customer's real pain, turning that strength into a liability.

**Step 1: Identify Hero Pain Points**
Before writing competitor entries, identify 2–3 "Hero Pain Points" — the most critical problems the ICP needs solved, drawn from company docs, customer outcomes shared in Phase 1, and research. State these clearly at the top of the guide.

**Step 2: For each competitor, produce:**

---

**[Competitor Name]** | Threat Tier: 🔴/🟡🟢

**How They Position Themselves**
Their own claimed strength, in their words (near-verbatim from their site or materials).

**De-Positioning Angle**
How that exact strength creates or hides a gap tied to one of the Hero Pain Points. This is not a generic weakness — the strength itself is the liability. Be specific and grounded in evidence.

---

Tone: Sharp but credible. This guide is for internal PMM and sales use — it should feel like a strategic insight, not a smear campaign.

---

#### Output 3: Kill Sheet Selection

After delivering Outputs 1, 2, 2a, and 2b, ask:

> "Kill sheets are one-pagers your sales team can use when going head-to-head with a specific competitor. Which competitors would you like kill sheets for?"

List all competitors from the analysis with checkboxes implied. User can say "all of them", name specific ones, or "none — I'm good for now."

If they select none, skip to the PDF compilation step.

For each selected competitor, produce a kill sheet using this structure:

---

**KILL SHEET: [Competitor Name]** | Threat Tier: 🔴/🟡🟢 | Updated: [Date]

**What They Do**
One sentence on their product and positioning.

**Who They Target**
ICP / buyer profile.

**Their Pitch**
Their headline claim and top 3 differentiators (verbatim or near-verbatim from their site).

**Where They're Strong** *(be honest)*
2–3 genuine strengths — features, brand, reviews, pricing.

**Where They're Weak**
2–3 consistent gaps — from reviews, customer feedback, positioning holes.

**How We Win**
3–5 differentiators that matter when going head-to-head. For each:
- The differentiator
- Why it matters to the buyer
- Proof point or supporting evidence

**Objection Handling**
| If they say... | We say... |
|----------------|-----------|
| "[Competitor] does this too" | ... |
| "[Competitor] is cheaper" | ... |
| "I've heard good things about them" | ... |

**Landmines to Set**
Questions to ask early in the sales conversation that surface competitor weaknesses naturally:
- "How important is [X] to you?" *(where X is a capability the competitor lacks)*
- "Have you thought about [risk] that comes with [their approach]?"
- "What happens to your workflow when [known limitation of competitor]?"
- "How are you currently handling [gap the competitor doesn't address]?"

**Landmines to Defuse**
Questions they might coach prospects to ask us, with prepared responses.

**Win/Loss Patterns**
- We tend to win when: ...
- We tend to lose when: ...
- Prospect profile that favors us vs. them: ...

---

#### Final Delivery: Combined PDF

After all outputs are complete, compile everything into a single downloadable PDF in this order:
1. Competitive Comparison Chart
2. Feature & Capability Matrix
3. De-Positioning Guide
4. Kill Sheets (for whichever competitors were selected)

**How to build it:**
- Build each section as styled HTML (clean, professional, print-ready)
- Convert each HTML section to PDF using `wkhtmltopdf`
- Merge all section PDFs into one file using `pypdf`
- Save the final PDF to `/mnt/user-data/outputs/competitive-intelligence-[date].pdf`
- Present the file for download using `present_files`

**HTML styling guidance:**
- White background, black body text
- Company column highlighted with a light brand-neutral color (e.g. light blue `#EBF4FF`)
- Section headers bold and clearly separated
- ✓ in green, ◐ in amber, ✕ in red for the Feature Matrix
- Threat tier badges: 🔴 High / 🟡 Moderate / 🟢 Low rendered as colored inline badges
- Font: system-safe (Arial or Helvetica)
- Page breaks between major sections

---

### Phase 7: Wrap-Up

After the PDF is delivered, offer:

> "Here's what you now have:
> - ✅ Competitive landscape overview
> - ✅ Comparison chart ([format])
> - ✅ Feature & Capability Matrix
> - ✅ De-Positioning Guide
> - ✅ Kill sheets for: [list or 'none selected']
> - ✅ Combined PDF download
>
> Want me to:
> - Dig deeper on any specific competitor?
> - Draft positioning or messaging that exploits the gaps we found?
> - Re-run this workshop in 90 days to refresh the intel?"

---

## Research Guidelines

### What to Research Per Competitor
- Homepage: headline, subhead, hero message, CTA
- Product pages: feature framing, use case emphasis
- Pricing page (if public): model, tiers, signals
- About/Story page: founding narrative, mission
- Blog/resources: content themes, publishing cadence
- G2 / Capterra / TrustRadius: top praise and complaint themes
- LinkedIn: employee count, recent hires, job postings
- News: last 6 months — funding, launches, partnerships, leadership changes
- Social: Twitter/LinkedIn tone and topics

### Threat Tier Assignment Logic
- 🔴 High: Direct ICP overlap + comes up in sales + well-resourced
- 🟡 Moderate: Partial overlap OR growing fast OR strong in adjacent segment
- 🟢 Low/Watch: Early, niche, or indirect — flag for monitoring, not urgent action

### Status Quo Research
Search for: "[category] alternatives", "[problem] without software", "how companies handle [problem] manually". This reveals what the no-decision path looks like.

---

## Output Quality Standards

- **Landscape overview**: Narrative, not bullets. Designed to be shared with non-PMMs.
- **Comparison chart**: Accurate to research. Use "N/A" or "Not public" rather than guessing.
- **Feature matrix**: Use "?" where data is genuinely unavailable. Never fabricate support levels.
- **De-positioning guide**: Grounded in the competitor's actual claims. Sharp but credible — for internal use.
- **Kill sheets**: Balanced and honest. Salespeople won't trust a kill sheet that makes competitors look like clowns. Acknowledge genuine strengths.
- **Dates matter**: Always stamp outputs with the research date. Competitive intel goes stale fast.
