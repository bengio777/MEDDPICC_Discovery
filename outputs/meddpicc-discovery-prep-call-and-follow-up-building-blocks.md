# AI Building Block Map: MEDDPICC Discovery Prep, Call, and Follow-up

## Scenario Summary

| Field | Value |
|---|---|
| **Workflow Name** | MEDDPICC Discovery Prep, Call, and Follow-up |
| **Description** | End-to-end workflow for an enterprise AE to research, prepare for, execute, and follow up on a discovery call with a senior stakeholder, using MEDDPICC to qualify the opportunity. |
| **Outcome** | A qualified (or disqualified) opportunity with MEDDPICC criteria assessed, CRM updated, and next steps defined. |
| **Trigger** | A discovery call is scheduled with a Director of Security or above at a target account. |
| **Type** | Augmented (human-driven, AI-augmented) |
| **Business Objective** | Be better prepared, ask better questions, follow up more quickly, and present a more polished and courteous interaction than the average sales rep — and more importantly, than the competitor's sales rep. The competitive edge is not the AI; it is the AE who shows up better prepared than anyone else in the deal. |
| **Current Owner(s)** | Strategic/Enterprise Account Executive, supported by Sales Engineer (and occasionally Director of Sales) |

---

## Step-by-Step Decomposition

| # | Step | Action | Autonomy | Decision Points | Failure Mode | Data In | Data Out | Context Needed | AI Building Block(s) | Human Gate |
|---|------|--------|----------|----------------|-------------|---------|----------|----------------|----------------------|------------|
| 1 | Send Agenda & Confirmation Email | Draft and send a confirmation email with proposed agenda. Command the process while inviting collaboration. Introduce team members joining. | AI-Semi-Autonomous | Who joins from your side (VAR present, seniority, 1:1 vs. multi-party). Default: AE + SE. | No response. Pushback on agenda. Reschedule or delegation to junior. | Meeting context (how booked, prior conversations), stakeholder name and title. | Sent confirmation email with proposed agenda. Prospect's response. | Agenda framework/template (deferred). | **Prompt** (email drafting), **Context** (meeting context, stakeholder info, agenda framework) | Review and approve email before sending. |
| 2 | Stakeholder & Organization Research | Conduct deep research on the individual stakeholder, their team, their organization, and broader market/regulatory context. Single continuous activity with expanding scope. | AI-Semi-Autonomous | Prior product/competitor experience changes call strategy. Filing language naming your domain escalates priority. | Thin LinkedIn profiles. Private company with no filings. Can't map team structure. Ambiguous regulatory landscape. | Stakeholder name, title, company, LinkedIn profile URL. | Stakeholder map, mutual connections, legislative drivers, filing excerpts, similar companies for third-party stories. | General competitor landscape awareness. Relevant legislation by vertical. LinkedIn access. Public filing sources. | **Agent** (orchestrates parallel research threads), **MCP** (LinkedIn, SEC EDGAR, web search), **Context** (competitor landscape, vertical knowledge) | Review research outputs for accuracy and strategic relevance. |
| 3 | Build Call Briefing Doc | Synthesize all research into a structured, scannable briefing document for glanceable reference during the live call. Share with SE. | AI-Semi-Autonomous | Does the doc differ by audience? Which talking points are conditional vs. definite? | Research was thin — doc has gaps. SE doesn't review before call. Doc too dense to glance mid-conversation. Key intel gets buried. | All Step 2 outputs (stakeholder map, research findings, filing excerpts, legislative drivers). | Formatted briefing doc. Aligned call team. | Call briefing doc template (needs creation). | **Skill** (briefing doc generation), **Prompt** (synthesis and formatting instructions), **Context** (research outputs, template) | Review briefing doc before sharing with team. |
| 4 | Execute the Discovery Call | Run the discovery call using MEDDPICC to qualify the opportunity. Determine whether sufficient pain exists to dictate action. Maintain 75/25 talk ratio. | Human | Rapport angle (human judgment). Pivot timing (instinct-driven). VAR dynamics. Weak pain or no budget — adjust or push through. | Prospect guarded. Prospect dominates agenda. Key MEDDPICC elements unanswered. Champion misidentified. Decision criteria written by competitor ally. Time runs short. | Briefing doc (Step 3), confirmed agenda (Step 1), MEDDPICC framework. | Qualification data per MEDDPICC element. New intelligence. Agreed next steps. Call recording/transcript. | MEDDPICC framework (exists). Briefing doc. TED framework (informal). Future: battlecards, competitive positioning, ROI data, industry reports. | **Context** (MEDDPICC framework, briefing doc, TED framework). Future state: **Agent** (live coaching). | The entire step IS human. |
| 5 | Post-Call Follow-up & Mutual Action Plan | Generate AI-drafted call recap for human review. Send follow-up email with recap, next steps, and mutual commitments. Near-instant, polished, tone-appropriate. | AI-Semi-Autonomous | Tone selection (formal / business casual / casual). What to include vs. exclude. Mutual action plan in same email or separate. | Recap misses key points. Wrong tone. Prospect goes silent. Mutual commitments are vague. | Call recording/transcription, notes, briefing doc context. | Follow-up email with recap and next steps. Mutual action plan with reciprocal commitments. | Call transcription tool (future). Email drafting with tone calibration. Mutual action plan template (needs creation). | **Skill** (follow-up email generation), **Prompt** (recap generation, tone-calibrated drafting), **Context** (transcript, mutual action plan template) | Tone selection, content filtering (include/exclude), send approval. |
| 6 | MEDDPICC Opportunity Scoring | AI analyzes call transcript and research against each MEDDPICC element. Produce scored qualification baseline for human review. Living scorecard — first call may only fill 2-3 elements. | AI-Semi-Autonomous | Does deal move forward, get deprioritized, or get disqualified? Are some elements deal-breakers on their own? | AI misinterprets nuance. Scores too optimistically. Misses implicit signals. AE overrides without justification. | Call transcript, research from Step 2, MEDDPICC framework, follow-up commitments from Step 5. | Scored MEDDPICC qualification card with confidence ratings, evidence, and gap analysis. Stage gate into Needs Analysis/Value Proposition. | MEDDPICC framework (exists). Scoring criteria (needs creation). | **Skill** (MEDDPICC scoring), **Prompt** (scoring instructions), **Context** (MEDDPICC framework, scoring criteria, transcript) | Review scores, adjust ratings, make qualify/disqualify decision. |

