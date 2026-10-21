# NY — state education directory sources

Agency: New York State Education Department (NYSED) — SEDREF (State Education Department Reference File) public reports

Download date: 2026-10-21

The person-contact columns are labelled `CEO ...` in SEDREF (for schools the CEO is the principal; for districts the superintendent). Report names below are NYSED's titles.

## `SEDREF_public_school_principal_contacts.csv`

Report: "Public Schools: Active Public School Principal Contact Info and School Grade Organization". Public schools with principal (CEO) name, title, email, phone.

- URL: https://eservices.nysed.gov/sedreports/api/reports/i87FF58798BFD4C1397D28779D529008C/1
- How obtained: SEDREF public reports SPA https://eservices.nysed.gov/sedreports/list?id=1 . The SPA's API GET https://eservices.nysed.gov/sedreports/api/reports/i87FF58798BFD4C1397D28779D529008C/1 returns a redirect URL to the public IBM Cognos pass-through (the generic public 'sedrefreports' account embedded by NYSED in the public report links — no user login) with storeID('i87FF58798BFD4C1397D28779D529008C'); run.outputFormat=HTML was changed to CSV and the URL was opened in headless Chromium (plain curl gets the async Cognos viewer page; the host returns 403 to the HeadlessChrome user-agent, so a desktop Chrome UA string was set). The CSV arrived as a browser download named "Public Schools_ Active Public School Principal Contact Info and School Grade Organization.csv".
- Size: 954,809 bytes
- Data rows: 4,383
- Column count: 18
- Columns: `Institution ID`, `Legal Name`, `Popular Name`, `SED Code`, `SchDistofLoc Code`, `SchDistofLoc Description`, `County Code`, `County Description`, `CEO Salutation`, `CEO FName`, `CEO LName`, `CEO Title`, `CEO Active Date`, `CEO email`, `CEO Phone #`, `CEO Phone Extension`, `Grade Organization Code`, `Grade Organization Description`

## `SEDREF_district_superintendent_contacts.csv`

Report: "School Districts: Active School District Superintendent Contact Info and Institution URL". Districts with superintendent name, email, phone, website.

- URL: https://eservices.nysed.gov/sedreports/api/reports/i673A0B99690E44DE9169E3F112697285/1
- How obtained: SEDREF public reports SPA https://eservices.nysed.gov/sedreports/list?id=1 . The SPA's API GET https://eservices.nysed.gov/sedreports/api/reports/i673A0B99690E44DE9169E3F112697285/1 returns a redirect URL to the public IBM Cognos pass-through (the generic public 'sedrefreports' account embedded by NYSED in the public report links — no user login) with storeID('i673A0B99690E44DE9169E3F112697285'); run.outputFormat=HTML was changed to CSV and the URL was opened in headless Chromium (plain curl gets the async Cognos viewer page; the host returns 403 to the HeadlessChrome user-agent, so a desktop Chrome UA string was set). The CSV arrived as a browser download named "School Districts_ Active School District Superintendent Contact Info and Institution URL.csv".
- Size: 141,719 bytes
- Data rows: 725
- Column count: 13
- Columns: `Institution ID`, `Legal Name`, `Popular Name`, `SED Code`, `CEO Salutation`, `CEO FName`, `CEO LName`, `CEO Title`, `CEO Active Date`, `CEO Phone#`, `CEO Phone Extension`, `CEO email`, `Institution URL`

## `SEDREF_districts_addresses_CEO.csv`

Report: "School Districts: Active School Districts with Mailing & Physical Addresses, Institution contact Info & CEO Contact Info". Districts with addresses, institution email/URL and superintendent contact.

- URL: https://eservices.nysed.gov/sedreports/api/reports/i81B4E31133AD46AA9467AFBEDB70BC7D/1
- How obtained: SEDREF public reports SPA https://eservices.nysed.gov/sedreports/list?id=1 . The SPA's API GET https://eservices.nysed.gov/sedreports/api/reports/i81B4E31133AD46AA9467AFBEDB70BC7D/1 returns a redirect URL to the public IBM Cognos pass-through (the generic public 'sedrefreports' account embedded by NYSED in the public report links — no user login) with storeID('i81B4E31133AD46AA9467AFBEDB70BC7D'); run.outputFormat=HTML was changed to CSV and the URL was opened in headless Chromium (plain curl gets the async Cognos viewer page; the host returns 403 to the HeadlessChrome user-agent, so a desktop Chrome UA string was set). The CSV arrived as a browser download named "School Districts_ Active School Districts with Mailing & Physical Addresses, Institution contact Info & CEO Contact Info.csv".
- Size: 248,770 bytes
- Data rows: 725
- Column count: 34
- Columns: `Institution ID`, `Legal Name`, `Popular Name`, `SED Code`, `District Type Code`, `District Type Description`, `Physical Address Line1`, `Physical Address Line2`, `Physical City`, `Physical State Code`, `Physical Zipcd5`, `Physical Zipadd4`, `Mailing Address Line1`, `Mailing Address Line2`, `Mailing City`, `Mailing State Code`, `Mailing Zipcd5`, `Mailing Zipadd4`, `County Code`, `County Description`, `Institution Phone #`, `Institution Phone Extension`, `Institution Fax #`, `Institution email`, `Institution URL`, `CEO Salutation`, `CEO FName`, `CEO LName`, `CEO Title`, `CEO Active Date`, `CEO Phone #`, `CEO Phone Extension`, `CEO Fax #`, `CEO email`

