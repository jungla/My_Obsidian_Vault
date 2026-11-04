---
publish: true
title: Credit and Savings Group Data Sheet Review
created: 2026-10-19T10:00:52.063Z
modified: 2026-10-19T10:53:37.928Z
published: 2026-11-02T19:31:51.945Z
wispr_id: 682bbab1-abea-4c1b-a011-35755a703dd8
type: note
updated: 2026-10-19T10:53:37.928Z
duration: 49m
speakers:
  - Ema
  - Hassan
  - Jean Mensa
source: wispr-flow
---

> [!summary]- Flow Summary
> Ema walked through the VSLA tracking spreadsheet; Jean Mensa and Hassan recommended restructuring it as clean relational tables (users, transactions) with net balances, and Ema will revise it.

### Spreadsheet Overview

- Workbook has 3 sheets: master data (records up to August 2026), monthly data (from September 2026), and summary.
  - Monthly entries auto-update the master sheet
- Master sheet uses dropdowns for education level, grouped activities, village, and the 10 current groups.
- Excess shares are auto-applied to outstanding loans, modeled on mobile credit systems like Tigo.

### Master Data Feedback

- Shares and loan repayments should not be separate: any deposit by a member with a loan repays that loan.
  - Current share formula sums only share columns, ignoring repayments
- Balance should simply be total deposits minus total loans; loan availability is 2x a positive balance, else zero.
- Replace phase 1/phase 2 loan columns with loans received to date; add initial loan and initial balance columns.
- Move activity column to transactions, remove merged title cells, and move per-group summaries to the summary tab.

### Monthly Data Restructure

- Monthly sheet should be a transaction list: one row per transaction, not one column per month.
  - Columns: transaction ID, user ID, type (loan or deposit), amount, date
- Split into separate loans and deposits tables, both linked to master data.
  - Loans need a justification field; deposits split into eco activities vs cash savings

### Summary Sheet

- Summary tab should have a dropdown to pick one group or all groups and auto-calculate stats (pivot table or macro).

### Training Update

- Hassan ran Sharks and Rays awareness and ID trainings with about 120 participants, including pre/post assessments.

### Next Steps

- (Ema) Revise the spreadsheet per the feedback and share it back for review
- (Hassan) Work with Ema on fixing the spreadsheet before reporting back to Jean Mensa
- (Hassan) Compile training pre/post assessments and group discussions into a report this week

### Decisions Made

- Keep unique member IDs built from village, group, and a cumulative number
- Add an 'Other' option to the activities dropdown for activities outside existing categories

[[Meetings/Wispr/Transcripts/Credit and Savings Group Data Sheet Review-2026-10-19_10-00-52-transcript]]