---

## Step 2: Output Format Options

The research outputs from Step 2 can be presented in multiple formats. The right format (or combination) will be determined in the Build phase:

| Format | Description | Use Case |
|---|---|---|
| **Call Prep Card** | Single-page, glanceable summary of key research findings | Quick reference before and during the call |
| **Stakeholder Map Visualization** | Visual representation of org structure, relationships, and product/competitor exposure history | Understanding the political landscape and influence paths |
| **Spreadsheet (Excel / Google Sheets)** | Multi-tab structured data (e.g., Stakeholder Profiles, Company Intel, Legislative Drivers, Filing Excerpts) | Detailed reference and ongoing data capture across the deal cycle |

Note: The Call Prep Card and the Briefing Doc (Step 3) may converge into a single artifact or remain separate depending on how they are used in practice.

---

## Autonomy Spectrum Summary

| Level | Steps | Count |
|---|---|---|
| **Human** | Step 4 (Execute the Discovery Call) | 1 |
| **AI-Semi-Autonomous** (with human review gates) | Steps 1, 2, 3, 5, 6 | 5 |
| **AI-Deterministic** | — | 0 |
| **AI-Autonomous** | — | 0 |

Every AI-augmented step includes a human-in-the-loop gate. Nothing goes out the door or advances the deal without the AE's judgment.

---

## Step Sequence and Dependencies

### Sequential Flow

```
Step 1: Send Agenda & Confirmation Email
    │ (can run in parallel with Step 2)
Step 2: Stakeholder & Organization Research
    │
    ▼
Step 3: Build Call Briefing Doc
    │
    ▼
Step 4: Execute the Discovery Call
    │
    ▼
Step 5: Post-Call Follow-up & Mutual Action Plan
    │
    ▼
Step 6: MEDDPICC Opportunity Scoring
```

### Parallel Opportunities
- **Steps 1 and 2** can run concurrently — send the confirmation email while beginning research.

### Critical Path
Research (2) → Briefing Doc (3) → Call (4) → Follow-up (5) → Scoring (6)

### Dependency Map

| Step | Depends On |
|---|---|
| Step 1: Send Agenda & Confirmation Email | Trigger (call scheduled) |
| Step 2: Stakeholder & Organization Research | Trigger (call scheduled) |
| Step 3: Build Call Briefing Doc | Step 2 (research outputs) |
| Step 4: Execute the Discovery Call | Steps 1 + 3 (confirmed agenda + briefing doc) |
| Step 5: Post-Call Follow-up & Mutual Action Plan | Step 4 (call must have happened) |
| Step 6: MEDDPICC Opportunity Scoring | Steps 4 + 5 (transcript + research + commitments) |

### Workflow Boundary
This workflow ends at the scored MEDDPICC baseline. Downstream activities (second discovery call, demo, deeper qualification) are separate workflows that stitch to this one. The scoring output serves as the stage gate from Qualification/Discovery into Needs Analysis/Value Proposition.

---

## Prerequisites

### What Must Be in Place
- A discovery call has been scheduled with a Director of Security or above
- Stakeholder name, title, and company are known
- AE has access to LinkedIn for research
- MEDDPICC Qualification Framework is available as reference (exists: `Reference Files/MEDDICC_Qualification_Framework.md`)