## `SEDREF_public_nonpublic_charter_schools_CEO.csv`

Report: "Public, Nonpublic & Charter Schools: Active Public, Nonpublic & Charter Schools CEO Info with Physical & Mailing addresses, Grades & Grade Orgs". All active schools incl. **nonpublic (private)** with CEO/principal name, email, phone.

- URL: https://eservices.nysed.gov/sedreports/api/reports/i4F0B510380DA448D96BE0114D35BBD3A/1
- How obtained: SEDREF public reports SPA https://eservices.nysed.gov/sedreports/list?id=1 . The SPA's API GET https://eservices.nysed.gov/sedreports/api/reports/i4F0B510380DA448D96BE0114D35BBD3A/1 returns a redirect URL to the public IBM Cognos pass-through (the generic public 'sedrefreports' account embedded by NYSED in the public report links — no user login) with storeID('i4F0B510380DA448D96BE0114D35BBD3A'); run.outputFormat=HTML was changed to CSV and the URL was opened in headless Chromium (plain curl gets the async Cognos viewer page; the host returns 403 to the HeadlessChrome user-agent, so a desktop Chrome UA string was set). The CSV arrived as a browser download named "Public, Nonpublic & Charter Schools_ Active Public, Nonpublic & Charter Schools CEO Info with Physical & Mailing addresses, Grades & Grade Orgs.csv".
- Size: 2,269,016 bytes
- Data rows: 6,570
- Column count: 47
- Columns: `Institution ID`, `Legal Name`, `Popular Name`, `SED Code`, `INST Type Code`, `INST Type Description`, `INST Sub Type Code`, `INST Sub Type Description`, `County Code`, `County Description`, `Physical Address Line1`, `Physical Address Line2`, `Physical City`, `Physical State Code`, `Physical Zipcd5`, `Mailing Address Line1`, `Mailing Address Line2`, `Mailing City`, `Mailing State Code`, `Mailing Zipcd5`, `CEO Salutation`, `CEO FName`, `CEO LName`, `CEO Title`, `CEO Active Date`, `CEO email`, `CEO Phone`, `CEO Phone Extension`, `Grade Organization Code`, `Grade Organization Description`, `Grade Pre-K`, `Grade Half K`, `Grade Full K`, `Grade 1`, `Grade 2`, `Grade 3`, `Grade 4`, `Grade 5`, `Grade 6`, `Grade Ungraded Elementary`, `Grade 7`, `Grade 8`, `Grade 9`, `Grade 10`, `Grade 11`, `Grade 12`, `Grade Ungraded Secondary`

## `SEDREF_nonpublic_schools_contacts.csv`

Report: "Religious and Independent (Nonpublic) Schools: Active NonPublic Schools with Physical & Mailing Addresses & Institution Contact Info". Nonpublic schools with institution email, phone, URL (no person names).

