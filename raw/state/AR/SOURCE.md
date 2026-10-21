# AR — state education directory sources

Agency: Arkansas Division of Elementary and Secondary Education (DESE) — ADE Data Center, School Personnel Directory (SPD)

Download date: 2026-10-21

SPD is fed daily from the ADE SIS LEA profiles. The "All" view (https://adedata.arkansas.gov/SPD/Home/DirectoryAll) has an **Export Excel** button; its link was downloaded directly (server filename "SPD Printed-10-21-2026-06_16_06.xlsx"). One row per contact person per LEA (district or school; `LEA` = 7-digit state LEA number, school LEAs are district number + 3 digits) with title, phone, email; every row has an email. `Title` can hold several roles separated by line breaks; rows whose roles include `Superintendent`: 265; `Principal or School Administrator`: 1057. Other roles: assistant principals, counselors, nurses, coordinators, etc. Header row is preceded by title rows (kept). No DESE private-school contact file found; the NCES ID Directory (/nid) is a separate lookup tool.

## `SPD_All_Printed-10-21-2026.xlsx`

All district and school personnel contacts in SPD.

- URL: https://adedata.arkansas.gov/SPD/Home/ExceliseDirectoryAll?sortDescending=False&sortField=DirectoryName
- How obtained: Direct link behind the "Export Excel" button on https://adedata.arkansas.gov/SPD/Home/DirectoryAll
- Size: 1,316,181 bytes
- Sheet: SPD  All
- Data rows: 11,792
- Column count: 22
- Columns: `LEA`, `LEA Name`, `Grade Low`, `Grade High`, `Contact Name`, `Title`, `Phone Number`, `Email`, `Fax Number`, `Website`, `Phone Number`, `Fax Number`, `Mailing Address 1`, `Mailing Address 2`, `Mailing City`, `Mailing State`, `Mailing Zipcode`, `Shipping Address 1`, `Shipping Address 2`, `Shipping City`, `Shipping State`, `Shipping Zipcode`
