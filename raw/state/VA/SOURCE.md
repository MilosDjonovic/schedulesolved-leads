# VA — state education directory sources

Agency: Virginia Department of Education (VDOE) — Virginia School Directories

Download date: 2026-10-21

Landing page: https://www.doe.virginia.gov/about-vdoe/virginia-school-directories (doe.virginia.gov returns 403 to curl; links were read by rendering the page in headless Chromium). VDOE publishes **no email addresses** in its directories. School file: principal name only (plus school phone). Superintendents and other division staff (names, titles, phones) exist only as one HTML page per division; all 132 pages were fetched (0.5 s apart) and zipped unmodified. No VDOE private-school directory with contacts was found.

## `Public_School_report.csv`

All public schools with division, NCES school number, principal name, address, phone, fall membership.

- URL: https://www.va-doeapp.com/Download.aspx?n=School%20Listing
- How obtained: Direct link ("School List with Principal Contact Information (CSV)"). Server filename Public_School_report.csv (served as application/vnd.ms-excel but is CSV). Begins with 2 title lines before the header (kept).
- Size: 625,248 bytes
- Data rows: 2,988
- Column count: 19
- Columns: `Division Num`, `Division Name`, `NCES School Num`, `School Num`, `School Name`, `Low Grades`, `High Grades`, `Division Description`, `School Description`, `Grade Standard`, `Schedule`, `Principal`, `Address1`, `Address2`, `City`, `State`, `Zip`, `Phone Number`, `Fall Membership Schools`

## `division_staff_pages_html.zip`

Division staff listing pages (HTML). Each contains `Superintendent: <name> Phone: ... Website ... Street address ... Mailing address`, followed by a table of division staff (title, name, phone).

- URL: https://www.va-doeapp.com/StaffBySchoolDivisions.aspx?d=<division>&w=true
- How obtained: Paged: the 132 division IDs were taken from the links on https://www.doe.virginia.gov/about-vdoe/virginia-school-directories/virginia-public-school-division-staff-listing-by-division ; each page saved as division_<id>.html and zipped.
- Size: 1,438,692 bytes
- Files in zip: 132 HTML pages (one per school division); 132/132 contain a Superintendent line.
- Columns: n/a (HTML). Fields shown per page: division name, superintendent name, division phone, fax, website, street/mailing address; staff rows: title, name, phone.
