# TN — state education directory sources

Agency: Tennessee Department of Education — Tennessee School Directory (Power Pages portal)

Download date: 2026-10-21

The portal's "Download Directory" button runs JavaScript that pages the portal's public OData endpoint (`/_api/accounts?fetchXml=...`, 5,000 rows per page) and builds the Excel file client-side, so the file was produced by clicking that button in headless Chromium and saving the browser download (TN-School-Directory.xlsx). Row 1 of the sheet is a stray page-text cell ("Home"), the header is row 2 — kept unmodified. Includes active and inactive public, charter, virtual and **private** schools (727 active private). `Principal` filled on 5,081 rows, `Email Address` (school/principal email) on 3,717 rows. No separate district/superintendent rows.

## `TN-School-Directory.xlsx`

All Tennessee schools in the directory with region, district, NCES school no., principal, email, website.

- URL: https://tnschooldirectory.tnedu.gov/ (Download Directory button; data from https://tnschooldirectory.tnedu.gov/_api/accounts)
- How obtained: Headless browser click on `#download-btn`; the page's script fetched 2 API pages and exported 5,578 rows.
- Size: 738,490 bytes
- Sheet: Sheet1
- Data rows: 5,578
- Column count: 22
- Columns: `Region`, `District`, `District No.`, `School Name`, `School No.`, `NCES School No.`, `Principal`, `Type`, `Grade Level`, `Categories`, `County`, `Status`, `Address 1 Composite`, `Address 1 City`, `Address 1 State`, `Address 1 Zipcode`, `Address 2 Composite`, `Phone 1`, `Phone 2`, `Fax 1`, `Email Address`, `Website`
