# WI — state education directory sources

Agency: Wisconsin Department of Public Instruction (DPI) — Wisconsin School Directory

Download date: 2026-10-21

The directory (https://apps6.dpi.wi.gov/SchDirPublic/) is a Blazor Server app (no static URL). On the Contacts page, **Statewide Downloads → Download All Contacts** was clicked in headless Chromium and the browser download saved (server filename sd-statewide-contacts-all-20261021T054829.csv). One row per contact; 50 contact types including `District Administrator` (superintendent, 421), `Public School Primary Contact` (principal, 2,120), `Add'l Public School Principal`, `Private School Primary Contact` (877), `Independent Charter School Primary Contact`, plus coordinators. Entity lists (districts/schools/private schools pages) have no statewide-download button, so school IDs come only via `LEA Code`/`School Code` in this file.

## `sd-statewide-contacts-all-20261021T054829.csv`

All 11,912 contacts in the WI School Directory, public and private.

- URL: https://apps6.dpi.wi.gov/SchDirPublic/contacts
- How obtained: Browser click: Contacts → Statewide Downloads → Download All Contacts (Blazor app; file generated server-side and delivered as a download).
- Size: 2,543,836 bytes
- Data rows: 11,912
- Column count: 16
- Columns: `Contact Type`, `Local Title`, `LEA Code`, `District Name`, `School Code`, `School Name`, `CESA`, `Organization Type`, `School Type`, `Contact Name`, `Email`, `Phone`, `Ext`, `Address`, `Fax Number`, `County Name`
