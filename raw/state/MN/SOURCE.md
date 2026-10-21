# MN — state education directory sources

Agency: Minnesota Department of Education — MDE-ORG (MDE Organization Reference Glossary)

Download date: 2026-10-21

MDE-ORG (https://pub.education.mn.gov/MdeOrgView/) offers CSV output (`?output=csv`, "Excel-formatted CSV") only for its contact lists; both superintendent lists were downloaded. Principal names appear only on individual organization pages (`/organization/show/<id>`, no email shown) and there is no statewide principal export; the host is protected by a Radware bot manager that challenges after a few rapid requests, so per-school pages were not paged. Other contact-type lists (48 types, e.g. District Assessment Coordinator, Special Education Director, District Nonpublic School/Homeschool Liaison) are available at /MdeOrgView/contact/contactTypeList but were not needed. No nonpublic-school contact export exists in MDE-ORG.

## `MDE_superintendents_districts_and_charters.csv`

Superintendents / directors of all school districts and charter schools, with email and phone.

- URL: https://pub.education.mn.gov/MdeOrgView/districts/superintendentsDistricts?output=csv
- How obtained: Direct CSV link ("Superintendents/Directors for School Districts and Charter Schools", on https://pub.education.mn.gov/MdeOrgView/districts/index). Server filename MDE_Contacts_10-21-2026.csv.
- Size: 79,191 bytes
- Data rows: 543
- Column count: 8
- Columns: `Number`, `Organization`, `Title`, `Name`, `Email`, `Phone`, `StateOrganizationId`, `Data Extracted`

## `MDE_directors_charter_schools.csv`

Charter school directors with email and phone (subset of the file above).

- URL: https://pub.education.mn.gov/MdeOrgView/districts/superintendentsCharters?output=csv
- How obtained: Direct CSV link ("Directors of Charter Schools").
- Size: 24,746 bytes
- Data rows: 177
- Column count: 8
- Columns: `Number`, `Organization`, `Title`, `Name`, `Email`, `Phone`, `StateOrganizationId`, `Data Extracted`
