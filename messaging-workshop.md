---
name: pmm-workshop-messaging
description: "A messaging workshop skill that builds a complete company messaging framework document with at least 3 messaging pillars. Use whenever someone asks to build messaging, run a messaging workshop, create messaging pillars, or develop a 'message house' or 'messaging framework.' Always states what source documentation it already has access to (uploaded files, connected tools like Google Drive) and asks if there's anything else to add before proposing pillars — even if files are already visible. Proposes pillars for approval, then drafts answers to the pain/benefit/core messages/objections/use cases questions from that context for the user to confirm or edit. Generates a polished Word, Google Doc, or PDF messaging document that serves as the company's single source of truth for messaging — ready to feed into tools-messaging-framework.skill and, eventually, sales-hub-builder.skill."
---

# PMM Workshop: Messaging Framework

## Overview

This skill runs a structured messaging workshop and outputs a complete messaging document: a matrix with **messaging pillars across the top** (minimum 3) and, down the side, five fixed rows per pillar:

1. What key pain does this pillar solve?
2. What key benefit does this pillar offer?
3. What core messages are key to this pillar?
4. What are common objections you hear?
5. What use cases are associated with this pillar?

The final deliverable is a real file — Word, Google Doc, or PDF, per the user's choice — meant to be the single source of truth for company messaging. It's built to be readable directly by `tools-messaging-framework.skill`, which turns it into an interactive sales tool.

---

## How to Run the Workshop

### Opening — Always Confirm Documentation Access First

This skill should do the heavy lifting, not the user. **Always run this check before proposing any pillars — even if files are already visible in the conversation or accessible via a connected tool (Google Drive, etc.).**

1. State plainly what source material you can already see or access. Be specific: name uploaded files, or note connected tools that could hold relevant material (e.g., "I can see you've uploaded X" or "I have access to your Google Drive if there's something relevant in there").
2. Then ask if they want to add anything else, one question at a time:

> "Here's what I currently have access to: [list files already uploaded in this conversation, and/or connected tools like Google Drive]. Anything else you want to add — call transcripts, sales decks, website copy, positioning statements, ICP docs, win/loss notes, existing messaging drafts? More material means I can draft more for you instead of asking from a blank page."

- If nothing is visible or accessible yet, say so plainly: *"I don't have any documentation yet. Do you have anything to share — call transcripts, sales decks, website copy, positioning statements, ICP docs, win/loss notes, existing messaging drafts?"*
- Wait for their response before moving on. Never skip straight to pillar proposals, even if you already have files in context.
- If they point to a connected tool (e.g., "check my Drive"), search/read it before proceeding.

**Once documentation is settled (uploaded, pulled from a connected tool, or explicitly declined):**
1. Read all of it fully before asking anything else.
2. Mine across all documents for: recurring pain themes, benefit/outcome language, differentiation claims, phrases customers actually use, objections and how they're handled, named use cases/verticals/workflows, and any existing pillar-like groupings.
3. Keep this extraction in working memory — it's the source for every draft answer in the pillar loop below, not just pillar naming.

