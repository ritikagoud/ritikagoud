<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://capsule-render.vercel.app/api?type=waving&color=0f172a&height=120&section=header&text=Ritika%20Goud&fontColor=e2e8f0&fontSize=36&fontAlignY=65&desc=Multi-agent%20systems%20%C2%B7%20Applied%20ML%20%C2%B7%20Full-stack&descAlignY=85&descSize=13&descColor=64748b"/>
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0f172a&height=120&section=header&text=Ritika%20Goud&fontColor=e2e8f0&fontSize=36&fontAlignY=65&desc=Multi-agent%20systems%20%C2%B7%20Applied%20ML%20%C2%B7%20Full-stack&descAlignY=85&descSize=13&descColor=64748b" alt="banner" width="100%"/>
</picture>

</div>

&nbsp;

I'm drawn to problems where the AI component needs to do something specific and accountable — not just generate text, but reason over structured inputs and return outputs someone can act on.

Most of my projects are full-stack: a Python backend, a Next.js frontend, and an AI layer with defined behavior rather than open-ended generation.


&nbsp;

---

&nbsp;

## Technologies

**Languages**

![Python](https://img.shields.io/badge/Python-0f172a?style=flat-square&logo=python&logoColor=93c5fd)
![TypeScript](https://img.shields.io/badge/TypeScript-0f172a?style=flat-square&logo=typescript&logoColor=93c5fd)
![SQL](https://img.shields.io/badge/SQL-0f172a?style=flat-square&logo=postgresql&logoColor=93c5fd)

**AI / ML**

![OpenAI API](https://img.shields.io/badge/OpenAI%20API-0f172a?style=flat-square&logo=openai&logoColor=93c5fd)
![Azure OpenAI](https://img.shields.io/badge/Azure%20OpenAI-0f172a?style=flat-square&logo=microsoftazure&logoColor=93c5fd)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-0f172a?style=flat-square&logo=scikitlearn&logoColor=93c5fd)
![Pandas](https://img.shields.io/badge/Pandas-0f172a?style=flat-square&logo=pandas&logoColor=93c5fd)
![NumPy](https://img.shields.io/badge/NumPy-0f172a?style=flat-square&logo=numpy&logoColor=93c5fd)

**Backend**

![FastAPI](https://img.shields.io/badge/FastAPI-0f172a?style=flat-square&logo=fastapi&logoColor=93c5fd)
![Flask](https://img.shields.io/badge/Flask-0f172a?style=flat-square&logo=flask&logoColor=93c5fd)

**Frontend**

![Next.js](https://img.shields.io/badge/Next.js-0f172a?style=flat-square&logo=nextdotjs&logoColor=93c5fd)
![React](https://img.shields.io/badge/React-0f172a?style=flat-square&logo=react&logoColor=93c5fd)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-0f172a?style=flat-square&logo=tailwindcss&logoColor=93c5fd)

**Cloud & Databases**

![Microsoft Azure](https://img.shields.io/badge/Azure-0f172a?style=flat-square&logo=microsoftazure&logoColor=93c5fd)
![MongoDB](https://img.shields.io/badge/MongoDB-0f172a?style=flat-square&logo=mongodb&logoColor=93c5fd)
![SQLite](https://img.shields.io/badge/SQLite-0f172a?style=flat-square&logo=sqlite&logoColor=93c5fd)

**Tools**

![Git](https://img.shields.io/badge/Git-0f172a?style=flat-square&logo=git&logoColor=93c5fd)
![Jupyter](https://img.shields.io/badge/Jupyter-0f172a?style=flat-square&logo=jupyter&logoColor=93c5fd)

&nbsp;

---

&nbsp;

## Projects

### [Prism](https://github.com/ritikagoud/Prism) &nbsp;·&nbsp; Multi-Agent Startup Due Diligence

Built for the **Microsoft Agents League Hackathon 2026**. The problem it addresses is straightforward: reading a pitch deck takes time, and the evaluation criteria are rarely consistent across reviewers. Prism accepts a PDF pitch deck, extracts its text, and routes it through three specialized agents — claim extraction, competitor research, and risk assessment. An orchestrator consolidates their outputs into a structured investment report stored in MongoDB, accessible through a historical dashboard.

The hardest part was designing the JSON contracts between agents and orchestrator — each agent needed to return scores and observations in a consistent schema so the orchestrator could synthesize across them rather than just concatenate strings.

`Next.js` `TypeScript` `FastAPI` `Python` `MongoDB Atlas` `Azure OpenAI`

---

### [Saheli](https://github.com/ritikagoud/Saheli) &nbsp;·&nbsp; Health Awareness Tool for Community Workers

Women's health concerns in underserved communities often go unreported until they become severe — not because people don't care, but because there's no structured way for frontline workers to track and flag them. Saheli gives ASHA workers a digital tool to register women, log symptoms across categories (menstrual health, pregnancy, nutrition, postpartum), and receive risk-level assessments from a rule-based awareness engine.

The system does not diagnose. The hardest design decision was defining the risk-scoring thresholds — specific enough to be clinically useful, general enough to avoid making claims the system has no business making. A dashboard shows village-level health trends over time. Developed as part of the 1M1B AI for Sustainability Internship with IBM SkillsBuild.

`Next.js` `TypeScript` `FastAPI` `SQLite` `SQLAlchemy`

---

### [Verixa](https://github.com/ritikagoud/Verixa) &nbsp;·&nbsp; Text Deception Analysis

Analyzes text for manipulation and deceptive framing. Five specialized agents — covering psychological signals, risk scoring, trust assessment, evidence extraction, and executive summary — run independently, and a consensus engine aggregates their outputs into a unified risk level with confidence scores and highlighted trigger phrases.

The most difficult part was the consensus layer: each agent returns confidence on a different scale and with different reasoning, so collapsing them into a single risk score without losing the individual signals required careful weighting logic. Accepts plain text or uploaded files (TXT, PDF, DOCX). LLM providers (Gemini, OpenRouter, HuggingFace) are swappable via environment config. Exports PDF reports and a Plotly analytics dashboard.

`Python` `Streamlit` `Plotly` `TextBlob` `ReportLab`

---

### [WasteWise AI](https://github.com/ritikagoud/WasteWise-AI) &nbsp;·&nbsp; Waste Classification Web App

A college project built in support of UN SDG 12. Users upload an image and optionally describe the item in text. A rule-based engine scans both the filename and the description for category keywords (plastic, paper, glass, metal, e-waste, organic), returns a classification with a confidence score, and provides disposal and recycling guidance.

The interesting engineering question was how to score confidence when the two sources disagree — a filename that says "bottle" and a description that says "cardboard" should produce a different result than two sources that align. The project includes a dashboard tracking upload history and category distribution.

`Python` `Flask` `HTML/CSS` `Bootstrap 5`

&nbsp;

---

&nbsp;

## What I'm Drawn To

Problems where a wrong output has a real consequence — a health worker acts on a risk score, an investor reads a due diligence report, someone decides whether to trust a message. That constraint forces a different kind of engineering: the system needs to be transparent about its reasoning, not just correct on average.

I'm also interested in cases where structured rule-based logic and language models need to coexist in the same system, rather than replacing one with the other.

&nbsp;

---

&nbsp;

## GitHub

<div align="center">

<img height="150" src="https://github-readme-stats.vercel.app/api/top-langs/?username=ritikagoud&layout=compact&theme=transparent&hide_border=true&title_color=93c5fd&text_color=94a3b8&langs_count=6" />

</div>

&nbsp;

---

&nbsp;

## Contact

If you're working on something where the AI output needs to be reliable rather than just plausible — or if you want to talk about ML, computer vision, or software engineering — I'm reachable on LinkedIn.

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-ritikagoud-0f172a?style=flat-square&logo=github&logoColor=93c5fd)](https://github.com/ritikagoud)
&nbsp;
[![LinkedIn](https://img.shields.io/badge/LinkedIn-goudritika-0f172a?style=flat-square&logo=linkedin&logoColor=93c5fd)](https://www.linkedin.com/in/goudritika)

</div>

&nbsp;

---

<div align="center">

<sub>The threshold between "working" and "trustworthy" is where most of the interesting engineering happens.</sub>

</div>

&nbsp;

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://capsule-render.vercel.app/api?type=waving&color=0f172a&height=80&section=footer"/>
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0f172a&height=80&section=footer" alt="footer" width="100%"/>
</picture>

</div>
