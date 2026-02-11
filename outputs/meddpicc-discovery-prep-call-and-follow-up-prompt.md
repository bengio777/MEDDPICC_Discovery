# Baseline Workflow Prompt: MEDDPICC Discovery Prep, Call, and Follow-up

## Purpose

**Workflow:** MEDDPICC Discovery Prep, Call, and Follow-up
**Description:** End-to-end workflow for an enterprise Account Executive to research, prepare for, execute, and follow up on a discovery call with a senior stakeholder, using MEDDPICC to qualify the opportunity.
**Outcome:** A qualified (or disqualified) opportunity with MEDDPICC criteria assessed, next steps defined, and mutual commitments in place.
**When to use:** A discovery call has been scheduled with a Director of Security or above at a target account.

**Guiding Principle:** Be better prepared, ask better questions, follow up more quickly, and present a more polished and courteous interaction than the average sales rep — and more importantly, than the competitor's sales rep. The competitive edge is not the AI; it is the AE who shows up better prepared than anyone else in the deal.

---

## Instructions

Run these steps in order. Steps marked **(AI)** are executed by the model. Steps marked **(Human)** are executed by the AE — the model pauses and waits for the human to complete the step and provide any outputs back.

---

### Step 1: Draft Agenda and Confirmation Email (AI)

Using the meeting context provided in the inputs, draft a confirmation email to the prospect that:

1. Proposes a structured agenda for the discovery call. The agenda should demonstrate command of the process while explicitly inviting the prospect's collaboration. Use language like: "Here's what I'd like to cover — what would you add or adjust?"
2. Introduces any team members who will be joining from the AE's side (Sales Engineer, Director of Sales, or others as specified in the inputs).
3. Strikes a tone that is confident, courteous, and collaborative — not presumptuous or generic.
4. Keeps the email concise — no more than 150-200 words.

**Output:** A draft confirmation email ready for human review.

**Present the draft to the AE and pause.** The AE will review, adjust tone, add or remove team members, and send.

---

### Step 2: Stakeholder and Organization Research (AI)

Conduct deep research on the primary stakeholder, their team, their organization, and the broader market context. This is the highest-value automation step. Execute the following research threads:

#### 2a. Individual Stakeholder Research
- Find the stakeholder's LinkedIn profile. Capture: current role and tenure, career history (previous companies and roles), recent LinkedIn posts and activity, mutual connections with the AE or the AE's organization, education background (school, university).
- For each previous employer in the stakeholder's career history, determine: Is that company a current customer of our organization? Did the stakeholder work in a role where they would have used our product or a competitor's product?

#### 2b. Team Mapping
- Identify the stakeholder's direct reports, peers, and manager where possible.
- For each team member found, check: Have they previously worked at companies that are customers of our organization or customers of known competitors? Do their LinkedIn profiles indicate experience with our product category?
- Produce a stakeholder map showing the primary contact, their team members, and any product/competitor exposure flags.

#### 2c. Legislative and Regulatory Research
- Based on the prospect's industry vertical, identify current legislative or regulatory mandates that could drive urgency for the prospect to take action in our domain.
- Be specific — cite the regulation or mandate by name (e.g., "SEC cybersecurity disclosure rules effective December 2023," "NIS2 Directive," "DORA," "state-level privacy laws").
- Flag any pending or recently enacted legislation that creates a compliance deadline.

#### 2d. Financial Filing Analysis
- If the prospect's company is publicly traded, search their most recent 10-K, 8-K, 5-K, or investor statements for:
  - Any mention of our domain or the broader problem space as a strategic priority
  - The degree of specificity — did they name the problem generically or with detail that maps to our solution?
  - Risk factors disclosed that relate to our domain
  - Capital expenditure or budget signals related to our space
- If the company is private, search for press releases, funding announcements, or executive interviews that reveal strategic priorities.

#### 2e. Company and Industry Context
- Identify the prospect's industry vertical, primary competitors, and market position.
- Identify 2-3 companies in similar domains or verticals that could serve as third-party reference stories.
- Identify the organization's publicly stated guiding principles, values, or strategic directives and how they flow through to the stakeholder's business unit.

**Output:** A structured research package with five sections matching the threads above. Flag confidence levels on every finding:
- **Verified** — sourced and cited
- **Inferred** — reasonable conclusion from available data
- **Gap** — could not determine; needs to be uncovered on the call

**Present the research package to the AE and pause.** The AE will review for accuracy, flag what is strategically significant, and identify which findings change the call strategy.

