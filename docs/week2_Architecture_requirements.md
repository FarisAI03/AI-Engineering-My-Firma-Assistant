# Architect Requirements

| Requirement ID | What does the requirement need? | Architecture Response |
|---|---|---|
| FR2 | Answer using only the listed reports | AI capability finds evidence from the Report library and answers only from it |
| FR3 | Show the report name and page with every answer | AI capability returns the source with the answer, and the AI application displays it in the response |
| FR4 | Refuse investment-advice requests | Safety check blocks advice questions, and the response returns a safe refusal |
| NFR1 | Answers match the figures in the reports (accuracy) | AI capability answers from the Report library, which keeps text and tables readable; checked with the Evaluation test set |
| NFR2 | Every answer cites its source (groundedness) | Report library keeps the report name and page for each passage, and AI capability includes them in the response |
| NFR4 | Refuse advice and avoid guessing (safety) | Safety check blocks advice; AI capability and Coverage list give "not found" for out-of-scope questions |
| RAI1 | Prevent hallucinated or misread figures | Report library holds tables in a readable form, and answers must quote that evidence |
| RAI2 | Prevent investment advice misuse | Safety check refuses buy, sell and "which to invest in" questions |
