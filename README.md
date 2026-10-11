# Home Credit LAP Qualification Voice Agent

## What this repository contains
This repository documents a Retell AI voice agent designed for preliminary qualification of an existing customer's Loan Against Property (LAP) enquiry.

## Files
- `system-prompt.md` — the agent's system prompt.
- `test-cases.md` — manual scenarios to validate eligibility and call flow before submission.

## Assignment scope
The agent checks seven required details: property type, ownership, original property documents, requested loan amount, occupation and bank-received income, estimated market value, and tenure.

It must not promise loan approval or a guaranteed interest rate. Agricultural property, unavailable original documents, cash-only income, and tenure outside 3–15 years disqualify the lead. Loan-transfer, refinance, balance-transfer, or EMI-reduction requests are referred to a specialist for follow-up.

## Current status
- [x] Retell agent created and prompt updated
- [x] Documentation files added
- [ ] Validate scenarios using an approved test method
- [ ] Capture a real test call recording and transcript if required
- [ ] Add the final public demo/recording link after it exists

## Important
Do not publish the agent or place a live call until you have reviewed Retell's billing and publication settings. This repository does not contain API keys, customer data, or a working standalone web app.
