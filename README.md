# My Firma Assistant

> An AI question-answering assistant that answers questions about Malaysian property developers' annual, integrated and sustainability reports, with citations, for students, junior analysts and ESG researchers.

## Problem Statement
Malaysian property developers publish long annual, integrated and sustainability reports that mix narrative, targets and data tables. Students, junior analysts and Environment, Social and Governance (ESG) researchers must read and compare several reports manually to answer simple questions such as "What was the company's sales figure?" or "What is its net-zero target?". AI engineering makes it possible to build a document-grounded Q&A assistant that retrieves and cites the exact passage or table behind each answer, which keyword search cannot do across long, multi-document reports.

## Evidence of the Problem
- The Sunway Berhad 2025 Sustainability Report is 223 pages long and is aligned with the IFRS S1 and S2 standards, so users must navigate large, standards-structured documents to find specific figures. Source: [sustainabilityreports.com](https://www.sustainabilityreports.com/sunway/2025/sustainability-report)
- S P Setia's Integrated Report 2025 spreads financial, operational and sustainability information across one report, and includes an inaugural International Sustainability Standards Board (ISSB) statement within its sustainability disclosures, so one question can require combining several sections. Source: [S P Setia Integrated Report 2025](https://spsetia.com/wp-content/uploads/2026/03/Message_from_Our_Chairman.pdf)

## Initial Related Work / Existing Approaches
- Manual reading of company annual and sustainability reports (PDF) — authoritative, but time-consuming; comparing figures across companies and years requires reading several long documents by hand. Source: [Sunway Sustainability Report 2024](https://sustainability.sunway.com.my/Interactive-PDF/Sunway-Sustainability-Report-2024.pdf)
- Sustainability-report directory websites with AI-extracted ESG data — the site labels its AI-extracted data as experimental and possibly inaccurate, detailed data requires signing in, and answers are not conversational or traceable to exact passages. Source: [sustainabilityreports.com](https://www.sustainabilityreports.com/s-p-setia/2025/esg-report)
- ChatReport, an LLM-based system that analyses corporate sustainability reports — not built for Malaysian property developers' reports. Source: Ni, J., et al. (2023). *ChatReport: Democratizing Sustainability Disclosure Analysis through LLM-based Tools.* EMNLP 2023. [arXiv:2307.15770](https://arxiv.org/abs/2307.15770)

## Engineering Gap / Limitation
Existing manual and automated approaches are either slow or not transparent, and may give inaccurate answers that are not cited to the source page or protected against invented figures. There is no easy way to ask questions across Malaysian developers' reports and get verifiable, cited answers.

## Project Objectives
- O1: To design a document-grounded AI question-answering assistant based on publicly available annual, integrated and sustainability reports of Malaysian property developers.
- O2: To develop the assistant with retrieval, source citation, and guardrails (e.g. refusing investment advice and flagging low-confidence answers).
- O3: To evaluate the assistant in terms of answer accuracy, verification, latency, and safety.

## Target Users
Property and finance students, junior analysts, and ESG/sustainability researchers who need quick, verifiable answers from developers' published reports.

## Data Sources
- S P Setia Berhad Integrated Report 2025 — https://spsetia.com/wp-content/uploads/2026/03/Our_Investment_Case.pdf
- Sunway Berhad Sustainability Report 2024 — https://sustainability.sunway.com.my/Interactive-PDF/Sunway-Sustainability-Report-2024.pdf
- S P Setia Sustainability Financing Framework (April 2025) — https://spsetia.com/SPSetia/media/assets/Document/SPSetia.com/sustainability/S-P-Setia-Sustainability-Financing-Framework.pdf

## Weekly Progress
| Week | Focus | Deliverable | Status |
|------|-------|-------------|--------|
| W1 | System map + project scope | README + docs | System Map only Ongoing |