---

### Step 3: Build the Call Briefing Doc (AI)

Using the reviewed and validated research from Step 2, synthesize a **Call Briefing Doc** formatted for glanceable reference during the live call.

#### Format Requirements
The briefing doc must be scannable at a glance. Each section has a **bold title** with **highlighted sub-bullets** beneath it. The AE should be able to look down mid-conversation and immediately find the right thread to pull.

#### Required Sections

**RAPPORT ANGLES**
- Personal connection points: hobbies, interests, mutual connections, shared background
- Recent LinkedIn activity worth referencing
- Any personal or professional overlap with the AE

**COMPANY & INDUSTRY**
- Company overview: what they do, market position, stated values and strategic direction
- Industry vertical dynamics: trends, competitive landscape, pressures
- Strategic priorities from filings or public statements — quote the specific language
- Third-party reference companies in similar verticals

**STAKEHOLDER MAP**
- Primary contact: name, role, tenure, career path
- Team members: names, roles, product/competitor exposure flags
- Potential executive sponsor or economic buyer (if identifiable from research)
- Warm paths: mutual connections, former colleagues, alumni links

**INTELLIGENCE PLAYS**
- Legislative/regulatory drivers with specific mandates and deadlines
- Filing excerpts signaling our domain as a priority
- Competitor exposure on the team — who used what and when
- Anything that should change the default call strategy

**MEDDPICC TARGETING**
Using the MEDDPICC Qualification Framework and the Discovery Questions reference, identify:
- Which MEDDPICC elements do we already have evidence for based on research?
- Which elements are the primary gaps to probe on this call?
- For each gap, suggest 2-3 questions drawn from the MEDDPICC Discovery Questions reference, adapted to the specific context of this prospect. Start with Tell-level (TED framework) questions for elements where we know the least, and Explain/Describe-level questions for elements where we have partial information.
- Include one cost-of-inaction question tailored to the prospect's domain.
- Include one mutual commitment question for closing the call.

**Output:** A formatted Call Briefing Doc ready for human review and sharing with the SE.

**Present the briefing doc to the AE and pause.** The AE will review, prioritize talking points, share with the SE (and Director if joining), and confirm alignment before the call.

---

### Step 4: Execute the Discovery Call (Human)

This step is fully human. The AE runs the discovery call using the briefing doc and MEDDPICC framework.

**Key principles for the AE:**

**Opening rapport.** The angle — personal, organizational, or industry — is a human judgment call based on your instinct and experience. Use the briefing doc to arm yourself with options but trust your read of the room.

**Confirm the agenda.** "Here's what I planned to cover — does this work for you? Anything you'd add?"

**Pivot to qualification.** Generally within 5 minutes, sometimes within 30 seconds. Read the room.

**If the prospect rapid-fires feature questions,** pump the brakes: "I want to make sure I understand why this is important to you first. Can we start there?" or "Help me understand what the deal-breakers are and why."

**Run the MEDDPICC qualification engine.** Use the TED framework to progressively deepen each topic:
- **Tell me** (open the door) → **Explain to me** (widen the lens to other stakeholders) → **Describe to me** (get to concrete detail and the ideal future state)
- Use "Help me understand X" as the universal unlock when no TED starter feels right
- Key elements to probe, referencing the Discovery Questions:
  - **Identified Pain:** Why change now? Legal imperative? Breach? Consequence of inaction? (Questions 17-19)
  - **Metrics:** What does success look like? What's the cost of inaction? Build the number collaboratively. (Questions 1-3, 24-29)
  - **Economic Buyer:** Who has final authority? Can you meet them? (Questions 4-5)
  - **Champion:** Who gains the most? Will they connect you with the EB? (Questions 20-21)
  - **Decision Criteria:** What criteria exist? Who authored them? Competitor bias? (Questions 6-10)
  - **Decision Process:** What are the steps to a signed contract? (Questions 11-13)
  - **Competition:** Who else is being evaluated? What's the perception? (Questions 22-23)
  - **Paper Process:** What does procurement look like? Timeline? (Questions 14-16)

**Maintain 75/25 talk ratio.** The prospect should be doing 75% of the talking. If you're talking more than 25%, you're presenting, not discovering.

**Close with mutual commitments.** Frame next steps as reciprocal: "If I bring X, will you bring Y?" (Questions 30-32)

