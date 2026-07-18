---
name: pmm-workshop-ideal-customer-profile
description: "An ICP (Ideal Customer Profile) workshop skill for product marketers — based on Gartner's framework. Use whenever someone asks to build an ICP, define an ideal customer, or run an ICP workshop. Guides the user through all 6 Gartner ICP attribute blocks one question at a time — capturing ideal, acceptable, and unacceptable personas — then synthesizes a complete ICP with a structured profile and narrative summary. Always trigger this skill when the user mentions ICP or ideal customer profile."
---

# ICP Workshop — Gartner Framework (for Tech CEOs)

## Overview

This skill runs a structured ICP workshop based on the Gartner ICP framework. It guides the user through 6 attribute blocks, one question at a time, capturing the **Ideal**, **Acceptable**, and **Unacceptable** persona dimensions within each block. At the end, it synthesizes a complete ICP with both a structured profile (table format) and a narrative summary.

**The 6 Gartner ICP Attribute Blocks:**
1. Firmographics
2. Technographics
3. Psychographics
4. Business Situation
5. Business & Operating Model
6. Resources

---

## How to Run the Workshop

### Opening

When the workshop is triggered, open with this framing:

> "Let's build your Ideal Customer Profile using the Gartner ICP framework. We'll go through 6 attribute blocks — I'll ask focused questions for each one, then pull everything together into a complete ICP with a structured profile and a narrative summary.
>
> For each block, we'll define your ideal customer, then end with a quick disqualifier check to identify who's a poor fit. The middle ground — accounts that are acceptable but not ideal — will emerge naturally from that contrast.
>
> Let's start with Block 1: Firmographics."

---

### Rules for All Blocks

- Ask **one question at a time**. Wait for an answer before asking the next.
- Ask **no more than 5 questions per block** (including the disqualifier question). Fewer is better.
- The **disqualifier question is always the last question in every block**. Generate it dynamically based on what the user has shared in that block. See disqualifier guidance below.
- After the last question in each block, briefly summarize what you've captured and confirm before moving on: *"Here's what I've captured for [Block Name]: [summary]. Ready to move to Block [N+1]?"*
- Do not move to the next block until confirmed.
- Keep questions sharp and coaching-oriented — push for specificity, not generalities.
- If an answer is vague, probe once before moving on.
- **Never re-ask something the user has already answered.** If a response covers the ground of a later question, skip it.

---

### Disqualifier Question — Dynamic Generation

The disqualifier is the final question in every block. It must be generated dynamically based on what the user has shared in that block — not a generic template.

**Format:**
> "Are there any [block name] characteristics that would make a prospect a poor fit? For example, [generate a specific, contextually relevant example based on what you've learned about their product, market, and customer in this conversation]."

**Guidance for generating the example:**
- Pull from signals in the conversation: the product they've described, the industry, the customer type, the technologies mentioned.
- Make the example feel like it could be real for their business — not generic.
- The example should name a specific scenario, technology, company characteristic, or behavior that would be disqualifying.

**Example disqualifier questions by block (illustrative — always adapt to the actual conversation):**

- *Firmographics:* "Are there any firmographic characteristics that would make a prospect a poor fit? For example, if you sell to mid-market and above, would a company with fewer than 200 employees be a deal-breaker — or just a stretch?"
- *Technographics:* "Are there any technographic characteristics that would make a prospect a poor fit? For example, if your product integrates deeply with Salesforce, would a prospect running a fully custom CRM be a red flag?"
- *Psychographics:* "Are there any psychographic characteristics that would make a prospect a poor fit? For example, if your product requires significant change management, would a risk-averse 'if it ain't broke' organization be a poor match?"
- *Business Situation:* "Are there any business situation characteristics that would make a prospect a poor fit? For example, if your product is built for companies in growth mode, would a company in cost-cutting or contraction be worth pursuing?"
- *Business & Operating Model:* "Are there any operating model characteristics that would make a prospect a poor fit? For example, if your product requires cross-functional data sharing, would a company with heavily siloed departments struggle to get value?"
- *Resources:* "Are there any resource characteristics that would make a prospect a poor fit? For example, if implementation requires a dedicated internal project lead, would a company with a fully outsourced IT function be too risky?"

---

## Block 1: Firmographics

**Goal:** Define the organizational characteristics of the ideal customer — size, industry, location, and structure.

