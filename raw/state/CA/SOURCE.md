# CA — state education directory sources

Agency: California Department of Education (CDE), California School Directory (County-District-School Administration)

Download date: 2026-10-21

Contact coverage: school and district administrator first/last name (AdmFName/AdmLName), phone, website, CDS code, NCES district and school IDs. CDE no longer publishes administrator **emails** in the directory export (the file-structure page, https://www.cde.ca.gov/schooldirectory/topic/8, now lists only administrator name/phone). The only CDE files with emails are the Chief Business Officer contact lists (districts and charters). Private schools are included in `public_and_private_schools.txt` (`PublicYN` = N) with administrator names. Note: the host shows a Radware captcha to browser-like User-Agents and to mixed-case `/SchoolDirectory/` paths; plain curl to the lowercase `/schooldirectory/` path works.

## `pubschls.txt`

Public schools and districts (all statuses: active, closed, merged, pending).

- URL: https://www.cde.ca.gov/schooldirectory/report?rid=dl1&tp=txt
- How obtained: Direct link (tab-delimited) from https://www.cde.ca.gov/ds/si/ds/pubschls.asp
- Size: 8,795,663 bytes
- Data rows: 18,409
- Column count: 46
- Columns: `CDSCode`, `NCESDist`, `NCESSchool`, `StatusType`, `County`, `District`, `School`, `Street`, `StreetAbr`, `City`, `Zip`, `State`, `MailStreet`, `MailStrAbr`, `MailCity`, `MailZip`, `MailState`, `Phone`, `Ext`, `FaxNumber`, `WebSite`, `OpenDate`, `ClosedDate`, `Charter`, `CharterNum`, `FundingType`, `DOC`, `DOCType`, `SOC`, `SOCType`, `EdOpsCode`, `EdOpsName`, `EILCode`, `EILName`, `GSoffered`, `GSserved`, `Virtual`, `Magnet`, `YearRoundYN`, `FederalDFCDistrictID`, `Latitude`, `Longitude`, `AdmFName`, `AdmLName`, `LastUpDate`, `Multilingual`

## `public_and_private_schools.txt`

Public **and private** schools; same layout as pubschls.txt plus `PublicYN`. PublicYN counts: Y=17,015, N=9,870, No Data=1,394.

- URL: https://www.cde.ca.gov/schooldirectory/report?rid=dl3&tp=txt
- How obtained: Direct link (same report endpoint, rid=dl3; tab-delimited)
- Size: 13,696,382 bytes
- Data rows: 28,279
- Column count: 47
- Columns: `CDSCode`, `NCESDist`, `NCESSchool`, `StatusType`, `County`, `District`, `School`, `Street`, `StreetAbr`, `City`, `Zip`, `State`, `MailStreet`, `MailStrAbr`, `MailCity`, `MailZip`, `MailState`, `Phone`, `Ext`, `FaxNumber`, `WebSite`, `OpenDate`, `ClosedDate`, `Charter`, `CharterNum`, `FundingType`, `DOC`, `DOCType`, `SOC`, `SOCType`, `EdOpsCode`, `EdOpsName`, `EILCode`, `EILName`, `GSoffered`, `GSserved`, `Virtual`, `Magnet`, `YearRoundYN`, `FederalDFCDistrictID`, `Latitude`, `Longitude`, `AdmFName`, `AdmLName`, `LastUpDate`, `Multilingual`, `PublicYN`

## `pubdistricts.txt`

Public districts / county offices with superintendent (administrator) first & last name and phone.

- URL: https://www.cde.ca.gov/schooldirectory/report?rid=dl2&tp=txt
- How obtained: Direct link from https://www.cde.ca.gov/ds/si/ds/pubschls.asp
- Size: 261,144 bytes
- Data rows: 1,059
- Column count: 22
- Columns: `CD Code`, `County`, `District`, `Street`, `City`, `Zip`, `State`, `MailStreet`, `MailCity`, `MailZip`, `MailState`, `Phone`, `Ext`, `FaxNumber`, `AdmFName`, `AdmLName`, `Latitude`, `Longitude`, `DOC`, `DOCType`, `StatusType`, `LastUpDate`

## `district_chief_business_officers.txt`

District Chief Business Officer contacts, with email and phone.

- URL: https://www.cde.ca.gov/schooldirectory/report?rid=dl5&tp=txt
- How obtained: Direct link (report endpoint rid=dl5)
- Size: 170,032 bytes
- Data rows: 1,003
- Column count: 11
- Columns: `CDS Code`, `District`, `District Type`, `Role`, `Title`, `First Name`, `Last Name`, `Email`, `Area Code`, `Phone`, `Phone Extension`

## `charter_chief_business_officers.txt`

Charter school Chief Business Officer contacts, with email and phone.

- URL: https://www.cde.ca.gov/schooldirectory/report?rid=dl4&tp=txt
- How obtained: Direct link (report endpoint rid=dl4)
- Size: 248,505 bytes
- Data rows: 1,246
- Column count: 14
- Columns: `Charter Number`, `CDS Code`, `Status`, `Funding Type`, `District`, `School`, `Role`, `Title`, `First Name`, `Last Name`, `Email`, `Area Code`, `Phone`, `Phone Extension`
