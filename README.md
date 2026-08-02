<div align="center">

# Sai Rithvik Reddy

**AI & Automation Engineer · Building production AI systems that actually ship**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sai-rithvik-reddy-kanyagari-62252b23b/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:rithvikreddy524@gmail.com)
[![SAP Build Developer](https://img.shields.io/badge/SAP_Build_Developer-Certified-0FAAFF?style=flat&logo=sap&logoColor=white)](https://www.credly.com/badges/41ff28ee-7523-4f0c-962c-726f4446ef7e)
[![SAP GenAI Developer](https://img.shields.io/badge/SAP_GenAI_Developer-Certified-0FAAFF?style=flat&logo=sap&logoColor=white)](https://www.credly.com/badges/95cacd9d-b471-4d67-add5-ba35288f3b0a)

</div>

---

I'm an AI & Automation Engineer based in Bengaluru, currently at **SAP Concur**, where I design and build production LLM, RAG, and automation systems for enterprise workflows.

My work spans **agentic AI, RAG, LLM evaluation, workflow orchestration, browser automation, and SAP BTP architecture** — from systems routing 1,000+ support cases every week to AI-assisted configuration transformation and risk analysis across 3,000+ enterprise accounts.

I work primarily with **Python, LangChain, LangGraph, FastAPI, SAP HANA Cloud, SAP AI Core / Generative AI Hub, Playwright, and IRPA**, with a focus on building AI systems that are grounded, observable, and reliable enough for real workflows.

Outside enterprise systems, I've built desktop applications, multi-agent SQL interfaces, RAG assistants, and full-stack AI platforms using Python, TypeScript, and Go.

---

## Production Systems @ SAP Concur

### ⚡ PANACHE — SAP Concur Configuration Transformation Platform

AI-assisted enterprise platform for transforming SAP Concur configurations through a multi-stage workflow spanning:

**Analysis → Indexing → Research → Clarification → Planning → Repair → Execution → Summarization**

The system combines a **SAPUI5/Fiori frontend, FastAPI services, SAP HANA Cloud, Event Mesh, BTP Object Store, SAP AI Core / Generative AI Hub, and Playwright-based execution**.

A secure local runner handles controlled browser execution while keeping authentication state on the consultant's machine, with runner registration, heartbeats, leases, command validation, screenshots/observations, takeover, and cancellation handling.

The platform uses shared **Pydantic/OpenAPI contracts, durable workflow state, idempotent operations, SSE event streaming, access-control boundaries, contract testing, and CI/CD validation**.

---

### 🔀 LLM + IRPA Case Routing

Production routing system processing **1,000+ SAP Concur support cases per week**.

The LLM classifies incoming cases and feeds the result into an IRPA-driven assignment workflow that considers:

- Consultant expertise and case domain
- Current consultant workload
- Per-consultant daily assignment limits
- Region-specific routing and automation rules
- Returned/previously triaged cases
- Retry safeguards and exception handling
- Region-specific automated notifications

For example, Travel cases are only assigned to consultants qualified to handle Travel while the assignment layer continuously tracks consultant capacity before allocating additional cases.

#### Evaluation & Continuous Improvement

A weekly evaluation workflow analyzes Salesforce cases where the assigned **Inventory Group or Queue changed after automated routing**.

These cases are reviewed to distinguish between:

1. genuine LLM classification errors, and
2. legitimate routing changes caused by new information or changing case requirements.

Confirmed classification errors are fed back into **prompt and classification-process improvements**, creating a continuous evaluation loop around the production routing system.

---

### 🧠 RAG-Based First Comment Agent

Production RAG assistant that generates the initial private comment for incoming support cases.

Built using **LangChain, LangGraph, and SAP HANA vector retrieval**, the system retrieves relevant support knowledge and generates grounded outputs containing:

- Issue summary
- Recommended next steps
- Outstanding customer questions

The goal is to give consultants an immediately actionable starting point while grounding the generated response in retrieved enterprise knowledge.

---

### 📊 Enterprise Risk Analysis System

Automated risk-analysis workflow covering **3,000+ enterprise accounts**.

Salesforce signals — including case activity, escalations, and other account indicators — are processed through a weighted scoring workflow, aggregated, and persisted in **SAP HANA** to classify accounts into:

**Safe · Monitor · Critical**

Every week, consultants receive an actionable risk report showing their exposure to at-risk accounts and associated cases.

Reports are directly connected to operational workflows: consultants can open individual cases or navigate to an account's risk-analysis view to inspect escalation history and other relevant customer signals.

---

## Featured Personal Projects

### 🏥 [Medical First-Aid AI Assistant](https://github.com/Rithvik119am/medical_ai_assistant)

> Python · LangGraph · ChromaDB · MedEmbed · PySide6 · Gemini

Desktop application with a hybrid RAG pipeline combining a local ChromaDB vector store using medical-specialized MedEmbed embeddings with live Google search, orchestrated through a LangGraph ReAct agent.

Responses follow a structured safety-oriented format covering triage, condition information, next steps, medicines, and citations, while severe symptom patterns trigger emergency escalation. QThread workers keep the desktop UI responsive during ingestion and inference.

---

### 🧠 [Data Bridge: Natural Language SQL](https://github.com/Rithvik119am/data-bridge)

> Python · LangChain · ChromaDB · PySide6 · PostgreSQL · MySQL · SQLite · Oracle · MSSQL

Multi-agent system that translates natural-language questions into SQL across five database platforms.

A question-enhancement agent refines requests and proposes visualizations; a SQL agent generates and self-corrects queries through multiple retry iterations; a response agent synthesizes results; and a visualization agent generates Plotly charts.

Supports document-based ChromaDB context, Excel exports, and encrypted database credentials.

---

### 📊 [VidhaRith: AI Quiz Platform for Educators](https://github.com/Rithvik119am/VidhaRith)

> Next.js 14 · TypeScript · Convex · Clerk · Google Generative AI · Tailwind CSS · Recharts

Live at [vidharith.vercel.app](https://vidharith.vercel.app).

Full-stack platform where educators upload teaching materials and automatically generate quiz questions using Gemini.

Built with **Convex** for real-time synchronization and **Clerk** for authentication, with live student responses, class-wide analytics, and per-student performance breakdowns.

---

### 🎨 Palattic

Desktop art portfolio manager designed for visual artists.

Built as a lightweight desktop application for managing artworks, collections, artists, tags, materials, availability, and sales.

[Watch the demo on YouTube](https://www.youtube.com/watch?v=qNzpNYNSV_s)

---

## Tech Stack

**AI / LLM**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat)
![RAG](https://img.shields.io/badge/RAG-Vector_Retrieval-blue?style=flat)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat&logo=huggingface&logoColor=black)
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=flat&logo=google&logoColor=white)

**SAP / Cloud**

![SAP BTP](https://img.shields.io/badge/SAP_BTP-0FAAFF?style=flat&logo=sap&logoColor=white)
![SAP HANA](https://img.shields.io/badge/SAP_HANA_Cloud-0FAAFF?style=flat&logo=sap&logoColor=white)
![SAP AI Core](https://img.shields.io/badge/SAP_AI_Core-0FAAFF?style=flat&logo=sap&logoColor=white)
![Generative AI Hub](https://img.shields.io/badge/Generative_AI_Hub-0FAAFF?style=flat&logo=sap&logoColor=white)
![SAP Event Mesh](https://img.shields.io/badge/Event_Mesh-0FAAFF?style=flat&logo=sap&logoColor=white)

**Backend & Automation**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat&logo=pydantic&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat&logo=playwright&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)

**Frontend & Engineering**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)
![SAPUI5](https://img.shields.io/badge/SAPUI5-Fiori-0FAAFF?style=flat&logo=sap&logoColor=white)
![PySide6](https://img.shields.io/badge/PySide6-41CD52?style=flat&logo=qt&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)

---

<div align="center">

**BTech CSE (AI & DS) · Vardhaman College of Engineering · CGPA 8.15**

*Open to AI / LLM / Automation Engineering roles · rithvikreddy524@gmail.com*

</div>
