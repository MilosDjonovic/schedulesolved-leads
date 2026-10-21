# FL — state education directory sources

Agency: Florida Department of Education (FLDOE) — Master School ID (MSID) application and Private Schools Directory

Download date: 2026-10-21

MSID files are served by the ColdFusion MSID app as tab-delimited text with an `.xls` filename/`application/msexcel` content type; saved unmodified with a `.txt` extension. `EMAIL_ADDRESS_PRI` holds the principal's email (4,458 of 4,785 active rows populated). Superintendents: there is no separate superintendent file reachable — www.fldoe.org returns Akamai 403 to this environment — but each district's `9001 ... DISTRICT OFFICE` row sometimes carries a contact name/email; `SUPERINTENDENT_IND` is a district-level appointed/elected flag. Federal (NCES) district/school numbers are in `MSID_all_schools.txt` (`FEDERAL_DIST_NO`, `FEDERAL_SCHL_NO`).

## `MSID_active_schools.txt`

All active public schools with principal name, title, principal email, phone, website.

- URL: https://eds.fldoe.org/EDS/MasterSchoolID/Downloads/Active_schools.cfm
- How obtained: Form postback: GET https://eds.fldoe.org/EDS/MasterSchoolID/ (session cookie) → POST Downloads.cfm → POST Downloads/Active_schools.cfm ("Active Schools" Download button). Server filename MSID_active_school.xls.
- Size: 2,180,213 bytes
- Data rows: 4,785
- Column count: 38
- Columns: `DISTRICT`, `DISTRICT_NAME`, `LOCATION_DISTRICT`, `LOC_DISTRICT_NAME`, `SCHOOL`, `SCHOOL_NAME_LONG`, `SCHOOL_NAME_SHORT`, `MAILING_ADDRESS1`, `MAILING_ADDRESS2`, `MAILING_CITY`, `MAILING_STATE`, `MAILING_ZIP`, `PHYSICAL_ADDRESS`, `PHYSICAL_CITY`, `PHYSICAL_STATE`, `PHYSICAL_ZIP`, `PHONE_NUMBER`, `SUNCOM_NUMBER`, `FAX_NUMBER`, `WEB_ADDRESS`, `EMAIL_ADDRESS_PRI`, `PRINCIPAL_LAST`, `PRINCIPAL_FIRST`, `PRINCIPAL_MI`, `PRINCIPAL_TITLE`, `SUPERINTENDENT_IND`, `GRADE_CODE`, `TYPE`, `CHARTER_SCHL_STAT`, `SCHL_FUNC_SETTING`, `PRIMARY_SERV_TYPE`, `NEG_DEL_IND`, `NEG_DEL_CLASS`, `MAGNET_STATUS`, `MAGNET_SPECIALTY`, `MAGNET_PURPOSE`, `CLASSICAL_SCHOOL`, ``

## `MSID_all_schools.txt`

All schools ever in MSID (active + closed + future), 77 columns incl. NCES IDs, lat/long, principal name/email.

- URL: https://eds.fldoe.org/EDS/MasterSchoolID/Downloads/All_schools.cfm
- How obtained: Same form postback flow, "All Schools" Download button. Server filename MSID_all_schools.xls.
- Size: 2,901,241 bytes
- Data rows: 7,209
- Column count: 77
- Columns: `DISTRICT`, `SCHOOL`, `LOCATION_DISTRICT`, `OFFR_DISTRICT`, `GM_AGENCY_CODE`, `TYPE`, `ROI_TYPE`, `YEAR_ROUND_SCHOOL`, `ACC_TYPE`, `ACTIVITY_CODE`, `DISTRICT_NAME`, `LOC_DISTRICT_NAME`, `SCHOOL_NAME_LONG`, `SCHOOL_NAME_SHORT`, `GRADE_CODE`, `NEG_DEL_IND`, `NEG_DEL_CLASS`, `ACCREDITED_SACS`, `PHONE_NUMBER`, `SUNCOM_NUMBER`, `FAX_NUMBER`, `MAGNET_STATUS`, `MAGNET_SPECIALTY`, `MAGNET_PURPOSE`, `CS_SCHOOL_CHOICE`, `PHYSICAL_ADDRESS`, `PHYSICAL_CITY`, `PHYSICAL_STATE`, `PHYSICAL_ZIP`, `MAILING_ADDRESS1`, `MAILING_ADDRESS2`, `MAILING_CITY`, `MAILING_STATE`, `MAILING_ZIP`, `PRINCIPAL_LAST`, `PRINCIPAL_FIRST`, `PRINCIPAL_MI`, `PRINCIPAL_TITLE`, `FEDERAL_DIST_NO`, `FEDERAL_SCHL_NO`, `ETS_CEEB_NO`, `COMMENTS`, `REGION_CODE`, `CHARTER_SCHL_STAT`, `CHARTER_SCHL_OPEN`, `SCHL_FUNC_SETTING`, `TITLE_I_STATUS`, `PRIMARY_SERV_TYPE`, `DATE_OPENED`, `DATE_CLOSED`, `LATITUDE`, `LONGITUDE`, `SCHOOL_GRADE`, `IMPROVEMENT_RATING`, `AYP`, `WEB_ADDRESS`, `EMAIL_ADDRESS_PRI`, `PROJECTED_OPENING`, `SUPERINTENDENT_IND`, `SCHOOL_IMPROVEMENT`, `SI_TURNAROUND_STATUS`, `SI_TURNAROUND_YEAR_STATUS`, `SI_TURNAROUND_CYCLE`, `SI_TURNAROUND_OPT`, `SI_REGION_CODE`, `ACCOUNTABILITY_ESE_CTR`, `NINE_HUNDRED_ANNUALLY`, `DJJ_IMPROV_YEAR_STATUS`, `DJJ_PROV_OPTIONS`, `CLASSICAL_SCHOOL`, `ADDED_DATE`, `ADDED_USERID`, `CHANGED_DATE`, `CHANGED_USERID`, `ACC_CHA_DATE`, `ACC_CHA_USERID`, ``

## `PrivateSchools_All.xlsx`

Private school directory from the annual private-school survey: director name + director email, contact name + email, phone, grades, enrollment by grade.

- URL: https://web09.fldoe.org/PrivateSchoolDirectory/DownloadSchools?handler=DownloadAll
- How obtained: Form postback: GET https://web09.fldoe.org/PrivateSchoolDirectory/DownloadSchools (antiforgery token + cookie) → POST ?handler=DownloadAll ("Download All Schools").
- Size: 396,840 bytes
- Sheet: PrivateSchools
- Data rows: 3,547
- Column count: 39
- Columns: `District`, `School Name`, `School Code`, `Director`, `Director Email`, `Contact`, `Contact Email`, `Address 1`, `Address 2`, `City`, `State`, `Zip`, `Phone`, `Fax`, `FES Educational Options Participant`, `FTC Participant`, `FES Unique Abilities Participant`, `PEP Participant`, `Non-Profit`, `Religious`, `Denomination`, `Grade Levels`, `Accreditation`, `Student Type`, `Last Annual Survey Year`, `Pre-K`, `Kindergarten`, `Grade 1`, `Grade 2`, `Grade 3`, `Grade 4`, `Grade 5`, `Grade 6`, `Grade 7`, `Grade 8`, `Grade 9`, `Grade 10`, `Grade 11`, `Grade 12`
