---
publish: true
title: Kobo Data Management Workflow
created: 2026-10-21T07:00:35.968Z
modified: 2026-10-21T08:28:58.129Z
published: 2026-11-02T19:31:51.961Z
wispr_id: e24220d3-d2d5-4104-b730-731e6b52c16e
type: note
updated: 2026-10-21T08:28:58.129Z
duration: 1h 13m
speakers:
  - Bennett
source: wispr-flow
---

> [!summary]- Flow Summary
> WCS shark team reviewed a consultant's database pipeline (Kobo to staging QC to live dashboard) as a replacement for editing Kobo data in spreadsheets. Next: a test Kobo account for a demo, plus cost estimates.

### Current Kobo Setup and Pain Points

- WCS regional paid Kobo account hosts forms shared to country accounts (Tanzania, Kenya, Mozambique, Madagascar); forms differ slightly
- Species IDs are assigned in office from photos, then corrected offline in Excel, so Kobo never holds the clean data
- Analysis runs from Kobo downloads via R/Python scripts and a Streamlit dashboard; re-uploads have caused duplicate records
- Other countries lack Tanzania's coding capacity, so the shark program needs a no-code system

### Consultant's Pipeline Demo

- Server pulls Kobo submissions about every 2 hours, checking Kobo UUIDs so late or duplicate records are handled
- New records land in staging tables for monthly QC: outlier flags, photo checks, enumerator scorecards, change logs, then 'load to live'
- A specialist species ID column would override the field ID without deleting it; Kobo raw data is never edited
- Specialist review portal, role-based access, per-country views, and regional dashboards shown (Liberia, Gabon, Lake Tanganyika examples)

### Kobo Write-back and Edits

- Pushing corrections back to Kobo is possible but untested by consultant and would lack a full change log
- Records edited in Kobo after download are not re-fetched unless a change log is built in

### Photo Storage and Future Data

- Hosting all Kobo photos on a server is expensive; Kobo plan is currently unlimited but terms may change
- Option: purge images after QC and push them to WCS SharePoint, keeping a link and the positive ID
- Images could later support an ID guide and species splits (e.g. silky shark), so they must stay queryable
- About 3,000 BRUV samples and possible eDNA data could join the same database; merged Kenya forms can be imported via script

### Next Steps

- (Speaker 1) Load test data, refine the QC and species verification demo, then host it on a live server for testing
- (Speaker 1) Prepare cost estimates covering initial setup and a monthly retainer
- (Speaker 3) Create a test Kobo account, share one survey into it, and send the consultant a login

### Decisions Made

- Pipeline only needs to download the first version of each Kobo record
- Demo scope limited to data QC streamlining and species verification, not analytics

[[Meetings/Wispr/Transcripts/Kobo Data Management Workflow-2026-10-21_07-00-35-transcript]]
