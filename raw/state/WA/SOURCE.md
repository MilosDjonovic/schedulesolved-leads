# WA — state education directory sources

Agency: Washington Office of Superintendent of Public Instruction (OSPI) — EDS Washington Education Directory; WA State Board of Education (private schools)

Download date: 2026-10-21

OSPI EDS directory page https://eds.ospi.k12.wa.us/DirectoryEDS.aspx has one dropdown (District / ESD / School) and an "Export To Excel" button that returns CSV. School file: `PrincipalName` + `Email` (principal email); district file: `AdministratorName` (superintendent) + `Email`. Private schools: approval is handled by the State Board of Education; its list has **no contacts** (name/address/district only).

## `Washington_School_Directory_20261021.csv`

All schools with principal name, email, phone, grades, org category.

- URL: https://eds.ospi.k12.wa.us/DirectoryEDS.aspx
- How obtained: ASP.NET form postback: `ctl00$PageContent$DirectoryReportTypeDropDownList=2` (School) + `ctl00$PageContent$ExportToExcelButton`. Server filename Washington_School_Directory_20261021.csv.
- Size: 681,268 bytes
- Data rows: 2,477
- Column count: 20
- Columns: `ESDCode`, `ESDName`, `LEACode`, `LEAName`, `SchoolCode`, `SchoolName`, `LowestGrade`, `HighestGrade`, `AddressLine1`, `AddressLine2`, `City`, `State`, `ZipCode`, `PrincipalName`, `Email`, `Phone`, `OrgCategoryList`, `AYPCode`, `GradeCategory`, `TransitionToKindergarten`

## `Washington_District_Directory_20261021.csv`

Districts with superintendent (AdministratorName), phone, email.

- URL: https://eds.ospi.k12.wa.us/DirectoryEDS.aspx
- How obtained: Same postback with dropdown = 0 (District).
- Size: 56,883 bytes
- Data rows: 319
- Column count: 12
- Columns: `ESDCode`, `ESDName`, `DistrictCode`, `DistrictName`, `AddressLine1`, `AddressLine2`, `City`, `State`, `Zipcode`, `AdministratorName`, `Phone`, `Email`

## `Washington_Esd_Directory_20261021.csv`

Educational Service Districts with administrator, phone, email.

- URL: https://eds.ospi.k12.wa.us/DirectoryEDS.aspx
- How obtained: Same postback with dropdown = 1 (ESD).
- Size: 1,277 bytes
- Data rows: 9
- Column count: 9
- Columns: `ESD Name`, `ESD Code`, `AddressLine1`, `AddressLine2`, `State`, `ZipCode`, `Administrator Name`, `Phone`, `Email`

## `SBE_2026-27_Approved_Private_Schools.xlsx`

State Board of Education approved private schools 2026-27 — **no contacts**.

- URL: https://sbe.wa.gov/sites/default/files/2026-07/2026-27%20Approved%20Private%20Schools_0_0.xlsx
- How obtained: Direct link from https://sbe.wa.gov/our-work/private-schools
- Size: 57,302 bytes
- Sheet: 26-27 Approved Private Schools
- Data rows: 558
- Column count: 8
- Columns: `Approval`, `School Name`, `Street Address`, `City`, `ZIP`, `County`, `School District`, `Profit`