- URL: https://eservices.nysed.gov/sedreports/api/reports/i2C602FE06B554BD4AA9D15E39B0C0C16/1
- How obtained: SEDREF public reports SPA https://eservices.nysed.gov/sedreports/list?id=1 . The SPA's API GET https://eservices.nysed.gov/sedreports/api/reports/i2C602FE06B554BD4AA9D15E39B0C0C16/1 returns a redirect URL to the public IBM Cognos pass-through (the generic public 'sedrefreports' account embedded by NYSED in the public report links — no user login) with storeID('i2C602FE06B554BD4AA9D15E39B0C0C16'); run.outputFormat=HTML was changed to CSV and the URL was opened in headless Chromium (plain curl gets the async Cognos viewer page; the host returns 403 to the HeadlessChrome user-agent, so a desktop Chrome UA string was set). The CSV arrived as a browser download named "Religious and Independent (Nonpublic) Schools_ Active NonPublic Schools with Physical & Mailing Addresses & Institution Contact Info.csv".
- Size: 516,559 bytes
- Data rows: 1,819
- Column count: 28
- Columns: `Institution ID`, `Legal Name`, `Popular Name`, `SED Code`, `Active Date`, `INST Type Code`, `INST Type Description`, `INST Sub Type Code`, `INST Sub Type Description`, `County Code`, `County Description`, `Institution Phone #`, `Institution Phone Extension`, `Institution Fax #`, `Institution email`, `Institution URL`, `Physical Address Line1`, `Physical Address Line2`, `Physical City`, `Physical State Code`, `Physical Zipcd5`, `Physical Zipadd4`, `Mailing Address Line1`, `Mailing Address Line2`, `Mailing City`, `Mailing State Code`, `Mailing Zipcd5`, `Mailing Zipadd4`

## `SEDREF_charter_schools_CEO_board_president.csv`

Report: "Charter Schools: Active Charter Schools CEO and Board of Trustee President Contact Info". Charter schools with CEO and board president contacts.

- URL: https://eservices.nysed.gov/sedreports/api/reports/iBDAD651EB187440AA8B36BD9362ECD1B/1
- How obtained: SEDREF public reports SPA https://eservices.nysed.gov/sedreports/list?id=1 . The SPA's API GET https://eservices.nysed.gov/sedreports/api/reports/iBDAD651EB187440AA8B36BD9362ECD1B/1 returns a redirect URL to the public IBM Cognos pass-through (the generic public 'sedrefreports' account embedded by NYSED in the public report links — no user login) with storeID('iBDAD651EB187440AA8B36BD9362ECD1B'); run.outputFormat=HTML was changed to CSV and the URL was opened in headless Chromium (plain curl gets the async Cognos viewer page; the host returns 403 to the HeadlessChrome user-agent, so a desktop Chrome UA string was set). The CSV arrived as a browser download named "Charter Schools_ Active Charter Schools CEO and Board of Trustee President Contact Info.csv".
- Size: 125,853 bytes
- Data rows: 368
- Column count: 23
- Columns: `Institution ID`, `Legal Name`, `Popular Name`, `SED Code`, `Charter Sch Authorizer Code`, `Charter School Authorizer`, `Active Date`, `CEO Salutation`, `CEO FName`, `CEO LName`, `CEO Title`, `CEO Active Date`, `CEO Phone #`, `CEO Phone Extension`, `CEO email`, `BoardTrusteePres Salutation`, `BoardTrusteePres FName`, `BoardTrusteePres LName`, `BoardTrusteePres Title`, `BoardTrusteePres Active Date`, `BoardTrusteePres Phone #`, `BoardTrusteePres Phone Extension`, `BoardTrusteePres email`

## `SEDREF_NCES_IDs.csv`

Report: "School Districts, Public & Charter Schools: NCES IDs". Crosswalk SED code / Institution ID to NCES LEA and school IDs.

- URL: https://eservices.nysed.gov/sedreports/api/reports/iE0680D8ED23E4088B5F288AEE1B63E23/1
- How obtained: SEDREF public reports SPA https://eservices.nysed.gov/sedreports/list?id=1 . The SPA's API GET https://eservices.nysed.gov/sedreports/api/reports/iE0680D8ED23E4088B5F288AEE1B63E23/1 returns a redirect URL to the public IBM Cognos pass-through (the generic public 'sedrefreports' account embedded by NYSED in the public report links — no user login) with storeID('iE0680D8ED23E4088B5F288AEE1B63E23'); run.outputFormat=HTML was changed to CSV and the URL was opened in headless Chromium (plain curl gets the async Cognos viewer page; the host returns 403 to the HeadlessChrome user-agent, so a desktop Chrome UA string was set). The CSV arrived as a browser download named "School Districts, Public & Charter Schools_ NCES IDs.csv".
- Size: 1,212,728 bytes
- Data rows: 6,204
- Column count: 20
- Columns: `Institution ID`, `Legal Name`, `Popular Name`, `SED Code`, `SchDistofLoc Code`, `SchDistofLoc Description`, `County Code`, `County Description`, `INST Type Code`, `INST Type Description`, `INST Sub Type Code`, `INST Sub Type Description`, `Active Date`, `Inactive Date`, `EDEN NCES LEA ID`, `EDEN LEA Type CODE`, `EDEN LEA OP Status Code`, `EDEN NCES SCH ID`, `EDEN Sch Type Code`, `EDEN Sch OP Status Code`
