# AI Building Block Spec: MEDDPICC Discovery Prep, Call, and Follow-up

## Execution Pattern
**Recommended Pattern:** Prompt with Context Files (Claude Project)
**Reasoning:**
- This workflow runs in Claude Project (web UI), not Claude Code — no skill/plugin infrastructure available
- The prompt orchestrates the full 11-step flow with 4 pre-loaded context files providing domain expertise
- Step 3 (research) is designed for multi-agent orchestration with 5 parallel threads, but executes as a single prompt with web search in the current implementation
- Every AI output has a mandatory human review gate — the prompt pattern supports this conversational back-and-forth naturally
- No MCP connectors or tool integrations required — outputs are emails, documents, and scorecards consumed by the AE

---

## Scenario Summary
| Field | Value |
|-------|-------|
| **Workflow Name** | MEDDPICC Discovery Prep, Call, and Follow-up |
| **Description** | End-to-end workflow for an enterprise AE to research, prepare for, execute, and follow up on a discovery call with a senior stakeholder, using MEDDPICC to qualify the opportunity. |
| **Process Outcome** | A qualified (or disqualified) opportunity with MEDDPICC criteria assessed and next steps defined. |
| **Trigger** | A discovery call is scheduled with a Director of Security or above at a target account. |
| **Type** | Augmented |
| **Business Process** | Revenue Operations / Sales Execution |

---

## Step-by-Step Decomposition
| Step | Name | Autonomy Level | Building Block(s) | Tools / Connectors | Skill Candidate | HITL Gate |
|------|------|---------------|-------------------|-------------------|----------------|-----------|
| 1 | Draft agenda & confirmation email | AI-Semi-Autonomous | Prompt, Context | — | — | — |
| 2 | Review and send confirmation email | Human | — | Email client | — | AE approves and sends |
| 3 | Research stakeholder & organization | AI-Semi-Autonomous | Prompt, Context, Web Search | Web Search, LinkedIn (manual) | — | — |
| 4 | Review research outputs | Human | — | — | — | AE validates findings |
| 5 | Build call briefing doc | AI-Semi-Autonomous | Prompt, Context | — | — | — |
| 6 | Review briefing & align with team | Human | — | — | — | AE + SE align on strategy |
| 7 | Execute discovery call | Human | Context (briefing doc) | Video conferencing, recording | — | The entire step IS human |
| 8 | Generate follow-up & mutual action plan | AI-Semi-Autonomous | Prompt, Context | — | — | — |
| 9 | Review and send follow-up | Human | — | Email client | — | AE approves and sends |
| 10 | Score opportunity against MEDDPICC | AI-Semi-Autonomous | Prompt, Context | — | — | — |
| 11 | Review scores & qualification decision | Human | — | — | — | AE makes final call |

## Autonomy Spectrum Summary

```
|--Human--------------------|--AI-Semi-Autonomous---------|--AI-Autonomous--|
    2, 4, 6, 7, 9, 11           1, 3, 5, 8, 10
```

| Level | Steps | Count |
|-------|-------|-------|
| **Human** | Steps 2, 4, 6, 7, 9, 11 | 6 |
| **AI-Semi-Autonomous** (with human review) | Steps 1, 3, 5, 8, 10 | 5 |
| **AI-Deterministic** | — | 0 |
| **AI-Autonomous** | — | 0 |

Every AI-augmented step includes a human-in-the-loop gate. Nothing goes out the door or advances the deal without the AE's judgment.

---

## Skill Candidates

This workflow runs in Claude Project, not Claude Code, so there are no formal skill files. The building blocks are the prompt (workflow instructions) and 4 context files that provide domain expertise.

### Prompt: MEDDPICC Discovery Workflow
- **Purpose:** Orchestrate the 11-step workflow from agenda email through MEDDPICC scoring.
- **Inputs:**

| Input | Source | Required |
|-------|--------|----------|
| Stakeholder name, title, company | AE | Yes |
| LinkedIn URL | AE | Yes |
| Meeting context (how booked, date/time, attendees) | AE | Yes |
| Call notes / transcript | AE (post-call) | Yes (for Steps 8-10) |
| Tone selection (formal / business casual / casual) | AE (post-call) | Yes (for Step 8) |
| Exclusions (sensitive info to omit) | AE (post-call) | No |

- **Outputs:**

| Output | Destination | Format |
|--------|-------------|--------|
| Confirmation email with agenda | Prospect (via email) | Email draft |
| Research package (5 sections) | AE review | Markdown with confidence flags |
| Call briefing doc | AE + SE (shared) | Markdown — glanceable format |
| Follow-up email with recap | Prospect (via email) | Email draft |
| Mutual action plan | Prospect + AE | Markdown with owners and deadlines |
| MEDDPICC scorecard | AE (internal) | Markdown table + narrative |