**Block Summary (share with user before asking questions):**
> "Firmographics are the foundational 'who' of your ICP — the hard, observable facts about a company. Think of it as the criteria you'd use to filter a list of companies: what industry they're in, how big they are, where they operate, and how they're structured. Getting this right means your teams can quickly identify whether a company is worth pursuing before a single conversation."

**What to capture:**
- Industry or vertical
- Company size (employees, revenue, or both)
- Geography
- Company type or structure (public/private, startup/enterprise, standalone/subsidiary)
- Disqualifiers

**Questions (ask one at a time, in order — stop early if answers cover later questions):**

1. *"What industry or vertical does your ideal customer operate in? If you serve multiple industries, which one produces your best customers?"*

2. *"How big is the ideal company — in terms of employees, annual revenue, or both? Is there a sweet spot where you win most often?"*

3. *"Does geography matter? Are there specific regions, countries, or markets where you see the strongest fit — or that you intentionally avoid?"*

4. *"Is there anything about company type or structure that matters — for example, public vs. private, standalone vs. subsidiary, or startup vs. established enterprise?"*

5. *(Disqualifier — generate dynamically based on what's been shared)*

---

## Block 2: Technographics

**Goal:** Define the technology environment the ideal customer operates in — what they use, what they need, and what's incompatible.

**Block Summary (share with user before asking questions):**
> "Technographics tell us what the customer's technology environment looks like — the systems they run, how mature they are with technology, and what needs to be in place for your product to actually work. This block often surfaces deal-breakers early: if your product requires Salesforce and they're on a custom CRM, that's critical to know before investing time in a deal."

**What to capture:**
- Key systems or platforms the customer uses (ERP, CRM, data infrastructure, etc.)
- Technology maturity or sophistication
- Integration requirements or dependencies
- Disqualifiers

**Questions (ask one at a time, in order):**

1. *"What does the technology environment of your ideal customer look like? Are there specific systems, platforms, or tools they're typically running — like a particular ERP, CRM, or cloud infrastructure?"*

2. *"How technically sophisticated is your ideal customer? Are they early adopters, mainstream buyers, or more conservative with new technology?"*

3. *"Does your product require integration with or dependency on a specific technology? If so, what does the customer need to have in place for your product to deliver full value?"*

4. *(Disqualifier — generate dynamically based on what's been shared)*

---

## Block 3: Psychographics

**Goal:** Define how the ideal customer thinks about technology, change, and vendor relationships — their mindset and decision-making culture.

**Block Summary (share with user before asking questions):**
> "Psychographics go beyond what a company looks like on paper — they describe how the organization thinks and behaves. Two companies can be identical firmographically but have completely different buying cultures. This block helps your teams identify whether a prospect has the mindset to actually adopt and champion your product, or whether they'll stall, second-guess, and churn."

**What to capture:**
- Technology adoption posture (innovator, early majority, laggard)
- Attitude toward change and risk
- How they view vendor relationships (partner vs. vendor)
- Strategic vs. tactical orientation
- Disqualifiers

**Questions (ask one at a time, in order):**

1. *"How does your ideal customer think about technology — is it a strategic driver of their business, or more of a cost to be managed? Are they trying to lead with tech or keep up with it?"*

2. *"How do they approach change? Do they move fast and experiment, or do they prefer to observe, validate, and follow proven paths?"*

3. *"How do they think about vendor relationships — are they looking for a long-term strategic partner, or do they prefer transactional, low-touch procurement?"*

4. *(Disqualifier — generate dynamically based on what's been shared)*

---

## Block 4: Business Situation

**Goal:** Define the business circumstances, events, or conditions that make a prospect ready and motivated to buy.

**Block Summary (share with user before asking questions):**
> "Business Situation is about timing and context — what has to be true in a company's world for them to feel the urgency to buy. The best ICPs don't just describe who to target; they describe *when* to target them. This block helps your teams recognize the moments that make a prospect ready, and equally important, the situations that mean the timing is just wrong."

**What to capture:**
- Growth stage or company trajectory
- Trigger events (regulatory change, M&A, leadership change, competitive pressure)
- The specific pain or problem that creates urgency
- Industry-specific conditions that drive buying behavior
- Disqualifiers

**Questions (ask one at a time, in order):**

1. *"What has to be happening inside a company for them to feel urgency to buy your product? Is it a specific growth stage, a strategic initiative, a pain they've hit a breaking point with — what's the 'something just changed' moment?"*

2. *"Are there specific trigger events that tend to put you on a prospect's radar? Think about your best customers — what was happening in their business in the 3–6 months before they bought? Things like a new executive hire, a merger, a compliance deadline, a failed implementation?"*

3. *"What's the core problem your ideal customer is trying to solve — and how long have they typically been sitting with that problem before they come to you? Are they in acute pain or more proactively planning?"*

4. *"Is there a 'not yet' scenario — a business situation where the timing is clearly wrong, even if the company looks like a perfect fit on paper?"*

5. *(Disqualifier — generate dynamically based on what's been shared)*

---

## Block 5: Business & Operating Model

**Goal:** Define how the ideal customer's business actually runs — the operational structure and model that determines whether your product fits.

**Block Summary (share with user before asking questions):**
> "The Business & Operating Model block is about the mechanics of how a company runs — how they make money, how work flows through the organization, and how decisions get made. Two companies in the same industry at the same size can operate very differently, and those differences determine whether your product is a natural fit or a constant friction point. This block helps identify the operational DNA of your best customers."

**What to capture:**
- How the business generates revenue (transaction model, subscription, project-based, etc.)
- Key operational characteristics (distributed vs. centralized, high-volume vs. complex, etc.)
- Decision-making structure (centralized vs. decentralized, who has authority)
- Ecosystem dependencies (partners, channels, suppliers)
- Disqualifiers

**Questions (ask one at a time, in order):**

1. *"How does your ideal customer generate revenue — and how does that shape their day-to-day operations? For example, are they high-volume and transactional, project-based and bespoke, or subscription-driven with recurring delivery cycles?"*

2. *"How is the organization structured operationally — is decision-making centralized with strong leadership, or distributed across business units and regions? And how does that affect how your product gets bought and rolled out?"*

3. *"Where does your product sit in their operational workflow — is it a core system of record, a layer on top of existing systems, or a point solution for a specific team? What does the 'before and after' look like in their day?"*

4. *"Do they operate within a broader ecosystem — partners, suppliers, channel resellers, or a marketplace — that your product needs to connect with or support?"*

5. *(Disqualifier — generate dynamically based on what's been shared)*

---

## Block 6: Resources

**Goal:** Define the internal resource profile of the ideal customer — what they have available to implement, adopt, and sustain your product.

**Block Summary (share with user before asking questions):**
> "Resources is the often-overlooked block that separates companies that can succeed with your product from those that will struggle regardless of fit. It's not just about budget — it's about people, bandwidth, and organizational capacity. A company might love your product and have the budget, but if they don't have the internal resources to implement and sustain it, they'll churn. This block helps define the minimum viable customer from an operational standpoint."

**What to capture:**
- Internal IT capability and availability
- Budget ownership and procurement structure
- Implementation capacity (dedicated team vs. lean/no IT)
- Disqualifiers

**Questions (ask one at a time, in order):**

1. *"What does the internal IT or technical capability of your ideal customer look like? Do they have a dedicated team that can implement and manage your product, or are they more lean?"*

2. *"Who owns the budget for your product — is it IT, a business unit, or the C-suite? And how do they typically buy — direct, through a channel, or via a procurement process?"*

3. *"How much implementation lift does your product require from the customer's side? What does the ideal customer need to have in place — people, time, and internal ownership — for a successful deployment?"*

4. *(Disqualifier — generate dynamically based on what's been shared)*

---

## Synthesis: Complete ICP Output

After all 6 blocks are confirmed, ask the user how they'd like the output delivered before generating anything:

> "We've covered all 6 blocks — great work. Before I pull everything together into your complete ICP, how would you like it delivered?
> - **Word document** — a formatted .docx you can edit and share
> - **Google Doc** — delivered as a formatted document in Google Drive
> - **PDF** — a clean, ready-to-share PDF
>
> Just let me know and I'll generate accordingly."

Wait for the user's selection, then generate the ICP in the chosen format. If they choose Word or PDF, use the appropriate skill (docx or pdf). If they choose Google Doc, use the Google Drive MCP to create and deliver it. For all formats, the content structure remains the same — three parts as defined below.

---

### Part 1: Structured ICP Profile

Present a clean table with all three persona tiers across all 6 blocks:

| Attribute | Ideal Persona | Acceptable Persona | Unacceptable Persona |
|---|---|---|---|
| **Firmographics** | [from Block 1] | [inferred middle ground] | [disqualifiers from Block 1] |
| **Technographics** | [from Block 2] | [inferred middle ground] | [disqualifiers from Block 2] |
| **Psychographics** | [from Block 3] | [inferred middle ground] | [disqualifiers from Block 3] |
| **Business Situation** | [from Block 4] | [inferred middle ground] | [disqualifiers from Block 4] |
| **Business & Operating Model** | [from Block 5] | [inferred middle ground] | [disqualifiers from Block 5] |
| **Resources** | [from Block 6] | [inferred middle ground] | [disqualifiers from Block 6] |

**Guidance for the Acceptable Persona column:**
- This is the inferred middle ground between Ideal and Unacceptable.
- It represents accounts worth pursuing that fall short of ideal — they may require more effort, longer cycles, or lower ACV, but aren't disqualified.
- Derive it from the contrast between what the user described as ideal and what they named as disqualifying. Don't ask the user for this — synthesize it yourself.

---

### Part 2: ICP Narrative Summary

Write a concise narrative (4–6 paragraphs) that brings the ICP to life. This is not a repeat of the table — it's a story of the ideal customer that a sales rep, marketer, or CEO could read and immediately visualize.

Structure the narrative as follows:

**Paragraph 1 — Who they are:** Describe the ideal company in plain language — industry, size, geography, structure.

**Paragraph 2 — How they operate:** Describe their technology environment, operating model, and how they run their business day-to-day.

**Paragraph 3 — How they think:** Describe their psychographic profile — their mindset around technology, change, and vendor relationships.

**Paragraph 4 — What's driving them:** Describe the business situation and trigger events that make them ready to buy.

**Paragraph 5 — What they bring to the table:** Describe the internal resources, budget ownership, and implementation capacity that makes them a successful customer.

**Paragraph 6 — Who to avoid:** Briefly describe the unacceptable persona — the characteristics that signal a prospect is unlikely to succeed with your product, and why.

---

### Part 3: How to Use Your ICP

After the narrative, include a brief section on how each key team should put the ICP to work. Keep each entry to 2–4 bullet points — practical and specific, not generic advice.

Generate this section dynamically based on what you've learned about the user's business, product, and market throughout the workshop. The tips should feel tailored, not boilerplate.

Use this structure:

---

**How to Use Your ICP**

**Marketing**
- How to use the ICP for audience targeting, channel selection, and campaign messaging
- How firmographics and technographics should inform list building and ABM strategy
- How psychographics should shape content tone, themes, and thought leadership angles

**Sales**
- How to use the ICP for prospect qualification and pipeline prioritization
- How the Acceptable and Unacceptable personas help reps decide where to invest time
- How trigger events from the Business Situation block should inform outreach timing

**Product**
- How to use the ICP to validate roadmap priorities and feature bets
- How the Resources and Operating Model blocks reveal integration needs and onboarding considerations
- How the Unacceptable persona can help define what the product should *not* be built to accommodate

**Customer Success**
- How to use the ICP to identify at-risk accounts (those that drifted from the ideal profile)
- How onboarding and adoption milestones should be calibrated to the Resources block
- How the ICP helps CS proactively identify expansion opportunities within the right account types

**Leadership / GTM Strategy**
- How to use the ICP to align Sales, Marketing, and Product around a shared target
- How to revisit and refresh the ICP as the market evolves (recommended: every 6–12 months or after a major product or market shift)
- How the ICP informs market sizing, segment prioritization, and resource allocation decisions

---

**Guidance for dynamic generation:**
- If the user's product is highly technical, lean into technographic tips for Sales and Product.
- If they sell into a specific vertical, make the Marketing tips vertical-specific.
- If their Resources block revealed lean IT buyers, flag that for Customer Success and Product onboarding design.
- Keep each bullet punchy — one clear action or insight per line.

---

### Closing Prompt

After delivering the full ICP output, offer:

> "You now have your complete ICP — structured profile, narrative, and activation guidance. Would you like to stress-test any of this, adapt it for a specific market segment, or use it to kick off a positioning workshop?"

---

## Coaching Notes

Use these when answers are vague — probe once, then move on:

- **Vague industry:** "Can you be more specific? 'B2B companies' isn't precise enough — which sector, vertical, or function?"
- **Too broad on size:** "Is there a sweet spot — a size where you win most often and see the strongest retention? That's the size to anchor to."
- **Generic psychographic:** "'Forward-thinking' is a claim every company makes about themselves. What behavior tells you they actually are — what do they *do* differently?"
- **Unclear trigger:** "Is this a trigger you see repeatedly in your best accounts — or more of a one-off? Repeatable triggers are what make ICP operationalizable."
- **Weak disqualifier:** "Push a bit further — is there a prospect type you've learned the hard way not to pursue? That's often the sharpest disqualifier."
