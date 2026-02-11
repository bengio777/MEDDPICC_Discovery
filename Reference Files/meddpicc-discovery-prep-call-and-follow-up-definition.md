# Workflow Definition: MEDDPICC Discovery Prep, Call, and Follow-up

## Scenario Metadata

| Field | Value |
|---|---|
| **Workflow Name** | MEDDPICC Discovery Prep, Call, and Follow-up |
| **Description** | End-to-end workflow for an enterprise AE to research, prepare for, execute, and follow up on a discovery call with a senior stakeholder, using MEDDPICC to qualify the opportunity. |
| **Outcome** | A qualified (or disqualified) opportunity with MEDDPICC criteria assessed, CRM updated, and next steps defined. |
| **Trigger** | A discovery call is scheduled with a Director of Security or above at a target account. |
| **Type** | Augmented (human-driven, AI-augmented) |
| **Business Objective** | Be better prepared, ask better questions, follow up more quickly, and present a more polished and courteous interaction than the average sales rep — and more importantly, than the competitor's sales rep. The competitive edge is not the AI; it is the AE who shows up better prepared than anyone else in the deal. |
| **Current Owner(s)** | Strategic/Enterprise Account Executive, supported by Sales Engineer (and occasionally Director of Sales) |
| **Business Process** | Revenue Operations |
| **Lifecycle Position** | Spans Prospecting/Research through Qualification/Discovery. The scored MEDDPICC baseline serves as the stage gate into Needs Analysis/Value Proposition. |

---

## Refined Steps

### Step 1: Send Agenda and Confirmation Email

| Field | Detail |
|---|---|
| **Action** | Send a confirmation email with a proposed agenda to the prospect. Command the process and message while inviting collaboration. Introduce any team members who will be joining the call. |
| **Sub-steps** | 1. Draft a proposed agenda based on deal context (how meeting was booked, prior conversations, stakeholder seniority). 2. Determine who from your side joins the call. 3. Introduce team members joining (SE, Director if applicable). 4. Send with a tone that is confident but collaborative — "Here's what I'd like to cover. What would you add?" |
| **Decision Points** | Who joins from your side depends on: (a) whether the prospect is bringing a VAR, (b) stakeholder seniority, (c) whether it is a 1:1 or multi-party meeting. Default is AE + SE. Escalate to include Director of Sales when warranted. |
| **Data In** | Meeting context (how it was booked, who requested it, any prior conversations), stakeholder name and title. |
| **Data Out** | Sent confirmation email with proposed agenda. Prospect's response (acceptance, modifications, or silence). |
| **Context Needs** | Agenda framework/template (deferred to future iteration). |
| **Failure Modes** | Prospect does not respond. Prospect pushes back on the agenda. Prospect attempts to reschedule or delegate to someone more junior. |

---

### Step 2: Stakeholder and Organization Research

| Field | Detail |
|---|---|
| **Action** | Conduct deep research on the individual stakeholder, their team, their organization, and the broader market and regulatory context. This is a single continuous activity with expanding scope — individual, then their history, then their org's principles and directives, then how it all filters down to this person. |
| **Sub-steps** | 1. Research primary stakeholder on LinkedIn — role, tenure, career history, recent posts, mutual connections. 2. Map the stakeholder's team — who reports to them, who are peers, who has prior experience with your product or competitors' products. 3. Research legislative and regulatory drivers relevant to their industry vertical. 4. Scan public financial filings (10-K, 8-K, 5-K, investor statements) for strategic priority signals — has the company stated your domain or the broader problem space as a priority, and to what degree of specificity? 5. Identify the organization's guiding principles, directives, and how they flow through business units and teams to the individual. 6. Identify companies in similar domains or verticals for potential third-party stories or references. |
| **Decision Points** | If a team member previously used your product — that is leverage. Learn about their experience. If they used a competitor — learn whether it was positive or negative and use that as leverage. These findings change call strategy. If a filing explicitly names your domain as a priority, that escalates the opportunity and may change the agenda. |
| **Data In** | Stakeholder name, title, company, LinkedIn profile URL. |
| **Data Out** | Stakeholder map (primary contact + team members with roles and history). List of mutual connections and warm paths. Legislative/regulatory drivers relevant to their vertical. Financial filing excerpts signaling strategic priority. Companies in similar domains for third-party reference stories. |
| **Context Needs** | General awareness of competitor landscape and relevant legislation by vertical (not hardcoded lists — this is a framework). LinkedIn access. Public filing sources (SEC EDGAR, investor relations pages). |
| **Failure Modes** | Stakeholder has a thin LinkedIn profile. Company is private with no public filings. Team structure cannot be determined. Legislative landscape is ambiguous or does not clearly apply. |

---

### Step 3: Build the Call Briefing Doc

