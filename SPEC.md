# MEDDPICC Discovery Prep, Call, and Follow-up — Project Spec

**Project:** MEDDPICC Discovery

---

## Capabilities Demonstrated

### 1. End-to-end sales workflow from scheduling through qualification
**Met.** The workflow covers the complete discovery lifecycle: agenda email, deep research (5 parallel threads), call briefing doc, call execution support, post-call follow-up with mutual action plan, and MEDDPICC scoring with stage gate assessment. 11 steps from trigger to qualification decision.
**Evidence:** `WORKFLOW-DEFINITION.md` (Steps 1-11), `outputs/meddpicc-discovery-prep-call-and-follow-up-sop.md`

### 2. Multi-threaded research with confidence flagging
**Met.** Step 3 conducts research across 5 parallel threads (individual stakeholder, team mapping, legislative/regulatory, financial filings, company/industry context). Every finding is flagged as Verified (sourced), Inferred (reasonable conclusion), or Gap (unknown -- probe on call).
**Evidence:** `WORKFLOW-DEFINITION.md` (Step 3), `outputs/meddpicc-discovery-prep-call-and-follow-up-building-blocks.md` (Step 2 decomposition)

### 3. Prompt with 4 context files providing domain expertise
**Met.** The Claude Project loads 4 reference files that encode the full MEDDPICC framework: element definitions, 32 discovery questions organized by element with TED framework, scoring rubric (Strong/Partial/Gap/Unknown per element), and 6-stage CRM model with entry/exit criteria.
**Evidence:** `Reference Files/MEDDICC_Qualification_Framework.md`, `Reference Files/MEDDPICC_Discovery_Questions.md`, `Reference Files/MEDDPICC_Scoring_Criteria.md`, `Reference Files/Sales_Stage_Definitions.md`

### 4. Structured MEDDPICC scoring with stage gate assessment
**Met.** Step 10 maps call evidence to each MEDDPICC element using the scoring criteria. Each element receives a rating with supporting evidence and a recommended next action. Stage gate minimums are enforced: Identified Pain, Champion, and Economic Buyer must each be at least Partial to advance.
**Evidence:** `WORKFLOW-DEFINITION.md` (Step 10), `Reference Files/MEDDPICC_Scoring_Criteria.md`

### 5. Human-in-the-loop at every outbound and decision point
**Met.** 6 of 11 steps are human gates. No email is sent, no deal is advanced, and no qualification decision is made without AE review and approval. AI handles research, drafting, and scoring; human handles judgment and execution.
**Evidence:** `WORKFLOW-DEFINITION.md` (Steps 2, 4, 6, 7, 9, 11)

### 6. Tone-calibrated post-call follow-up
**Met.** Step 8 generates a follow-up email matched to the tone the AE specifies (formal / business casual / casual) based on how the call actually went. Sensitive information flagged by the AE is excluded. Mutual action plan lists reciprocal commitments with owners and deadlines.
**Evidence:** `WORKFLOW-DEFINITION.md` (Steps 8-9)

---

## Deliverables

| # | Deliverable | File | Status |
|---|-------------|------|--------|
| 1 | Qualification Framework | `Reference Files/MEDDICC_Qualification_Framework.md` | Complete |
| 2 | Discovery Questions (32 questions) | `Reference Files/MEDDPICC_Discovery_Questions.md` | Complete |
| 3 | Scoring Criteria | `Reference Files/MEDDPICC_Scoring_Criteria.md` | Complete |
| 4 | Sales Stage Definitions | `Reference Files/Sales_Stage_Definitions.md` | Complete |
| 5 | Workflow definition (SOP) | `WORKFLOW-DEFINITION.md` | Complete |
| 6 | Building blocks analysis | `outputs/meddpicc-discovery-prep-call-and-follow-up-building-blocks.md` | Complete |
| 7 | Workflow prompt | `outputs/meddpicc-discovery-prep-call-and-follow-up-prompt.md` | Complete |
| 8 | Process definition | `Reference Files/meddpicc-discovery-prep-call-and-follow-up-definition.md` | Complete |
| 9 | Building block spec | `BUILDING-BLOCK-SPEC.md` | Complete |
| 10 | Project spec | `SPEC.md` | Complete |
| 11 | README | `README.md` | Complete |

---

## Review Criteria

| Criterion | Status | Evidence |
|-----------|--------|----------|
| All 4 context files loaded in Claude Project | Pass | Files exist in `Reference Files/` directory |
| Workflow covers pre-call, call, and post-call phases | Pass | Steps 1-6 (pre-call), Step 7 (call), Steps 8-11 (post-call) |
| Research outputs are confidence-flagged | Pass | Verified/Inferred/Gap flagging specified in Step 3 |
| Briefing doc is designed for glanceable use during live calls | Pass | Bold titles, highlighted sub-bullets, 5 sections specified in Step 5 |
| MEDDPICC scoring includes evidence per rating | Pass | Strong requires quotes; Partial requires paraphrase; Gap/Unknown defined |
| Stage gate minimums are enforced | Pass | Pain, Champion, Economic Buyer must be at least Partial |
| Every AI output has a human review gate | Pass | Steps 2, 4, 6, 9, 11 are explicit review gates |
| SOP follows standard template | Pass | `WORKFLOW-DEFINITION.md` has all required sections |

---

## File Inventory

| File | Location | Purpose |
|------|----------|---------|
| `MEDDICC_Qualification_Framework.md` | `Reference Files/` | MEDDPICC element definitions (M, E, D, D, P, I, C, C) |
| `MEDDPICC_Discovery_Questions.md` | `Reference Files/` | 32 discovery questions organized by element with TED framework |
| `MEDDPICC_Scoring_Criteria.md` | `Reference Files/` | Strong/Partial/Gap/Unknown rubric per element |
| `Sales_Stage_Definitions.md` | `Reference Files/` | 6-stage CRM model with entry/exit criteria |
| `meddpicc-discovery-prep-call-and-follow-up-definition.md` | `Reference Files/` | Process definition document |
| `meddpicc-discovery-prep-call-and-follow-up-prompt.md` | `outputs/` | Generated workflow prompt for Claude Project |
| `meddpicc-discovery-prep-call-and-follow-up-building-blocks.md` | `outputs/` | Building block decomposition analysis |
| `meddpicc-discovery-prep-call-and-follow-up-sop.md` | `outputs/` | Generated SOP document |
| `notion-registration-queue.md` | `outputs/` | Notion asset registration queue |
| `WORKFLOW-DEFINITION.md` | `WORKFLOW-DEFINITION.md` | Standard operating procedure |
| `BUILDING-BLOCK-SPEC.md` | `BUILDING-BLOCK-SPEC.md` | AI building block specification |
| `SPEC.md` | `SPEC.md` | Project spec (this file) |
| `README.md` | `README.md` | Project overview and structure |