### External Dependencies
- LinkedIn access (profile research, team mapping, activity monitoring)
- Public financial filing access (SEC EDGAR, investor relations pages)
- Web search access (legislative research, company intel, industry context)
- Email client access (confirmation and follow-up emails)
- Video conferencing with recording capability (call execution)
- Call transcription tool (future integration — Gong, Otter, Fireflies, or similar)
- CRM access (future integration — Salesforce or equivalent)

---

## Context Inventory

| Artifact | Type | Description | Used By Steps | Status | Format | Key Contents |
|----------|------|-------------|---------------|--------|--------|--------------|
| MEDDPICC Qualification Framework | Reference | Qualification element definitions — M, E, D, D, I, C, C + Paper Process | 4, 6 | Exists | Markdown | 7 elements + Paper Process variant. File: `Reference Files/MEDDICC_Qualification_Framework.md` |
| Sales Stage Definitions | Reference | CRM stage model from Prospecting through Closed Won/Lost | 1, 4, 5, 6 | Exists (informal) | Informal | 6 stages: Prospecting/Research, Qualification/Discovery, Needs Analysis/Value Proposition, Proposal/Quote, Negotiation & Commitment, Closed Won/Lost |
| TED Questioning Framework | Reference | Conversational technique: Tell me, Explain to me, Describe to me | 4 | Exists (informal) | Informal | Technique for 75/25 prospect-to-seller talk ratio. Includes "Help me understand X." |
| Agenda Framework/Template | Template | Structured agenda for first discovery calls | 1 | Needs Creation (deferred) | TBD | Standard topics, customizable sections, collaborative tone |
| Call Briefing Doc Template | Template | Scannable format with titled sections and sub-bullets | 3 | Needs Creation | TBD | Rapport angles, company intel, stakeholder map, legislative drivers, filing excerpts, third-party reference stories |
| Mutual Action Plan Template | Template | Reciprocal commitment framework | 5 | Needs Creation | TBD | "If I do X, you do Y" structure with deliverables and owners |
| MEDDPICC Scoring Criteria | Reference | What constitutes strong/partial/gap/unknown per element | 6 | Needs Creation | TBD | Confidence ratings with evidence requirements |
| Stakeholder LinkedIn Data | Research Data | Profile, career history, posts, connections, team | 2, 3 | Gathered per deal | Varies | Individual + team mapping, competitor/product exposure |
| Public Financial Filings | Research Data | 10-K, 8-K, 5-K, investor statements | 2, 3 | Gathered per deal | PDF/HTML | Strategic priority signals, degree of specificity |
| Legislative/Regulatory Drivers | Research Data | Compliance mandates relevant to vertical | 2, 3, 4 | Gathered per deal | Varies | Industry-specific legal imperatives |
| Battlecards & Competitive Positioning | Reference | Competitor analysis and differentiation | 4 | Future integration | TBD | Product comparison, objection handling |
| ROI Data & Industry Reports | Reference | Credibility-building data points | 4 | Future integration | TBD | Metrics, case studies, benchmarks |

---

## Tools and Connectors Required

| Tool / Connector | Purpose | Used By Steps | Status | Building Block Type |
|---|---|---|---|---|
| LinkedIn | Stakeholder research, team mapping, activity monitoring, mutual connections | 2 | Needed | MCP |
| SEC EDGAR / Financial Filing Sources | Public company filings, investor statements, strategic priority analysis | 2 | Needed | MCP or Web Search |
| Web Search | Legislative research, company intel, industry context, competitor landscape | 2 | Needed | MCP or Agent capability |
| Email Client | Send agenda confirmation (Step 1) and follow-up email (Step 5) | 1, 5 | Exists | Future MCP integration |
| Video Conferencing + Recording | Call execution and recording | 4 | Exists | External tool |
| Call Transcription (Gong, Otter, Fireflies) | Transcription, key points, action items | 5, 6 | Future integration | MCP or API |
| CRM (Salesforce or equivalent) | Deal tracking, stage management, contact records | All | Future integration | MCP or API |
| Document Generation | Briefing doc, call prep card, stakeholder map outputs | 2, 3 | Needed | Skill / Prompt output |
| Spreadsheet (Excel / Google Sheets) | Multi-tab structured research data | 2 | Option (Build phase) | Export / API |

---

## AI Building Block Summary

| Building Block | Where Used | Purpose |
|---|---|---|
| **Prompt** | Steps 1, 2, 3, 5, 6 | Email drafting, research instructions, synthesis/formatting, recap generation, tone calibration, scoring instructions |
| **Context** | All steps | MEDDPICC framework, meeting context, research outputs, templates, transcript, scoring criteria |
| **Skill** | Steps 3, 5, 6 | Briefing doc generation, follow-up email generation, MEDDPICC scoring |
| **Agent** | Step 2 (primary), Step 4 (future) | Research orchestration across multiple sources (Step 2). Future: live call coaching (Step 4). |
| **MCP** | Step 2 | LinkedIn, SEC EDGAR, web search connectors |
| **Project** | — | The workflow itself, once built, constitutes a Project-level building block |
