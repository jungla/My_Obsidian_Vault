---
publish: true
title: Loan Management System Enhancements
created: 2026-11-06T12:00:45.725Z
modified: 2026-11-15T20:07:34.569Z
published: 2026-11-18T11:03:31.268Z
wispr_id: 3c934c27-1bae-46fb-bc35-bc6e88355799
type: note
updated: 2026-11-15T20:07:34.569Z
duration: 40m
speakers:
  - Chipanha
  - Jean Mensa
source: wispr-flow
---

> [!summary]- Flow Summary
> Eco-Connect web app approved as the direction, but its data must come from a cleaned Google Sheet master file, targeting finalization before next week's Tanga training.

### Spreadsheet Updates

- Repayment status column added (no loan, not paid, partially paid at 30%, fully paid); should become a repaid-vs-loan percentage instead
- Entering a member ID auto-fills details; transaction UUID auto-generates via VBA after all fields, including a new calendar date picker
- UUID should move to column A since it is the transaction ID; generating on receipt is fine
- Loan cycle meant a per-individual count of loans received in master data (e.g. 6th loan), not a dropdown

### Loan Reasons and Deposits

- Merge school fees, emergency and personal expenses into personal expenses; expand business into specific business types
- Business list could be AI-generated from common livelihoods in Pemba (e.g. fishing equipment, sewing machine, food stand)
- Deposits now auto-pay outstanding loans in master data; deposit type dropdown includes eco-credit activities
- New member registration sheet with button (name, gender, education, livelihood, village, group), suited to the Tanga team

### Interface Options: Softer vs Eco-Connect

- Jean Mensa showed Softer, a free-for-small-teams AI tool building dashboards and entry forms over Google Sheets
- Chipanha demoed Eco-Connect, built on Supabase and hosted on Vercel, with language switching and real imported data
- Eco-Connect has dashboard, groups, members, savings/repayments, loans, loan applications, SMS, banking, reports, administration
  - SMS meant for group leader reminders; planned mobile app limits leaders to their own group
- Jean Mensa called it exactly what is needed, but wants it linked to Google Sheets, and WCS emails used for accounts

### Eco-Connect Feedback

- Loans split across three pages is confusing; use a form plus list per area, matching savings
- Rename SMS to reminders or notifications; bank account registration belongs under groups
- Savings form needs an auto-generated transaction ID

### Next Steps

- (Chipanha) Update spreadsheet: repayment percentage, UUID in column A, loan count per individual, expanded business loan reasons
- (Chipanha) Invite Jean Mensa to the Vercel project
- (Chipanha) Restructure Eco-Connect pages, add auto transaction ID, rename SMS to reminders, move bank info under groups
- (Chipanha) Import Excel into Google Sheets using WCS email and share the link with Jean Mensa
- (Chipanha) Adapt Eco-Connect to read from the finalized Google Sheet, ideally before next week's Tanga training
- (Jean Mensa) Clean up the shared spreadsheet (table titles, proper English) and confirm when final

### Decisions Made

- Google Sheet remains the source data; the web app reads from it, with a database copy optional
