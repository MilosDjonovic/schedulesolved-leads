# MI — state education directory sources

Agency: Michigan Center for Educational Performance and Information (CEPI) — Educational Entity Master (EEM), Public Data Sets

Download date: 2026-10-21

All 34 entity types were selected (higher ed, ISD/LEA/PSA (charter)/nonpublic/state districts, schools, unique education providers, ancillary facilities, etc.), all statuses (open and closed). Contacts: `EntityEmail` (generic entity/admin email), `EntityPhone`, `EntityLeadAdminHonorific/FirstName/LastName` (principal for schools, superintendent for districts). Among open LEA/PSA/Nonpublic schools: 3,785 rows, 3,778 with EntityEmail, 3,492 with lead admin name. NCES code in `EntityNCESCode`. Column descriptions PDF is linked on the page.

## `EEM_public_dataset_all_entity_types.csv`

EEM public data set, all entity types.

- URL: https://cepi.state.mi.us/eem/PublicDatasets.aspx
- How obtained: ASP.NET form postback: GET the page, POST back with all 34 `ctl00$cphMain$cblEntityTypes$N` checkboxes checked, `ctl00$cphMain$ddlFormat=0` (CSV) and the `Download Data Set` button. Server filename `EEMDataReport 10-21-2026 06-14-10-071.csv`.
- Size: 8,174,692 bytes
- Data rows: 16,638
- Column count: 62
- Columns: `ISDCode`, `ISDOfficialName`, `DistrictCode`, `DistrictOfficialName`, `DistrictType`, `DistrictTypeName`, `DistrictCommonName`, `EntityCode`, `EntityOfficialName`, `AgreementNumber`, `EntityType`, `EntityTypeName`, `EntityTypeGroup`, `EntityTypeGroupName`, `EntityTypeCategory`, `EntityTypeCategoryName`, `EntityCountyCode`, `EntityCountyName`, `EntityCharteringAgencyCode`, `EntityCharteringAgencyName`, `EntityGeographicLEADistrictCode`, `EntityGeographicLEADistrictOfficialName`, `EntityNCESCode`, `EntityLocaleCode`, `EntityLocaleName`, `EntityAuthorizedEducationalSettings`, `EntityActualEducationalSettings`, `EntityStatus`, `EntityOpenDate`, `EntityCloseDate`, `EntityAuthorizedGrades`, `EntityActualGrades`, `EntityFIPSCode`, `EnttiyREMCId`, `EntityScheduleList`, `EntityEarlyChildhoodProgramList`, `ReceivesTransportationServicesFromCode`, `ReceivesTransportationServicesFromOfficialName`, `EntityReligiousOrientationCode`, `EntityReligiousOrientationName`, `EntityEmail`, `EntityPhone`, `EntityPhoneExt`, `EntityFax`, `EntityFaxExt`, `EntityLeadAdminHonorific`, `EntityLeadAdminFirstName`, `EntityLeadAdminLastName`, `EntityPhysicalStreet`, `EntityPhysicalCity`, `EntityPhysicalState`, `EntityPhysicalZip4`, `EntityMailingStreet`, `EntityMailingCity`, `EntityMailingState`, `EntityMailingZip4`, `EarlyMiddleCollege`, `SEEType`, `HeadStartGrantee`, `SchoolEmphasis`, `ESSASupportStatus`, `MEMCACertification`
