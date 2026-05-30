<div align="center">

# Sai Rithvik Reddy

**AI & Automation Engineer · Building systems that actually ship**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sai-rithvik-reddy-kanyagari-62252b23b/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:rithvikreddy524@gmail.com)
[![SAP Build Developer](https://img.shields.io/badge/SAP_Build_Developer-Certified-0FAAFF?style=flat&logo=sap&logoColor=white)](https://www.credly.com/badges/41ff28ee-7523-4f0c-962c-726f4446ef7e)
[![SAP GenAI Developer](https://img.shields.io/badge/SAP_GenAI_Developer-Certified-0FAAFF?style=flat&logo=sap&logoColor=white)](https://www.credly.com/badges/95cacd9d-b471-4d67-add5-ba35288f3b0a)

</div>

---

I'm an AI & Automation Engineer based in Bengaluru, currently at **SAP Concur** where I design and own production LLM + RPA systems that handle thousands of enterprise cases every week. I care about one thing: automation that actually works at scale, not demos.

My stack lives in the LangChain/LangGraph/RAG ecosystem, deployed on SAP BTP with CI/CD through Honeycomb. Before this, I built across Python, TypeScript, and Go — from desktop GUI apps to multi-agent SQL interfaces to full-stack web platforms.

---

## Production Systems @ SAP Concur

These run in prod. Not side projects.

**LLM + IRPA Triage Pipeline**
Parses case subject, description, and business rules to route 1,000+ cases/week to the right consultant queue automatically — replacing a fully manual process.

**E2E Concur Implementation Agent**
Multi-agent pipeline: an analysis agent reasons through workbook configs and dependency ordering, a planning agent generates a JSON task plan, a critic agent flags gaps, and a chat agent handles human-in-the-loop review before a Playwright-based execution layer configures SAP Concur entities end-to-end.

**RAG Case Assistant** *(LangChain + SAP HANA)*
Auto-generates the first private comment per case — issue summary, next steps, client questions — the moment a case is created.

**Triage Validation Engine**
LLM comparison of bot-assigned vs consultant-modified inventory groups. Flags triage errors automatically, replacing 50–60 manual reviews per week.

**Risk Analysis System** *(Pandas + Salesforce signals)*
Scores 3,000+ enterprise accounts across Safe / Should Monitor / Critical tiers using a rule-based weighted engine built on case spikes, escalations, and SLA signals.

**Sentiment Analysis Layer** *(Teams integration)*
Monitors high-risk account comments and auto-pings the assigned consultant on Teams when client tone turns negative or neutral.

---

## Featured Projects

### 🏥 [Medical First-Aid AI Assistant](https://github.com/Rithvik119am/medical_ai_assistant)
> Python · LangGraph · ChromaDB · MedEmbed · PySide6 · Gemini

Desktop app with a hybrid RAG pipeline — local ChromaDB vector store (medical-specialized MedEmbed embeddings) + live Google search — fed into a LangGraph ReAct agent. Every response follows a strict safety template: Triage → Condition → Steps → Medicines → Citations. Severe symptoms trigger emergency escalation. QThread workers keep the GUI fully responsive during ingestion.

---

### 🧠 [Data Bridge — Natural Language SQL](https://github.com/Rithvik119am/data-bridge)
> Python · LangChain · ChromaDB · PySide6 · PostgreSQL · MySQL · SQLite · Oracle · MSSQL

Multi-agent system that turns plain English into SQL across five database types. A question enhancer agent refines the query and suggests visualizations; a SQL agent generates and self-corrects queries (up to 5 retry iterations); a response agent builds the final answer; a visualization agent generates Plotly charts. Results download as `.xlsx`. Document uploads enrich ChromaDB context. Credentials encrypted at rest.

---

### 📊 [VidhaRith — AI Quiz Platform for Educators](https://github.com/Rithvik119am/VidhaRith)
> Next.js 14 · TypeScript · Convex · Clerk · Google Generative AI · Tailwind CSS · Recharts

Live at [vidharith.vercel.app](https://vidharith.vercel.app). Educators upload teaching materials; the platform auto-generates quiz questions via Gemini, runs real-time analytics as students respond, and surfaces per-student and class-wide performance breakdowns. Built on Convex for real-time data sync, Clerk for auth, and Shadcn/Radix UI for components.

---

### 🎨 [Palattic](https://www.palattic.com)
Desktop art portfolio manager for artists. Built with PySide6. Currently in closed beta.

---

## Tech Stack

**AI / ML**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B35?style=flat)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat&logo=huggingface&logoColor=black)
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=flat&logo=google&logoColor=white)

**Backend & Data**

![Flask](https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![SAP HANA](https://img.shields.io/badge/SAP_HANA-0FAAFF?style=flat&logo=sap&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat&logo=sqlite&logoColor=white)

**Frontend & Full-Stack**

![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![PySide6](https://img.shields.io/badge/PySide6-41CD52?style=flat&logo=qt&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat&logo=tailwindcss&logoColor=white)

**Infrastructure & Tools**

![SAP BTP](https://img.shields.io/badge/SAP_BTP-0FAAFF?style=flat&logo=sap&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat&logo=playwright&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white)

---

## GitHub Stats

<div align="center">

![Rithvik's GitHub Stats](https://github-readme-stats.vercel.app/api?username=Rithvik119am&show_icons=true&theme=dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9&icon_color=58a6ff)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Rithvik119am&layout=compact&theme=dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9)

</div>

---

<div align="center">

**BTech CSE (AI & DS) · Vardhaman College of Engineering · CGPA 8.28**

*Open to AI/automation engineering roles · rithvikreddy524@gmail.com*

</div>
