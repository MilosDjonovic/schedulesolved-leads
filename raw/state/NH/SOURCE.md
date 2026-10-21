# NH — state education directory sources

Agency: New Hampshire Department of Education — Bureau of Education Statistics, Schools and SAU Information (myNHDOE Public Reports)

Download date: 2026-10-21

my.doe.nh.gov is Akamai-protected and returns 403 to curl; the public report links were opened in headless Chromium, which received the files as downloads. Both are real .xls (BIFF) files despite the 'CSV' report names; row 1 is a title ("School List - Up to date as of 10/21/2026"), header on row 2. School file: one row per school with its administrator (principal/head) name, title and email — 506 public/charter and 136 **non-public** schools; 622 of 642 rows have an email. SAU file: superintendents (Admin Type SUP), business administrators (BUS), assistant superintendents (ASU) etc. with emails. The separate 'Senior Education Official' (SupList) and 'Non-Public Schools' reports are HTML pages whose content is already covered by these two files; not saved.

## `NHDOE_SchoolListCSV_School_Information_All.xls`

All public, chartered public and non-public schools with principal name, title, email.

- URL: https://my.doe.nh.gov/myNHDOE/Help/PublicReports.aspx?ReportName=SchoolListCSV
- How obtained: Public report link ("School Information - All") from https://www.education.nh.gov/who-we-are/division-of-educator-and-analytic-resources/bureau-of-education-statistics/schools-and-sau-information , opened in headless Chromium (download SchoolListCSV.xls).
- Size: 535,032 bytes
- Sheet: SchoolListCSV
- Data rows: 642
- Column count: 30
- Columns: `Dst ID`, `Dist Name`, `Sch ID`, `School Name`, `Open Date`, `FName`, `MI`, `LName`, `Title`, `Address1`, `Address2`, `City`, `State`, `Zip Code`, `Phone`, `Fax`, `EMail`, `County`, `Region`, `School Group`, `Type`, `Sch Type Desc`, `Sch Apr Lvl`, `Sch Apr Lvl Desc`, `Grade Span`, `Sau ID`, `SAUName`, `Admin Type`, `Group Id`, `Web Page`

## `NHDOE_SAUListCSV_SAU_Information.xls`

School Administrative Units with superintendent, assistant superintendent and business administrator names and emails.

- URL: https://my.doe.nh.gov/myNHDOE/Help/PublicReports.aspx?ReportName=SAUListCSV
- How obtained: Public report link ("SAU Information"), headless Chromium (download SAUListCSV.xls).
- Size: 125,429 bytes
- Sheet: SAUListCSV
- Data rows: 277
- Column count: 16
- Columns: `SAU`, `SAUName`, `Admin Type`, `Title`, `FName`, `MI`, `LName`, `Address1`, `Address2`, `Town`, `State`, `Zip Code`, `Phone`, `FAX`, `Email`, `Web Page`
