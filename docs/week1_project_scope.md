# Week 1 Project Scope

## Project Name
My Firma Assistant

## Domain
Real Estate / Corporate Sustainability and Annual Report Analysis (Malaysian property developers)

## Problem Statement
Malaysian property developers publish long annual, integrated and sustainability reports that mix narrative, targets and data tables. Students, junior analysts and Environment,Social and Governance researchers must read and compare several reports manually to answer simple questions such as "What was the company's sales figure?" or "What is its net-zero target?". 

With AI technologies,a document-facts Q&A assistant that retrieves and cites the exact passage or table behind each answer, which keyword search cannot do across long, multi-document reports is able to developes.

## Evidence of the Problem
Evidence 1: The Sunway Berhad 2025 Sustainability Report is 223 pages long, and Sunway's 2025 reporting is aligned with the IFRS S1 and S2 standards, so users must navigate large, standards-structured documents to find specific figures.

Evidence 2: S P Setia's Integrated Report 2025 spreads financial, operational and sustainability information across one report, and its chairman's message notes the inclusion of an inaugural ISSB (International Sustainabilty Standard Board) statement within the sustainability disclosures. Answering one question can require combining financial highlights with sustainability sections.

## Initial Related Work (at least 3)

Study / solution 1: Manual reading of company annual and sustainability reports (PDF, interactive PDF).
Key limitation: Authoritative, but time-consuming; comparing figures across companies and years requires reading several long documents by hand.

Study / solution 2: Sustainability-report directory websites that aggregate reports and offer AI-extracted Environement,Social and Governance data.
Key limitation: The site labels its AI-extracted ESG data as experimental and possibly inaccurate, and detailed data requires signing in; answers are not conversational or traceable to exact passages.

Study / solution 3: ChatReport, an LLM-based system that analyses corporate sustainability reports.
Key limitation: Not built for Malaysian property developers’ reports

## Engineering Gap / Limitation
Gap / Limitation: - Automated or manual process for the existing approaches but it is not transparent.
                  - May gives a inaccurate answer ,cited to the source page and safe from invented figures due to Malaysian developers'reports from language question.

## Initial Project Objectives (2-3)
O1: To design a document-grounded AI question-answering assistant based on publicly available annual, integrated and sustainability reports of Malaysian property developers.
O2: To develop the assistant with retrieval, source citation, and guardrails (e.g. refusing investment advice and flagging low-confidence answers).
O3: To evaluate the assistant in terms of answer accuracy ,verification, latency, and safety.

## Target Users
Property and finance students, junior analysts, and Environment, Social and Governance/sustainability researchers who need quick, verifiable answers from developers' published reports.

## Data Sources (at least 2)
Source 1: S P Setia Berhad Integrated Report 2025 — URL: https://spsetia.com/wp-content/uploads/2026/03/Our_Investment_Case.pdf 
Source 2: Sunway Berhad Sustainability Report 2024 — URL: https://sustainability.sunway.com.my/Interactive-PDF/Sunway-Sustainability-Report-2024.pdf
Source 3: S P Setia Sustainability Financing Framework (April 2025) — URL: https://spsetia.com/SPSetia/media/assets/Document/SPSetia.com/sustainability/S-P-Setia-Sustainability-Financing-Framework.pdf

## Similar to EduAdvisor
Both are document-grounded Q&A assistants using retrieval over public PDF documents, with guardrails and evaluation of answer quality and groundedness.

## Different from EduAdvisor
PropReport Assistant works over long corporate reports that contain many tables and figures, so it must extract and compare numbers across companies and years, not only answer policy or course questions. Its users are analysts and researchers rather than students seeking academic advice, and its main safety concern is financial misuse rather than student wellbeing.

## Responsible AI Risks (at least 2)
Risk 1 — Hallucination / numeric errors: The model invents or misreads a figure - user relies on incorrect company data.
Risk 2 — Investment advice misuse: Users treat answers as recommendations on which company to invest in - the system must only report what documents say and refuse advice.
Risk 3 — Coverage bias: Only a few developers' reports are included, so comparisons may be incomplete or favour well-documented companies - clearly state which companies and years are covered.
