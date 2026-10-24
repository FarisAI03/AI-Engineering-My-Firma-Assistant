# Requirements Specification [ My Firma Assistant ]

| # | Responsible AI Risk | Requirement | Measurement Method | Metric | Threshold |
|---|---|---|---|---|---|
| RAI1 | Hallucination | The answer must matching the source report and include the citation it gets from | Do a small sample test for question with the actual facts | Numeric Accuracy and Citation accuracy | >= 80% for both accuracy |
| RAI2 | Recommendation misuse | Only guiding the user without instructs to do the suggestion completely | prompt question with the generic facts question to identify whether it does not refuse too much | Refusal advice prompting rate,false refusal on normal question | Refusal rate >= 90%,false refusal rate <= 5%> |
| RAI3 | Coverage bias | Honest in total years gap that the model can analyze | out of scope sample data | Accuracy gap between company | <= 10% |
