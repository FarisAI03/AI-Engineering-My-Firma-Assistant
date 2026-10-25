# Design Decision

| Objective | Requirement | Evaluation Criterion | Architecture Element | Later Evidence |
|---|---|---|---|---|
| O1: Design a document-grounded assistant using public property developer reports | FR1, FR2, FR3 | Citation correctness (≥ 80%); answers use only the listed reports | AI application, AI capability, Report library | Architecture and flowchart diagrams; sample answers showing report name and page |
| O2: Develop the assistant with retrieval, citation and guardrails | FR4, NFR2, NFR4, RAI2, RAI3 | Retrieval hit rate @5 (≥ 80%); refusal rate on advice prompts (≥ 90%); correct "not found" rate (≥ 90%) | Report library (retrieval), Safety check, Coverage list | Retrieval test results; red-team and out-of-scope prompt results |
| O3: Evaluate answer accuracy, verification, latency and safety | NFR1, NFR3, RAI1, RAI3 | Answer accuracy (≥ 90%); table figure accuracy (≥ 85%); average response time (≤ 10 s); accuracy gap between companies (≤ 10 points) | Evaluation test set and logs, AI capability | Test question set in `evaluation/`; results report with scores against each threshold |