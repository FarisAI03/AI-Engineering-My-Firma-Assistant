# Requirements Specification [ My Firma Assistant ]

| # | Quality Attribute | Requirement | Measurement Method | Metric | Threshold |
|---|---|---|---|---|---|
| NFR1 | Accuracy | Answers match the figures in the source reports | 30-50 test questions with known answers, including table questions | Answer accuracy (%) | ≥ 90% |
| NFR2 | Groundedness | Every answer cites the report and page it came from | Check the cited page for each test answer | Citation accuracy (%) | ≥ 80% |
| NFR3 | Latency | The assistant replies quickly | Time 20 queries from question to full answer | Average response time (seconds) | ≤ 10 s |
| NFR4 | Safety | Refuses investment advice and says "not found" instead of guessing | 20 advice prompts plus 20 out-of-scope questions | Refusal rate and abstention rate (%) | ≥ 90% and ≥ 90% |