- **Decision Logic:**
  - Research confidence: every finding flagged as Verified (sourced), Inferred (reasonable conclusion), or Gap (unknown — probe on call)
  - MEDDPICC scoring: Strong (can quote the prospect), Partial (paraphrasing), Gap (no evidence), Unknown (not discussed)
  - Stage gate: Identified Pain, Champion, and Economic Buyer must each be at least Partial to advance
  - Deal recommendation: qualify, deprioritize, or disqualify based on scorecard + gap analysis

- **Failure Modes:**

| Failure | Impact | Handling |
|---------|--------|----------|
| Thin research (private company, minimal LinkedIn) | Briefing doc has gaps | Flag gaps explicitly; prioritize as call objectives |
| AI scores too optimistically | False confidence in deal | Apply Strong vs. Partial test: can you quote, or are you paraphrasing? |
| Prospect goes silent post-follow-up | Deal stalls | Review mutual commitments for specificity; follow up referencing reciprocal agreement |
| MEDDPICC mostly Gap after first call | Incomplete qualification | Normal for first discovery — focus top 3 gaps for next interaction |

---

## Step Sequence and Dependencies

```
Step 1: Draft agenda email [AI]
    │ (can run in parallel with Step 3)
Step 2: Review and send [Human]
    │
Step 3: Research stakeholder & org [AI — 5 parallel threads]
    │
    ▼
Step 4: Review research [Human]
    │
    ▼
Step 5: Build call briefing doc [AI]
    │
    ▼
Step 6: Review briefing & align with team [Human]
    │
    ▼
Step 7: Execute discovery call [Human]
    │
    ▼
Step 8: Generate follow-up & mutual action plan [AI]
    │
    ▼
Step 9: Review and send follow-up [Human]
    │
    ▼
Step 10: Score opportunity against MEDDPICC [AI]
    │
    ▼
Step 11: Review scores & qualification decision [Human]
```

### Dependency Map

| Step | Depends On |
|------|-----------|
| Step 1 | Trigger (call scheduled, meeting inputs provided) |
| Step 2 | Step 1 (email drafted) |
| Step 3 | Trigger (stakeholder info known) |
| Step 4 | Step 3 (research complete) |
| Step 5 | Step 4 (research validated) |
| Step 6 | Step 5 (briefing doc generated) |
| Step 7 | Steps 2 + 6 (email sent, briefing reviewed, team aligned) |
| Step 8 | Step 7 (call executed, notes/transcript provided) |
| Step 9 | Step 8 (follow-up drafted) |
| Step 10 | Steps 3 + 8 (research + call evidence) |
| Step 11 | Step 10 (scorecard generated) |

### Parallel Opportunities
- Steps 1 and 3 can run concurrently — send confirmation while beginning research.
- Step 3 internally runs 5 parallel research threads (individual, team, legislative, financial, company).

### Critical Path
Research (3) → Briefing (5) → Call (7) → Follow-up (8) → Scoring (10)

---

## Prerequisites
- Discovery call scheduled with a Director of Security or above
- Stakeholder name, title, and company are known
- Claude Project set up with all four context files pre-loaded
- LinkedIn access for stakeholder and team research
- Access to public financial filing sources (SEC EDGAR, investor relations pages)

## Context Inventory

| Artifact | Type | Used By Steps | Status |
|----------|------|---------------|--------|
| MEDDPICC_Qualification_Framework.md | Reference | 7, 10 | Exists |
| MEDDPICC_Discovery_Questions.md | Reference | 5, 7 | Exists |
| MEDDPICC_Scoring_Criteria.md | Reference | 10 | Exists |
| Sales_Stage_Definitions.md | Reference | 1, 7, 10 | Exists |
| MEDDPICC Discovery Workflow Prompt | Prompt | All AI steps | Exists |

## Tools and Connectors

| Tool / Connector | Purpose | Used By Steps | Status |
|-----------------|---------|---------------|--------|
| Web Search | Company research, legislative drivers, financial filings | 3 | Available (Claude Project) |
| LinkedIn | Stakeholder profiles, team mapping, mutual connections | 3 | Manual access |
| SEC EDGAR / Financial Sources | Public filings, investor statements | 3 | Manual / web search |
| Email Client | Send confirmation and follow-up emails | 2, 9 | External |
| Video Conferencing + Recording | Call execution | 7 | External |

## Recommended Implementation Order
1. Context files (Qualification Framework, Discovery Questions, Scoring Criteria, Sales Stage Definitions)
2. Workflow prompt covering Steps 1 and 3 (pre-call)
3. Briefing doc generation (Step 5)
4. Follow-up and mutual action plan generation (Step 8)
5. MEDDPICC scoring logic (Step 10)
6. Full prompt integration with all 11 steps

## Where to Run
**Platform:** Claude Project (web UI)
**GitHub:** N/A (Claude Project — context files stored in MEDDPICC_Discovery repo for version control)
**Entry point:** Start a new conversation in the MEDDPICC Discovery Workflow Claude Project
