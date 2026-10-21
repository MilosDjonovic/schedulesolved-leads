# MT — state education directory sources

Agency: Montana Office of Public Instruction (OPI) — Directory of Montana Schools, OPI Reporting Center central directory reports

Download date: 2026-10-21

Report links are on https://opi.mt.gov/Leadership/Management-Operations/Montana-Schools-Directory ("Advanced Search" presets). Each report page has a "Create Excel Spreadsheet" button (ASP.NET postback); the postback was replicated with curl (GET report page, POST default form state + `ctl00$ContentPlaceHolder1$btnExcel`). Files are real BIFF .xls despite an xlsx content-type header. Contacts are entered by district clerks in the OPI Contacts application. A full ~300-page PDF directory also exists (https://apps.opi.mt.gov/SchoolDirectory/frmdirectorydistrictpdf.aspx) — not needed given the Excel exports.

## `rptViewCentralDirectorySchoolStaffByDistrict_public_schools_principals.xls`

Every public school building with principal name, title, phone, email.

- URL: https://apps.opi.mt.gov/OPIReportingCenter/frmCentralDirectory.aspx?ProcName=procCentralDirectorySchoolStaffByDistrict&ScreenTitle=Principal%20Database&SelectDistrict=1&SelectSector=1&Sector=PUBLIC&SelectRole=1&ShowReport=1&ScreenMsg=Use%20this%20database%20to%20reach%20every%20school%20building%20in%20Montana
- How obtained: Report "Show All Public Schools" → Create Excel Spreadsheet (postback).
- Size: 442,304 bytes
- Sheet: rptViewCentralDirectorySchoolSt
- Data rows: 881
- Column count: 18
- Columns: `County Name`, `SS`, `System Name`, `LE`, `District Name`, `SC`, `School Name`, `First`, `Last`, `Title`, `Phone`, `Fax`, `Email`, `Address`, `City`, `State`, `Zip`, `Sector`

## `rptViewCentralDirectorySystemStaffBySystem_district_superintendents.xls`

District superintendents with staff email, system email, phone.

- URL: https://apps.opi.mt.gov/OPIReportingCenter/frmCentralDirectory.aspx?ProcName=procCentralDirectorySystemStaffBySystem&ScreenTitle=District%20Superintendents&SelectRole=1&Role=SUPT&ShowReport=1&ScreenMsg=%20Database%20of%20Montana%20District%20Superintendents
- How obtained: Report "Show All Public District Superintendents" → Create Excel Spreadsheet (postback).
- Size: 114,624 bytes
- Sheet: rptViewCentralDirectorySystemSt
- Data rows: 278
- Column count: 14
- Columns: `County Name`, `SS`, `System Name`, `First`, `Last`, `Title`, `Phone`, `Staff E mail`, `Address`, `City`, `State`, `ZIP`, `Role`, `System E mail`

## `NonPublic_Accredited_Schools.xls`

OPI-accredited non-public schools with contact name and email (only accredited ones are listed).

- URL: https://apps.opi.mt.gov/opireportingcenter/frmPublicReports.aspx?ProcName=procRptViewNonpublicAccredited&ScreenTitle=NonPublic%20Accredited%20Schools%20
- How obtained: Report "Show All Non-Public Accredited Schools" → Create Excel Spreadsheet (postback).
- Size: 16,320 bytes
- Sheet: rptViewNonpublicAccredited
- Data rows: 13
- Column count: 15
- Columns: `County Name`, `LE`, `District Name`, `SC`, `School Name`, `First`, `Last`, `Title`, `Phone`, `Fax`, `Email`, `Address`, `City`, `State`, `Zip`
