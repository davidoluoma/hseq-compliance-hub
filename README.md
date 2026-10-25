# HSEQ Compliance Hub — SharePoint & Power BI

## Overview
A portfolio demonstration of Microsoft SharePoint Online and Power BI for HSEQ (Health, Safety, Environment and Quality) compliance reporting and controlled-document management.

## Business problem
HSEQ teams need a consistent way to monitor corrective actions, ownership, due dates and closure, while keeping document metadata and review information visible.

## Demonstration solution
- SharePoint site named **HSEQ Compliance Hub**.
- Controlled Documents library with document number, type, department, version, status, review due date and approval-status metadata.
- Corrective Actions Register with action title, source, location, department, risk level, owner, dates and status.
- Power BI report file, sample datasets, data-quality log and screenshots.
- Six documented DAX measures for corrective-action reporting.

## Tools
SharePoint Online · Power BI Desktop · Power Query · DAX · Excel · CSV

## Repository structure
- `PROJECT-SUMMARY.md` — portfolio case study
- `DAX-MEASURES.md` — measure definitions
- `sample-data/` — sample CSV and Excel data
- `assets/HSEQ_Compliance_Dashboard.pbix` — Power BI report file
- `assets/screenshots/` — SharePoint and data-preparation evidence
- `DATA-PRIVACY-CHECKLIST.md` — checks to complete before public release

## Review the report
1. Open `assets/HSEQ_Compliance_Dashboard.pbix` in Power BI Desktop.
2. If prompted for source locations, use Power Query / Data source settings to reconnect to files in `sample-data/`.
3. Review the screenshots for evidence of the SharePoint setup.

## Important
All records are demonstration/sample data, not live operational or safety information. This repository contains report and evidence files; it does not deploy or recreate the SharePoint site. Review screenshots and the PBIX for private names, tenant details, source paths or confidential data before making this repository public. Do not claim automation is implemented unless flows were actually configured and tested.
