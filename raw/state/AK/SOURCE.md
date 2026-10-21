# AK — state education directory sources

Agency: Alaska Department of Education & Early Development (DEED) — Alaska Public Schools Database (DOE_Rolodex)

Download date: 2026-10-21

DEED publishes no directory file (the 'Districts and Schools Information' page only offers PDFs of IDs/active schools without contacts). Two sources were saved: (1) the **Alaska School District Contact Information** page, rendered in headless Chromium (contact data is filled in client-side), which lists every district with address, phone, fax, district email (56 unique, often the superintendent's own address) and website, but no names; (2) the Public Schools Database pages: Districts list → 49 `SchoolsList?districtId=` pages → 440 `SchoolDetails/<id>` pages (each redirects to `/compass/ParentPortal/SchoolProfile?SchoolID=<id>`), fetched with curl at 1 request every 1–2 s and zipped unmodified. School profile pages show **Principal** name (391 of 440) and School Board President; no emails. No DEED private-school contact file.

## `DEED_District_Contact_Information_page.html`

All school districts with address, phone, fax, email, website (HTML).

- URL: https://education.alaska.gov/DOE_Rolodex/SchoolCalendar/DistrictAndSchoolInfo/DistrictDetails
- How obtained: Rendered page saved from headless Chromium.
- Size: 43,750 bytes
- Rows: one block per district (~54); 56 unique email addresses.
- Columns: n/a (HTML). Fields: district name, address, telephone, fax, email, website.

## `DEED_Public_Schools_Database_pages_html.zip`

Raw HTML of the school database (1 districts list, 49 district school lists, 440 school profiles).

- URL: https://education.alaska.gov/DOE_Rolodex/SchoolCalendar/Home/SchoolDetails/<id> (→ https://education.alaska.gov/compass/ParentPortal/SchoolProfile?SchoolID=<id>)
- How obtained: Paged with curl (redirects followed): Districts.html → SchoolsList_<district>.html → SchoolDetails_<school>.html; zipped.
- Size: 5,685,644 bytes
- Files in zip: Districts.html, SchoolsList_<id>.html (49), SchoolDetails_<id>.html (440).
- Columns: n/a (HTML). Fields per school profile: school name, grades, enrollment, address, phone, website, district, Principal, School Type, School Board President.
