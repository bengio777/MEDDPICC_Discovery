# Notion Registration Queue

These items need to be registered in the AI Assets database (Data Source ID: `2d5edcfd-b924-80cf-a0a0-000ba0164e40`) when the Notion MCP connection is available.

## SOP — Paste to Workflow Page

**Notion Page:** https://www.notion.so/304fb3a7cad4813e8dd7c9dfd2c19c02
**Action:** Paste the contents of `outputs/meddpicc-discovery-prep-call-and-follow-up-sop.md` into the page body.

## AI Building Blocks to Register

### 1. MEDDPICC Discovery Workflow Prompt
| Property | Value |
|----------|-------|
| Name | MEDDPICC Discovery Workflow Prompt |
| Description | Baseline Workflow Prompt for the MEDDPICC Discovery Prep, Call, and Follow-up workflow. Self-contained prompt that orchestrates 6 steps: agenda email, stakeholder research, briefing doc, discovery call support, post-call follow-up, and MEDDPICC scoring. Designed to run in a Claude Project with 4 pre-loaded context files. |
| Asset Type | Prompt |
| Platform | Claude |
| Quick Start Prompt | I have a discovery call scheduled with [name], [title] at [company] on [date]. Here are the details: [meeting context]. Run the MEDDPICC Discovery Workflow starting from Step 1. |

### 2. MEDDPICC Scoring Criteria
| Property | Value |
|----------|-------|
| Name | MEDDPICC Scoring Criteria |
| Description | Four-level rubric (Strong/Partial/Gap/Unknown) for scoring MEDDPICC elements with element-specific criteria, example evidence at each rating level, scoring discipline principles, and stage gate minimums for deal advancement. Reusable across discovery, deal review, and pipeline audit workflows. |
| Asset Type | Context MD |
| Platform | Claude |
| Quick Start Prompt | — |

### 3. MEDDPICC Discovery Questions
| Property | Value |
|----------|-------|
| Name | MEDDPICC Discovery Questions |
| Description | MEDDPICC-aligned question bank with 32 questions organized by element. Includes TED follow-up framework (Tell/Explain/Describe progressive deepening), cost-of-inaction quantification with ALE framework, competitor bias detection questions, and mutual commitment questions. Reusable across any discovery or qualification workflow. |
| Asset Type | Context MD |
| Platform | Claude |
| Quick Start Prompt | — |

### 4. Sales Stage Definitions
| Property | Value |
|----------|-------|
| Name | Sales Stage Definitions |
| Description | CRM stage model defining 6 stages from Prospecting/Research through Closed Won/Lost. Each stage includes entry/exit criteria, key activities, and progression rules. Ties MEDDPICC scoring to stage gate transitions. Foundational context for any sales workflow. |
| Asset Type | Context MD |
| Platform | Claude |
| Quick Start Prompt | — |

### 5. MEDDPICC Qualification Framework
| Property | Value |
|----------|-------|
| Name | MEDDPICC Qualification Framework |
| Description | Reference definition of the MEDDPICC sales qualification methodology. Defines all 8 elements (Metrics, Economic Buyer, Decision Criteria, Decision Process, Paper Process, Identified Pain, Champion, Competition) with how the framework works for both buyers and sellers. |
| Asset Type | Context MD |
| Platform | Claude |
| Quick Start Prompt | — |