| Field | Detail |
|---|---|
| **Action** | Synthesize all research into a structured, scannable briefing document formatted for glanceable reference during the live call. Share with SE (and Director if joining). |
| **Sub-steps** | 1. Synthesize research outputs into a structured doc. 2. Organize into distinct sections — each with a bold title and sub-bullets for rapid visual parsing: personal rapport angles (hobbies, shared interests, mutual connections), company and industry talking points (core values, vertical dynamics, strategic priorities from filings), specific intelligence plays (competitor history on their team, legislative drivers, warm paths). 3. Share with SE and any other team members joining the call to ensure alignment on account story and strategy. |
| **Decision Points** | Does the briefing doc differ based on who is joining the call? Does the SE get the same doc or a tailored version? Which talking points are "use if the conversation goes here" versus "definitely bring up"? |
| **Data In** | All outputs from Step 2 (stakeholder map, research findings, filing excerpts, legislative drivers). |
| **Data Out** | Formatted briefing doc. Aligned call team. |
| **Context Needs** | Call briefing doc template (needs creation) — consistent structure with titled sections and highlighted sub-bullets. Future state: this doc becomes the system prompt for live AI coaching during the call. |
| **Failure Modes** | Research was thin so the doc has gaps. SE does not review the doc before the call. Doc is too dense to glance at mid-conversation. Key intelligence gets buried in the format. |

---

### Step 4: Execute the Discovery Call

| Field | Detail |
|---|---|
| **Action** | Run the discovery call using the MEDDPICC framework to qualify the opportunity. The foundational principle is to determine whether there is sufficient pain to dictate action on a business decision. Maintain a 75/25 prospect-to-seller talk ratio. |
| **Sub-steps** | 1. Open with rapport — use briefing doc to connect on something personal, organizational, or industry-specific. The rapport angle is a human judgment call based on the AE's unique experience and instinct to develop a human relationship. 2. Confirm the agenda and invite additions. 3. Run the MEDDPICC qualification engine — work through key questions: Why change? (legal imperative, breach, consequence of inaction). Who are the key stakeholders and executive sponsor? Is there allocated budget? What gets in the way of this project? What is their personal stake? What happens if it goes poorly? What is the cost of inaction — have they calculated it? Who is the champion? Do they have defined decision criteria and who prepared them? (Research whether those people have competitor bias.) 4. Maintain 75/25 talk ratio using TED framework (Tell me, Explain to me, Describe to me) and "Help me understand X." 5. If prospect rapid-fires feature questions, redirect to pain — "I don't even understand why this is important to you. Can we start there?" 6. Identify and agree on next steps before closing. |
| **Decision Points** | Rapport angle is a human art — not scriptable. Pivot timing from rapport to qualification is instinct-driven (generally within 5 minutes, sometimes 30 seconds). If a VAR is on the call, conversation dynamics change. If prospect reveals weak pain or no budget, determine whether to push through full qualification or adjust. |
| **Data In** | Briefing doc (Step 3), confirmed agenda (Step 1), MEDDPICC framework. |
| **Data Out** | Qualification data against each MEDDPICC element. New intelligence (stakeholders not previously known, internal politics, timelines, pain depth). Agreed-upon next steps. Call recording/transcript. |
| **Context Needs** | MEDDPICC Qualification Framework (exists — reference file). Briefing doc from Step 3. TED questioning framework (informal — exists as technique). Future integration: battlecards, competitive positioning, ROI data, industry reports for credibility building. The goal is not to look smart but to demonstrate competency and orient your qualified expertise and specific experience. |
| **Failure Modes** | Prospect is guarded and will not open up. Prospect dominates with their own agenda. Key MEDDPICC elements go unanswered. Champion is not who you thought. Decision criteria were written by a competitor's ally. Call runs short on time. |

---

### Step 5: Post-Call Follow-up and Mutual Action Plan

| Field | Detail |
|---|---|
| **Action** | Generate an AI-drafted call recap for human review. Send follow-up email with recap, next steps, and mutual commitments. The follow-up should be near-instant, polished, and tone-appropriate. |
| **Sub-steps** | 1. AI-generated call recap — transcription, key points, action items — served up for human review. 2. AE selects tone (formal, business casual, or casual) based on how the conversation actually went. 3. Review, edit, and send the follow-up email with recap, agreed-upon next steps, and mutual commitments. 4. Define mutual outcome success plan — reciprocal commitments with specific deliverables and owners on both sides. Example: "If I provide you a well-articulated agenda and a high-caliber presentation, you bring your decision-maker to the next meeting." |
| **Decision Points** | Tone selection is a human call based on rapport established during the call. What gets included vs. excluded from the recap — some things discussed (competitive intelligence shared, internal politics revealed) may be deliberately left out of the email. Whether the mutual action plan goes in the same email or as a separate artifact. |
| **Data In** | Call recording/transcription, notes, briefing doc context. |
| **Data Out** | Follow-up email with recap and next steps. Mutual action plan with reciprocal commitments. Future state: CRM updates. |
| **Context Needs** | Call transcription tool (future integration — Gong, Otter, Fireflies, or similar). Email drafting with tone calibration. Mutual action plan template (needs creation). |
| **Failure Modes** | Recap misses key points or misinterprets context. Tone is wrong for the relationship. Prospect agreed to next steps verbally but goes silent after the email. Mutual commitments are vague and unenforceable. |

