# MEDDPICC Discovery Prep, Call, and Follow-up

End-to-end workflow for an enterprise AE to research, prepare for, execute, and follow up on a discovery call with a senior stakeholder, using MEDDPICC to qualify the opportunity.

## What It Does

Produces a scored qualification baseline through 6 steps:

1. **Draft agenda and confirmation email** (AI)
2. **Deep stakeholder and organization research** — 5 parallel threads: LinkedIn, team mapping, legislative drivers, financial filings, company intel (AI)
3. **Build call briefing doc** — scannable format with rapport angles, stakeholder map, intelligence plays, MEDDPICC targeting (AI)
4. **Execute the discovery call** (Human)
5. **Generate post-call follow-up** — recap email + mutual action plan with reciprocal commitments (AI)
6. **Score the opportunity** — MEDDPICC scorecard with Strong/Partial/Gap/Unknown per element + stage gate assessment (AI)

## Platform

Claude Project with 4 pre-loaded context files. Designed to run as an augmented workflow — AI handles research, drafting, and scoring; human drives the call and all approval gates.

## Context Files

| File | Purpose |
|------|---------|
| `MEDDICC_Qualification_Framework.md` | Element definitions for M, E, D, D, P, I, C, C |
| `MEDDPICC_Discovery_Questions.md` | 32 questions organized by element with TED framework |
| `MEDDPICC_Scoring_Criteria.md` | Strong/Partial/Gap/Unknown rubric per element |
| `Sales_Stage_Definitions.md` | 6-stage CRM model with entry/exit criteria |

## Outputs

- Confirmation email with proposed agenda
- Research package (5 sections, confidence-flagged as Verified/Inferred/Gap)
- Call briefing doc (scannable format)
- Follow-up email with call recap (tone-calibrated)
- Mutual action plan with owners and deadlines
- MEDDPICC scorecard with gap analysis and deal recommendation

## Multi-Agent Architecture

Step 2 (Research) is designed as a multi-agent orchestration with 5 parallel research threads coordinated by a master orchestrator:

- Individual LinkedIn profile research
- Team mapping with product/competitor exposure flags
- Legislative/regulatory drivers by industry vertical
- Financial filing analysis (10-K, 8-K, investor statements)
- Company context and industry intelligence

All findings are confidence-flagged and synthesized in Step 3.

## Project Structure

```
MEDDPICC_Discovery/
├── Reference Files/
│   ├── MEDDICC_Qualification_Framework.md
│   ├── MEDDPICC_Discovery_Questions.md
│   ├── MEDDPICC_Scoring_Criteria.md
│   ├── Sales_Stage_Definitions.md
│   └── meddpicc-discovery-prep-call-and-follow-up-definition.md
├── outputs/
│   ├── meddpicc-discovery-prep-call-and-follow-up-prompt.md
│   ├── meddpicc-discovery-prep-call-and-follow-up-building-blocks.md
│   ├── meddpicc-discovery-prep-call-and-follow-up-sop.md
│   └── notion-registration-queue.md
└── README.md
```

## SOP

Full standard operating procedure: [workflow-definitions/meddpicc-discovery.md](https://github.com/bengio777/workflow-definitions)

## Status

Deployed

## Author

Ben Giordano
