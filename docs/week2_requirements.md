# A0: Project Framing & Application Scope Confirmation

## 1. Problem Evidence

Evidence 1: The Sunway Berhad 2025 Sustainability Report is 223 pages long, and Sunway's 2025 reporting is aligned with the IFRS S1 and S2 standards, so users must navigate large, standards-structured documents to find specific figures.

Evidence 2: S P Setia's Integrated Report 2025 spreads financial, operational and sustainability information across one report, and its chairman's message notes the inclusion of an inaugural ISSB (International Sustainabilty Standard Board) statement within the sustainability disclosures. Answering one question can require combining financial highlights with sustainability sections.

## 2. Exisiting approaches 
- ChatReport, an LLM-based system that analyses corporate sustainability reports.
- Report directory websites 

## 3. Project/Engineering Gap
- Automated or manual process for the existing approaches but it is not transparent.
- May gives a inaccurate answer ,cited to the source page and safe from invented figures due to Malaysian developers'reports from language question.

## 4. Project Objectives
O1: To design a document-grounded AI question-answering assistant based on publicly available annual, integrated and sustainability reports of Malaysian property developers.
O2: To develop the assistant with retrieval, source citation, and guardrails (e.g. refusing investment advice and flagging low-confidence answers).
O3: To evaluate the assistant in terms of answer accuracy ,verification, latency, and safety.

## 5. Intended Users
- Students
- Junior Analyst
- Environment,Social, and Governance Researcher

## 6. Supported Tasks
- Business performance
- Business financial market
- Marketing business initiatives

## 7. Information
- Business ROI
- Market trends
- Company's net-zero target

## 8. Operating Context
- Who uses it: Students, junior analysts and ESG researchers.
- How they use it: They type a question in a chat box and get an answer with the report name and page number.

## 9. Important Constraints
- Unrelated information given 
- May difficult to access the data due to company's policy

## 10. Explicit Out-of-Scope Tasks
- Company's asset
- Business bank account

## 11. Evaluation Focus
- Model confidence compared to actual statement
- Hallucination test