# Career & Skill-Gap Advisor Agent

An AI-powered multi-agent system built with IBM watsonx.ai, IBM Granite models, and LangFlow that gives tier-2/3 college students personalized, data-backed career guidance — closing the gap between overloaded placement cells and individualized counseling.

## Problem Statement
Students at tier-2/3 colleges often lack access to personalized career counseling. Skill requirements change fast, and generic advice from forums leads to mismatched career choices and skill gaps at hiring time. See `yourproblemstatement.pdf` for the full brief.

## Solution Overview
A multi-agent system that analyzes a student's resume/skills, identifies gaps against real job-role requirements (via RAG), recommends learning paths, and runs mock interviews with feedback.

### Agents
| Agent | Role |
|---|---|
| Skill Assessment Agent | Parses resume, identifies skill gaps against target roles |
| Career Path Agent | Recommends roles based on interests, background, aptitude |
| Learning Resource Agent | Retrieves and ranks courses/certifications via RAG |
| Interview Coach Agent | Runs mock interviews, gives structured feedback |

## Tech Stack
- **LangFlow** – Multi-agent workflow orchestration
- **IBM Granite** (`granite-4.0-8b-instruct`) – Reasoning, resume parsing, feedback generation
- **IBM watsonx.ai** – Model deployment, embeddings, governance
- **IBM Cloud** – Hosting and scaling infrastructure
- **Vector DB (FAISS/Chroma)** – RAG-based retrieval of job/skill data

## Repository Contents
- `app.json` — Exported LangFlow flow
- `yourproblemstatement.pdf` — Official problem statement
- `yourprojectpresentation.pptx` — Project submission deck
- `README.md` — This file

## How to Run
1. Install [LangFlow](https://github.com/langflow-ai/langflow): `pip install langflow`
2. Launch LangFlow: `langflow run`
3. Import `app.json` via the LangFlow UI (Flow → Import)
4. Configure your IBM watsonx.ai API credentials in the watsonx AI Agent node
5. Run the flow and interact via the Chat Input/Output nodes

## Future Scope
- Integration with job portals (LinkedIn API) for live postings
- Regional language and voice support for wider accessibility

## Submitted by
Lakshitha R