---

### Step 6: MEDDPICC Opportunity Scoring

| Field | Detail |
|---|---|
| **Action** | AI analyzes the call transcript and research against each MEDDPICC element to produce a scored qualification baseline for human review. This is a living scorecard — a first discovery call may only fill 2-3 elements with confidence. The rest get refined across subsequent interactions. |
| **Sub-steps** | 1. AI analyzes call transcript and research against each MEDDPICC element: Metrics, Economic Buyer, Decision Criteria, Decision Process, Identified Pain, Champion, Competition (and Paper Process if applicable). 2. For each element, assign a confidence rating (strong / partial / gap / unknown) with supporting evidence pulled from the transcript. 3. Surface specific gaps — e.g., "Budget not discussed," "Champion identified but not validated," "Decision criteria exist but author's competitor affiliation unknown." 4. Present the scorecard for human review and adjustment. |
| **Decision Points** | Based on the score, does this deal move forward, get deprioritized, or get disqualified? What threshold applies — are some elements deal-breakers on their own (e.g., no Identified Pain)? Not everything will be uncovered in a single discovery call — this is the baseline, not the final answer. |
| **Data In** | Call transcript, research from Step 2, MEDDPICC framework reference, follow-up commitments from Step 5. |
| **Data Out** | Scored MEDDPICC qualification card with confidence ratings, evidence, and gap analysis. This score serves as the stage gate from Qualification/Discovery into Needs Analysis/Value Proposition. |
| **Context Needs** | MEDDPICC Qualification Framework (exists — reference file). Scoring criteria defining what constitutes strong/partial/gap per element (needs creation). |
| **Failure Modes** | AI misinterprets nuance in the conversation. Scores too optimistically (common bias in sales). Misses implicit signals. AE overrides the score without justification. |

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

## Context Shopping List

| Artifact | Description | Used By Steps | Status | Key Contents |
|---|---|---|---|---|
| **MEDDPICC Qualification Framework** | Qualification element definitions — Metrics, Economic Buyer, Decision Criteria, Decision Process, Identified Pain, Champion, Competition, Paper Process | 4, 6 | Exists | 7 elements + Paper Process variant. Reference file: `Reference Files/MEDDICC_Qualification_Framework.md` |
| **Sales Stage Definitions** | CRM stage model from Prospecting through Closed Won/Lost | 1, 4, 5, 6 | Exists (informal) | 6 stages: Prospecting/Research, Qualification/Discovery, Needs Analysis/Value Proposition, Proposal/Quote, Negotiation & Commitment, Closed Won/Lost. Governs where this workflow sits and what stage the deal advances to. |
| **TED Questioning Framework** | Conversational technique: Tell me, Explain to me, Describe to me | 4 | Exists (informal) | Technique for maintaining 75/25 prospect-to-seller talk ratio. Includes "Help me understand X." |
| **Agenda Framework/Template** | Structured agenda for first discovery calls | 1 | Needs Creation (deferred) | Standard topics, customizable sections, collaborative tone |
| **Call Briefing Doc Template** | Scannable format with titled sections and sub-bullets for glanceable reference during calls | 3 | Needs Creation | Sections: rapport angles, company intel, stakeholder map, legislative drivers, filing excerpts, third-party reference stories |
| **Mutual Action Plan Template** | Reciprocal commitment framework for post-call follow-up | 5 | Needs Creation | "If I do X, you do Y" structure with deliverables and owners |
| **MEDDPICC Scoring Criteria** | Definitions of what constitutes strong/partial/gap/unknown per element | 6 | Needs Creation | Confidence ratings with evidence requirements |
| **Stakeholder LinkedIn Data** | Profile, career history, posts, connections, team mapping | 2, 3 | Gathered per deal | Individual + team member mapping, competitor/product exposure history |
| **Public Financial Filings** | 10-K, 8-K, 5-K, investor statements | 2, 3 | Gathered per deal | Strategic priority signals in your domain, degree of specificity |
| **Legislative/Regulatory Drivers** | Compliance mandates relevant to prospect's vertical | 2, 3, 4 | Gathered per deal | Industry-specific legal imperatives driving action |
| **Battlecards & Competitive Positioning** | Competitor strengths/weaknesses, differentiation, objection handling | 4 | Future integration | Product comparison, competitive intelligence |
| **ROI Data & Industry Reports** | Credibility-building data points and analyst findings | 4 | Future integration | Metrics, case studies, industry benchmarks |
| **Call Transcription Tool** | Recording, transcription, key point extraction | 5, 6 | Future integration | Gong, Otter, Fireflies, or similar |
| **CRM** | Deal tracking, stage management, contact and account records | All | Future integration | Salesforce or equivalent — not integrated in this proof of concept |