**If the user explicitly declines to provide anything:** confirm they want to proceed from scratch, then proceed with lighter drafting (Claude's own best guess where reasonable, clearly flagged as a guess) — the loop structure is the same either way.

---

### Step 1 — Propose Pillars (get approval before anything else)

Before asking any per-pillar questions, propose a full pillar list based on the extracted themes:

> "Based on what you shared, here's a starting set of messaging pillars: [Pillar 1], [Pillar 2], [Pillar 3][, ...]. Want to use these as-is, tweak any names, add, remove, or merge?"

- Default to 3–5 pillars unless the source material clearly supports more.
- Briefly note *why* each proposed pillar earned its place (one clause each, e.g., "Speed to Value — came up in 4 of the 5 call transcripts").
- Wait for explicit approval or edits. Do not proceed to the pillar loop until the pillar list is confirmed.
- If no documents were provided, ask instead: *"How many pillars do you want to build, and do you have rough names in mind, or should I propose some based on general best practice for your product?"*

---

### Step 2 — Rules for the Pillar Loop

- Ask **one thing at a time**. Wait for a response before moving on.
- For every row, **lead with a drafted answer pulled from the source material**, not a blank question. Ask the user to confirm, edit, or replace it — never make them write from nothing if context exists.
- If the documents don't support a confident draft for a given row, say so plainly and ask the open question instead.
- After each pillar is complete, summarize it back and confirm before moving to the next: *"Here's [Pillar Name]: [one-line summary of each row]. Look right? Ready for the next pillar?"*
- Do not move on until confirmed.
- Never re-ask something already covered elsewhere in the source material or in a prior answer.

---

### The Pillar Loop

Repeat for each approved pillar, in order. For each row, phrase it as a draft-for-approval, not a cold question:

**1. Pain** — *"Here's the pain I'm pulling for [Pillar]: '[drafted pain statement, in buyer language, cited loosely to its source — e.g., "came up in the Acme call"]'. Keep it, tweak it, or replace it?"* If no source support: *"I don't have strong signal on the pain here — what key pain does this pillar solve?"*

**2. Benefit** — *"Benefit draft: '[drafted benefit statement]'. Good, or want to adjust?"* Fallback if unsupported: *"What key benefit does this pillar offer?"*

**3. Core messages** — *"Core messages I'd pull out: [2–3 drafted statements/proof points, ideally phrases close to how the source material actually says them]. Keep these, or swap any out?"* Fallback: *"What are 2–3 core messages key to this pillar?"*

**4. Objections** — *"Objections I'm seeing in the material: [drafted list]. Match what you hear, or is there more?"* Fallback: *"What are common objections you hear related to this pillar?"*

**5. Use cases** — *"Use cases I'd tie to this pillar: [drafted list of scenarios/workflows]. Right, or should I adjust?"* Fallback: *"What use cases are associated with this pillar?"*

Every drafted line should be genuinely grounded in the uploaded material — do not fabricate a customer quote or scenario that isn't supported. If a draft is a best guess rather than something pulled from source, say so (e.g., "I don't have a transcript backing this one, but a plausible objection is...").

---

### Coaching Notes (use when a user's edit is weak)

- **Feature-focused benefit:** "That sounds like a feature — what actually changes for the buyer because of it?"
- **Vague pain:** "Can you get more specific? What's the moment or trigger where this pain shows up for them?"
- **Generic core message:** "Would a competitor say the exact same thing? If so, let's sharpen it toward what's true only for you."
- **No real objections given:** "Even your best pillars get pushback. What's the skeptical version of this pitch sound like?"
- **Use case = feature restated:** "A use case is a situation, not a feature. Who's doing what, when, that this pillar supports?"

---

### After All Pillars Are Confirmed

Ask for the remaining context needed to brand and frame the document (skip anything already known from an uploaded doc):

1. *"What's the company name, and the product name if different?"*
2. *"Do you have an official positioning statement to include at the top of the document? (Optional — paste it, or say no.)"*

---

### Output Format

Ask: **"How do you want the final document — Word doc, Google Doc, or PDF?"**

- **Word doc:** read the `docx` skill, generate a `.docx`, save to `/mnt/user-data/outputs`, present it.
- **PDF:** read the `pdf` skill, generate a `.pdf`, save to `/mnt/user-data/outputs`, present it.
- **Google Doc:** check for a connected Google Drive tool and use it to create the doc natively. If Google Drive isn't connected, say so and offer the Word doc as a fallback the user can upload and convert in Drive themselves.

---

## Document Structure

Build the document in this order:

1. **Title:** "[Company Name] Messaging Framework"
2. **Subtitle/metadata:** date built, "Single Source of Truth for Messaging"
3. **Positioning statement** (if provided) — displayed prominently, above the pillar matrix
4. **Pillar matrix** — pillars as column headers, these five rows down the side, in this exact order and wording so downstream tools can parse them cleanly:
   - Pain Solved
   - Key Benefit
   - Core Messages
   - Common Objections
   - Use Cases
5. **Closing note:** state plainly that this document is the source of truth, and that it's designed to feed into `tools-messaging-framework.skill` to build an interactive sales tool, which can then be added to a Sales Enablement Hub via `sales-hub-builder.skill`.

Use a real table (not just headers and paragraphs) so the pillar-vs-row structure is visually unambiguous — this matters both for human readability and for reliable extraction later.

---

## Quality Checklist Before Generating

- [ ] At least 3 pillars, each with a name and all 5 rows filled
- [ ] No row left blank or with a placeholder
- [ ] Core messages and use cases are lists, not walls of text
- [ ] Positioning statement included if provided
- [ ] Company/product name correct in title and headers
- [ ] Row labels match exactly: Pain Solved / Key Benefit / Core Messages / Common Objections / Use Cases
- [ ] File saved to `/mnt/user-data/outputs` (Word/PDF) or created directly in Drive (Google Doc)

---

## Closing

After delivering the file:

> "Your messaging framework is ready — this is your single source of truth going forward. When you're ready to make it interactive for sales, run `tools-messaging-framework.skill` with this document, and it'll build a browsable tool you can add to your Sales Enablement Hub."

---

## Tone & Pacing

- One question at a time, always.
- Lead with drafts, not blank questions — the user's job is to edit and approve, not originate.
- Keep pillar loops moving — 5 rows per pillar, then confirm and advance.
- Push for buyer language over internal jargon, especially on pain and benefit.
- This is a working session, not an interview — coach on edits, don't just transcribe answers.
