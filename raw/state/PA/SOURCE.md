# PA — state education directory sources

Agency: Pennsylvania Department of Education — EdNA (Educational Names & Addresses), Output Files

Download date: 2026-10-21

All three files were produced with the form defaults (County = ALL, Status = Open, all categories, all administrators). PA EdNA contains administrator names, titles and phones; email columns exist but are sparsely filled (`SchoolPublicEmailAddress` 51 of 3,035 rows, `LEAPublicEmailAddress` 169; `PublicEmailAddress` in the nonpublic file is empty). `EdNA_ExtractEntitiesAdmin.xlsx` covers every entity type in EdNA (districts, IUs, charters, nonpublic/private, higher ed, libraries, Act 48 providers, etc.) with the chief administrator; `LEAAdmin*` in the public-schools file is the superintendent / CEO, `SchoolAdmin*` is the principal.

## `EdNA_ExtractPublicSchools.xlsx`

Open public schools with parent LEA, LEA chief administrator (superintendent) and school administrator (principal).

- URL: https://www.edna.pa.gov/Screens/Extracts/wfExtractPublicSchools.aspx
- How obtained: ASP.NET form postback: GET the page, POST back all default form fields + `ctl00$MainContent$cmdExport=Export`. Server filename ExtractPublicSchools.xlsx.
- Size: 1,190,729 bytes
- Sheet: ExtractPublicSchools
- Data rows: 3,035
- Column count: 92
- Columns: `LEAAUNumber`, `LEAInstName`, `PreK_Half`, `LEACategory`, `LEAIUNumber`, `LEAIU`, `LEACountyName`, `LEALegislativeDistrict`, `LEAStatus`, `LEAStatusEffectiveDate`, `LEAWebAddress`, `LEAPublicEmailAddress`, `Latitude`, `Longitude`, `LEAMailingAddressLine1`, `LEAMailingAddressLine2`, `LEAMailingCity`, `LEAMailingState`, `LEAMailingZipCode`, `LEAMailingZipCodeExtn`, `LEALocationAddressLine1`, `LEALocationAddressLine2`, `LEALocationCity`, `LEALocationState`, `LEALocationZipCode`, `LEALocationZipCodeExtn`, `LEAPhoneNumber`, `LEAPhoneNumberExtn`, `LEAAdminTitle`, `LEAAdminSalutation`, `LEAAdminFirstName`, `LEAAdminMiddleInitial`, `LEAAdminLastName`, `LEAAdminSuffix`, `LEAAdminPhone`, `LEAAdminPhoneExtn`, `SchoolInstCtgyDesc`, `SchoolAUNNum`, `SchoolBranchNum`, `SchoolName`, `GradeYear`, `GradeList`, `GradeCtgy`, `K4_Half`, `K4_Full`, `K5_Half`, `K5_Full`, `Grade_1`, `Grade_2`, `Grade_3`, `Grade_4`, `Grade_5`, `Grade_6`, `Elementary_Ungraded`, `Grade_7`, `Grade_8`, `Grade_9`, `Grade_10`, `Grade_11`, `Grade_12`, `Secondary_Ungraded`, `SchoolCountyName`, `SchoolStatus`, `SchoolStatusEffDate`, `SchoolWebAddress`, `SchoolPublicEmailAddress`, `SchoolPhone`, `SchoolPhoneExtn`, `SchoolMailingAddressLine1`, `SchoolMailingAddressLine2`, `SchoolMailingCity`, `SchoolMailingState`, `SchoolMailingZipCode`, `SchoolMailingZipCodeExtn`, `SchoolLocationAddressLine1`, `SchoolLocationAddressLine2`, `SchoolLocationCity`, `SchoolLocationState`, `SchoolLocationZipCode`, `SchoolLocationZipCodeExtn`, `SchoolAdminTitle`, `SchoolAdminSalutation`, `SchoolAdminFirstName`, `SchoolAdminMiddleInitial`, `SchoolAdminLastName`, `SchoolAdminSuffix`, `CyberSchoolInd`, `CharterEffectiveDate`, `CharterExpirationDate`, `LEALocaleDescription`, `LEAClassCode`, `LEAClassCodeDesc`

## `EdNA_ExtractEntitiesAdmin.xlsx`

"Educational Entities and Administrators" — all open entities with all administrators.

- URL: https://www.edna.pa.gov/Screens/Extracts/wfExtractEntitiesAdmin.aspx
- How obtained: ASP.NET form postback (Export button, defaults). Server filename ExtractEntitiesAdmin.xlsx.
- Size: 3,056,106 bytes
- Sheet: ExtractEntitiesAdmin
- Data rows: 18,472
- Column count: 33
- Columns: `AUNumber`, `InstName`, `Category`, `IUNumber`, `IU`, `CountyName`, `StatusDescription`, `EffectiveDate`, `PhoneNumber`, `PhoneNumberExtn`, `WebAddress`, `MailingAddressLine1`, `MailingAddressLine2`, `MailingCity`, `MailingState`, `MailingZipCode`, `MailingZipCodeExtn`, `LocationAddressLine1`, `LocationAddressLine2`, `LocationCity`, `LocationState`, `LocationZipCode`, `LocationZipCodeExtn`, `Title`, `Salutation`, `FirstName`, `MiddleInitial`, `LastName`, `Suffix`, `AdminPhoneNumber`, `AdminPhoneNumberExtn`, `CommissionStartDate`, `CommissionExpirationDate`

## `EdNA_ExtractPNP_private_nonpublic.xlsx`

"Private and Nonpublic Entities Extract" with NCES ID, administrator name/title/phone.

- URL: https://www.edna.pa.gov/Screens/Extracts/wfPNP.aspx
- How obtained: ASP.NET form postback (Export button, defaults). Server filename ExtractPNP.xlsx.
- Size: 750,961 bytes
- Sheet: ExtractPNP
- Data rows: 3,955
- Column count: 39
- Columns: `AUNumber`, `PubSchOrBranchNumber`, `NCESIdNumber`, `InstName`, `Category`, `CountyName`, `StatusDescription`, `EffectiveDate`, `PhoneNumber`, `PhoneNumberExtn`, `WebAddress`, `PublicEmailAddress`, `IUNumber`, `IU`, `Latitude`, `Longitude`, `LocaleDescription`, `ClassCode`, `ClassCodeDesc`, `MailingAddressLine1`, `MailingAddressLine2`, `MailingCity`, `MailingState`, `MailingZipCode`, `MailingZipCodeExtn`, `LocationAddressLine1`, `LocationAddressLine2`, `LocationCity`, `LocationState`, `LocationZipCode`, `LocationZipCodeExtn`, `AdminTitle`, `AdminSalutation`, `AdminFirstName`, `AdminMiddleInitial`, `AdminLastName`, `AdminSuffix`, `AdminPhone`, `AdminPhoneExtn`
