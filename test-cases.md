# Test Cases — Home Credit LAP Qualification Agent

Use these as a checklist when testing the agent in Retell. Do not initiate a billed simulation or live call until you understand the cost and explicitly decide to proceed.

| ID | Scenario | Expected behaviour |
|---|---|---|
| TC-01 | Correct customer confirms identity | Explain preliminary offer and ask if it is a convenient time. |
| TC-02 | Wrong person answers | Do not disclose loan details; end politely. |
| TC-03 | Customer says property is agricultural | Disqualify immediately and end the call. |
| TC-04 | Residential property, sole ownership | Accept ownership and continue collecting missing fields. |
| TC-05 | Joint ownership | Accept and continue. |
| TC-06 | Original documents are unavailable / only copies exist | Disqualify immediately and end the call. |
| TC-07 | Requested amount is ₹50 lakh | Record amount and continue. |
| TC-08 | Requested amount is ₹90 lakh | Offer the ₹75 lakh maximum and ask whether the customer wants to proceed at that amount. |
| TC-09 | Customer declines ₹75 lakh and insists on more | Explain this offer is capped at ₹75 lakh; end without implying a higher amount is available. |
| TC-10 | Salaried, income received in bank account | Accept and continue. |
| TC-11 | Self-employed, income received in bank account | Accept and continue. |
| TC-12 | Income received only in cash | Disqualify immediately and end the call. |
| TC-13 | Customer does not know market value | Ask for an approximate estimate; never invent a value. |
| TC-14 | Tenure is 2 years | Disqualify immediately and end the call. |
| TC-15 | Tenure is 3 or 15 years | Accept boundary values and continue. |
| TC-16 | Tenure is 16 years | Disqualify immediately and end the call. |
| TC-17 | Customer wants EMI reduction / balance transfer / refinance | Stop fresh-loan qualification, explain specialist follow-up, and end the call. |
| TC-18 | Customer is busy | Ask for preferred callback time; do not claim a callback has been scheduled. |
| TC-19 | Customer gives multiple fields in one answer | Save all clear answers and do not ask those fields again. |
| TC-20 | Customer provides fields out of order | Extract answers, apply disqualifying rules immediately, and ask only for unanswered fields. |
| TC-21 | All seven fields answered and all rules passed | Give the approved closing statement for senior-expert follow-up; do not guarantee approval or rate. |
| TC-22 | Customer asks for guaranteed approval or exact rate | Explain that final assessment and rate are determined by the senior expert. |

## Acceptance checklist
- [ ] No already-answered field is asked again.
- [ ] Disqualification stops further eligibility questions.
- [ ] No unsupported approval, rate, valuation, or callback promises.
- [ ] Loan-transfer cases do not continue the new-loan checklist.
- [ ] Qualified closing happens only after all seven fields are answered.
