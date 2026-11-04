---
publish: true
title: Loan and Deposit Registry Update
created: 2026-10-29T10:00:03.789Z
modified: 2026-10-29T10:36:19.599Z
published: 2026-11-02T19:31:51.998Z
wispr_id: 4406db7c-1195-4a73-bb68-943f8d7a9558
type: note
updated: 2026-10-29T10:36:19.599Z
duration: 34m
speakers:
  - Chipanha
  - Hassan
  - Jean Mensa
source: wispr-flow
---

> [!summary]- Flow Summary
> Review of Chipanha's revised loan and deposit spreadsheet: Jean Mensa approved the direction and requested several structural fixes, plus support for Chipanha to attend the Tanga trainings for one week.

### Master Data Revisions

- Balance now equals total deposit minus total loan received; margin and per-group summary cells were removed
- Transaction type should not be user-chosen: deposits auto-count as loan repayment while balance is negative
- Evaluation conditions use equals instead of greater than, so values like 74 or 76 are missed
- Loan available is twice a positive balance; negative balance shows standing loan

### Deposit Registry

- Monthly sheet is now one row per transaction and should be renamed deposit registry
- Member IDs in sample data were inconsistent with names, prompting a lookup-based name field
- UUID transaction IDs needed so identical same-day deposits stay distinguishable, e.g. if moved to Kobo
- No ECO credit activity since August, but an ECO credit vs cash option is kept for the future

### Loan Register

- Zero-amount rows existed because all members were copied in; only actual loans belong there
- Repayment period is about six months per groups, but kept as a column since it may change

### Summary and Next Phase

- Summary sheet dropdown filters by one group or all groups; mostly real data except two groups
- Moving the database online for multi-group access will be discussed at the next meeting

### Tanga Training

- Tanga team reports a funds shortfall but calls the savings training a priority for this week
- <@person3:n=Shabani> shared training materials; <@person3:n=Emmanuel>'s attendance was dropped due to funds
  - Chipanha estimates one week is enough for the trainings

### Next Steps

- (Chipanha) Replace master activity column with primary livelihood and auto-set transaction type from balance
- (Chipanha) Replace evaluation with repayment percentage column and add late or months-remaining indicator
- (Chipanha) Add deposit and loan counts per member in master data
- (Chipanha) Make name an XLOOKUP from member ID and add UUID transaction IDs to deposit and loan registers
- (Chipanha) Rename to deposit registry and add ECO credit vs cash column with activity dropdown
- (Chipanha) Remove zero rows from loan register and add repayment time and loan reason columns, then load real data
- (Hassan) Share loan status statistics for <@person3:n=Jada>'s request (repayment rates, loan types, activities)
- (Hassan) Tell Tanga team Chipanha should attend the trainings for one week and report back

[[Meetings/Wispr/Transcripts/Loan and Deposit Registry Update-2026-10-29_10-00-03-transcript]]
