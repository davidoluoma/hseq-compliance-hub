# Project Summary — HSEQ Compliance Hub

**Project type:** HSEQ compliance reporting and controlled-document management demonstration  
**Tools:** SharePoint Online, Power BI, Power Query, DAX, Excel and CSV

## Problem
HSEQ teams need to monitor corrective-action ownership, due dates and closure while maintaining document metadata and review schedules. Fragmented tracking can make overdue work and document status harder to see.

## What I built
- A SharePoint site named **HSEQ Compliance Hub**.
- A **Controlled Documents** library with fields including document number, document type, department, version, document status, review due date and approval status.
- A **Corrective Actions Register** with action title, source, location, department, risk level, owner, dates and status.
- A Power BI report file for corrective-action analysis.
- A data-quality log covering duplicate rows, missing owners, missing due dates and inconsistent status/department spelling.
- Screenshots documenting the site, library columns, versioning settings, review views, permissions, version history and register.

## Key reporting measures
1. **Total Actions** — count of action records.
2. **Open Actions** — actions not marked Closed.
3. **Closed Actions** — actions marked Closed.
4. **Overdue Actions** — open actions whose due date is earlier than today.
5. **Closure Rate** — closed actions divided by total actions.
6. **Avg Days To Close** — average days between raised and closed dates for records with a close date.

The dashboard previously displayed 120 demonstration records. Recheck the current PBIX and data connections before presenting figures as current.

## Outcome
The project demonstrates a structured way to track corrective actions and controlled-document review information and to report compliance indicators.

## Caveats
All data should be treated as sample/demo data. Redact private names and tenant details from screenshots before public release. The repository contains supporting artifacts, not a deployable SharePoint site. Describe automation only if it was actually built and tested.
