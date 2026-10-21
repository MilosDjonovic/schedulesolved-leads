# SC — state education directory sources

Agency: South Carolina Department of Education (SCDE) — School Directory

Download date: 2026-10-21

The directory page https://ed.sc.gov/districts-schools/schools/school-directory/ loads its school table from `schooldirectory.cfc?returnformat=json&method=getAllDeimsSchoolsFiltered` (1,361 school IDs); its **Export** button POSTs the table's row IDs (`sid`, JSON array, URL-safe base64, form field `myStr`) to `schooldirectory.cfc?method=getSchoolXLSFile2`. That request was replicated with all 1,361 IDs (= clicking Export on the unfiltered table); the server returned 1,316 rows. The parallel export for the 'special/alternative schools' tab (`getSchoolXLSFile3`, 120 IDs) returned HTTP 500 and was not saved. Private schools: SCDE posts only a 2023-24 private school survey list (no contacts; the sheet has 9 real columns followed by ~16,000 empty `ColumnNN` headers). No SCDE superintendent file was found.

## `SCDE_school_directory_report_21-Oct-26.xls`

Public schools 2026 with principal full name, principal email, principal phone, school phone/fax, website.

- URL: https://ed.sc.gov/sites/scdoe/includes/schoolDirectory2026/cfc/schooldirectory.cfc?method=getSchoolXLSFile2
- How obtained: POST replicating the page's Export button with all school IDs. Server filename "report_21-Oct-26_0657 AM.xls" (real BIFF .xls).
- Size: 569,344 bytes
- Sheet: Sheet1
- Data rows: 1,316
- Column count: 17
- Columns: `SCHOOLYEAR`, `DISTRICTCODE`, `SCHOOLCODE`, `SCHOOLNAME`, `COUNTYNAME`, `DISTRICTNAME`, `GRADESERVEDRANGE`, `PRINFULLNAME`, `ADDRESSPHYSICAL`, `CITY`, `STATE`, `ZIP`, `SCHOOLFAX`, `SCHOOLPHONE`, `PRINEMAIL`, `PRINPHONE`, `CHWEBURL`

## `2023-24_Private_School_Report_for_Publication.xlsx`

Private schools 2023-24 — **no contacts**.

- URL: https://ed.sc.gov/districts-schools/schools/school-directory/private-schools-listings-040424/
- How obtained: Direct link ("Private Schools Listing*") — the page URL itself returns the xlsx (Content-Disposition filename "2023-24 Private School Report for Publication.xlsx").
- Size: 157,062 bytes
- Sheet: 2023-24 Private School Report
- Data rows: 162
- Columns: `Response ID`, `SCHOOL NAME`, `STREET ADDRESS`, `CITY`, `ZIP`, `PHONE`, `GRADE SPAN`, `COUNTY`, `DISTRICT`, then empty headers `Column30` … `Column16303`