**When the call is complete,** provide the model with:
- The call recording or transcript (if available)
- Your notes on key takeaways, surprises, or things that went differently than expected
- The tone of the interaction (formal, business casual, casual) for follow-up calibration
- Any commitments made by either side
- Anything discussed that should NOT be included in the follow-up email

---

### Step 5: Generate Post-Call Follow-up and Mutual Action Plan (AI)

Using the call transcript (or AE's notes), the original briefing doc, and the tone guidance from the AE, generate:

#### 5a. Call Recap Email

- Summarize the key discussion points, decisions made, and action items — attributed to the correct party.
- Match the tone specified by the AE:
  - **Formal:** Professional, structured, no contractions, suitable for executive-level or first interactions with reserved stakeholders
  - **Business casual:** Warm but professional, light contractions okay, suitable for most business relationships
  - **Casual:** Conversational, first-name basis, suitable for established rapport or peer-level conversations
- Do NOT include: sensitive competitive intelligence the prospect shared, internal politics they revealed, or anything the AE specifically flagged for exclusion.
- Keep it concise and professional. The email should reinforce that this AE is organized, attentive, and reliable.
- Close by confirming the agreed-upon next steps with specific dates and owners.

#### 5b. Mutual Action Plan

- List every commitment made by both sides with owners and deadlines where discussed.
- Frame as reciprocal: "We committed to [X] by [date]. You committed to [Y] by [date]."
- If the next step is a second discovery call or demo, specify what each side will bring or prepare.
- Example: "We will provide a tailored agenda and technical presentation addressing your top three use cases. In return, we ask that you bring your [decision-maker / technical lead / etc.] to the next session."

**Output:** A draft follow-up email and a mutual action plan, both ready for human review.

**Present to the AE and pause.** The AE will review tone, adjust content (include/exclude), finalize mutual commitments, and send.

---

### Step 6: MEDDPICC Opportunity Scoring (AI)

Using the call transcript, the research from Step 2, the MEDDPICC Qualification Framework, and the Scoring Criteria reference, produce a scored qualification baseline.

#### Scoring Table

For each MEDDPICC element, apply the rating definitions from the Scoring Criteria reference (Strong / Partial / Gap / Unknown). Require evidence for every rating — if you cannot point to a specific quote, fact, or artifact, the element cannot be rated Strong.

| Element | Confidence | Evidence | Gap / Next Action |
|---------|-----------|----------|-------------------|
| **Metrics** | [Rating] | [Direct quotes or findings] | [What to probe next] |
| **Economic Buyer** | [Rating] | [Who, title, whether met or confirmed] | [What to probe next] |
| **Decision Criteria** | [Rating] | [Stated criteria, author, potential bias] | [What to probe next] |
| **Decision Process** | [Rating] | [Steps, stakeholders, timeline] | [What to probe next] |
| **Paper Process** | [Rating] | [Procurement, legal, compliance steps] | [What to probe next] |
| **Identified Pain** | [Rating] | [The "why change" in the prospect's own words] | [What to probe next] |
| **Champion** | [Rating] | [Who, their influence, actions taken] | [What to probe next] |
| **Competition** | [Rating] | [Who else, prospect's perception, team bias] | [What to probe next] |

#### Stage Gate Assessment

Apply the stage gate minimums from the Scoring Criteria reference:
- Identified Pain must be at least **Partial** to advance
- Champion must be at least **Partial** to advance
- Economic Buyer must be at least **Partial** to advance

If any of these three elements is rated **Gap**, the deal should remain in Qualification/Discovery until the gap is addressed.

#### Overall Assessment

- **Deal stage recommendation:** Advance to Needs Analysis/Value Proposition, stay in Qualification/Discovery, or Deprioritize/Disqualify. State the reasoning based on the scoring table and stage gate assessment.
- **Top 3 gaps to close:** The most critical unknowns that must be addressed in the next interaction. For each gap, reference the specific Discovery Questions that should be used to probe it.
- **Recommended next step:** What type of meeting (second discovery, demo, executive briefing) and who should attend from both sides.

**Scoring discipline:** Score honestly. Resist the temptation to score optimistically — this is the most common failure mode in sales qualification. A "Gap" rating is valuable because it tells you exactly where to focus next. Not everything will be uncovered in a single discovery call. This is a **baseline scorecard**, not a final assessment.

**Output:** A scored MEDDPICC qualification card with the table above, stage gate assessment, overall assessment, and recommended next step.

**Present to the AE and pause.** The AE will review scores, adjust ratings based on judgment and context the model may have missed, and make the final qualify/disqualify decision.

---

## Input Requirements

When running this workflow, provide the following:

| Input | Required | Format | Example |
|-------|----------|--------|---------|
| Stakeholder name | Yes | Text | "Sarah Chen" |
| Stakeholder title | Yes | Text | "VP of Information Security" |
| Company name | Yes | Text | "Acme Financial Services" |
| LinkedIn profile URL | Recommended | URL | https://linkedin.com/in/sarachen |
| How the meeting was booked | Yes | Text | "Inbound demo request via website" or "Referred by John Smith at XYZ Corp" or "Cold outreach, accepted after 3rd touch" |
| Meeting date and time | Yes | Date/Time | "Thursday Feb 13, 2026 at 2:00 PM ET" |
| Who is joining from your side | Yes | Text | "Me + Sarah Kim (SE)" or "Me + Sarah Kim (SE) + James Park (Director)" |
| Who is joining from their side | If known | Text | "Just the prospect" or "Prospect + their team lead + a VAR from PartnerCo" |
| Any prior conversations or context | If applicable | Text | "Had a brief intro call 2 weeks ago. They mentioned compliance pressure." |
| Your company's domain / what you sell | Yes | Text | "Enterprise cybersecurity — endpoint detection and response" |

---

## Context Requirements

These reference materials must be attached to the conversation or pre-loaded in the project:

| File | Purpose | Status |
|------|---------|--------|
| `MEDDICC_Qualification_Framework.md` | MEDDPICC element definitions — the qualification compass for Steps 4 and 6 | Exists |
| `MEDDPICC_Discovery_Questions.md` | Question bank organized by MEDDPICC element, including TED follow-up framework, cost-of-inaction quantification, competitor bias detection, and mutual commitment questions | Exists |
| `MEDDPICC_Scoring_Criteria.md` | Four-level rubric (Strong/Partial/Gap/Unknown) with element-specific criteria, example evidence, and stage gate minimums | Exists |
| `Sales_Stage_Definitions.md` | CRM stage model with entry/exit criteria — governs deal progression recommendations in Step 6 | Exists |

---

## Output Format

This workflow produces the following deliverables across its steps:

| Step | Deliverable | Format |
|------|------------|--------|
| Step 1 | Draft confirmation email with proposed agenda | Text (email body) |
| Step 2 | Structured research package (5 sections: Individual, Team Map, Legislative, Filings, Company/Industry) | Markdown with confidence flags (Verified/Inferred/Gap) |
| Step 3 | Call Briefing Doc (glanceable, titled sections with sub-bullets) | Markdown |
| Step 4 | *(Human step — no AI output)* | — |
| Step 5 | Draft follow-up email + Mutual Action Plan | Text (email body) + Markdown |
| Step 6 | Scored MEDDPICC qualification card with stage gate assessment and next steps | Markdown table + narrative |

### Step 2 Output Format Options (for future Build iterations)
The research outputs from Step 2 can alternatively be presented as:
- **Call Prep Card** — single-page glanceable summary
- **Stakeholder Map Visualization** — visual org chart with relationship and exposure flags
- **Multi-tab Spreadsheet (Excel / Google Sheets)** — structured data across tabs (Stakeholder Profiles, Company Intel, Legislative Drivers, Filing Excerpts)

The right format or combination will be determined based on usage patterns.

---

## Where to Run

### Recommendation: Claude Project

This workflow should be run inside a **Claude Project** for the following reasons:

1. **Frequency** — This workflow runs for every discovery call. A project provides a persistent home.
2. **Multiple context files** — Four reference files are used every run. Pre-load them once instead of attaching each time.
3. **Conversation memory** — The project accumulates context across runs: your writing style, tone preferences, the quality and format of outputs you prefer, patterns in what you adjust during review.
4. **Team adoption** — If other AEs adopt this workflow, they can duplicate the project and run the same prompt with their own inputs.

### Project Setup

**Project name:** MEDDPICC Discovery Workflow

**Project instructions:** Copy the full Instructions section of this prompt (Steps 1-6) into the project's custom instructions.

**Pre-load these files in the project:**
1. `MEDDICC_Qualification_Framework.md`
2. `MEDDPICC_Discovery_Questions.md`
3. `MEDDPICC_Scoring_Criteria.md`
4. `Sales_Stage_Definitions.md`

**Each run:** Start a new conversation in the project. Provide the inputs (stakeholder name, company, meeting context, etc.) and the workflow will execute from Step 1.

---

## Recommended Implementation Order

### Tier 1: Quick Wins (Start Here)

These steps have clear inputs and outputs and can be run immediately with the prompt and context files.

| Priority | Step | What to Do | Why First |
|----------|------|------------|-----------|
| 1 | Step 1: Draft Agenda Email | Run the prompt as-is. Provide meeting context as input. | Fastest to validate. Immediate time savings on every call. |
| 2 | Step 6: MEDDPICC Scoring | Run after your first discovery call with the transcript or notes. The Scoring Criteria file is ready. | Transforms a subjective assessment into a structured, evidence-based scorecard. |
| 3 | Step 5: Post-Call Follow-up | Run immediately after the call with transcript or notes. Select your tone. | Near-instant, polished follow-up is a competitive differentiator. |

### Tier 2: High-Value Semi-Autonomous Steps (Build Next)

These steps require AI to do substantial work with a human review gate.

| Priority | Step | What to Do | Why Next |
|----------|------|------------|----------|
| 4 | Step 3: Call Briefing Doc | Run after Step 2 research is reviewed. Optionally create a `Call_Briefing_Doc_Template.md` if you want to customize the structure beyond what the prompt specifies. | The briefing doc is the bridge between research and the call. High impact on call quality. |
| 5 | Step 2: Research (prompt-only version) | Run Step 2 as-is using web search within Claude. Review outputs for quality and coverage. | Validates the research framework before investing in MCP connectors or agents. |

### Tier 3: Complex Agent Steps (Tackle Last)

These require MCP connectors, multi-tool orchestration, or capabilities beyond a single prompt.

| Priority | Step | What to Build | Why Last |
|----------|------|---------------|----------|
| 6 | Step 2: Research (agent version) | Build MCP connectors for LinkedIn, SEC EDGAR, and web search. Orchestrate as a research agent that runs all five threads in parallel. | Highest automation ROI but highest build complexity. Validate the prompt-only version first. |
| 7 | Step 4: Live AI Coaching (future) | Build an agent that ingests the briefing doc as a system prompt, listens to the call transcript in real time, and provides contextual coaching nudges. | Requires real-time transcription integration and careful UX design. Future iteration. |
| 8 | Step 2: Output Format Options | Build export capabilities for Call Prep Card, Stakeholder Map Visualization, and multi-tab spreadsheet formats. | Presentation layer — valuable for team adoption but not required for the workflow to function. |

### Context Files Status

| File | Status |
|------|--------|
| `MEDDICC_Qualification_Framework.md` | Ready |
| `MEDDPICC_Discovery_Questions.md` | Ready |
| `MEDDPICC_Scoring_Criteria.md` | Ready |
| `Sales_Stage_Definitions.md` | Ready |
| `Call_Briefing_Doc_Template.md` | Optional — prompt contains inline format spec |
| `Mutual_Action_Plan_Template.md` | Optional — prompt contains inline format spec |
| `Agenda_Framework.md` | Deferred — build when the pattern stabilizes |

---

## Deliverable Inventory

This workflow deconstruction produced three files across the Discover, Deconstruct, and Build phases:

| File | Phase | Purpose |
|------|-------|---------|
| `outputs/meddpicc-discovery-prep-call-and-follow-up-definition.md` | Discover | Workflow Definition — structured decomposition of all 6 steps with sub-steps, decision points, data flows, context needs, and failure modes |
| `outputs/meddpicc-discovery-prep-call-and-follow-up-building-blocks.md` | Deconstruct | AI Building Block Map — autonomy classification, building block mapping, tools and connectors, context inventory |
| `outputs/meddpicc-discovery-prep-call-and-follow-up-prompt.md` | Build | Baseline Workflow Prompt — ready-to-use, self-contained prompt with implementation order and project setup guidance (this file) |

### Reference Files Created or Augmented

| File | Status |
|------|--------|
| `Reference Files/MEDDICC_Qualification_Framework.md` | Existed |
| `Reference Files/MEDDPICC_Discovery_Questions.md` | Augmented — added TED framework, cost-of-inaction, competitor bias detection, mutual commitments |
| `Reference Files/MEDDPICC_Scoring_Criteria.md` | Created — four-level rubric with element-specific criteria and stage gate minimums |
| `Reference Files/Sales_Stage_Definitions.md` | Created — 6 CRM stages with entry/exit criteria |
