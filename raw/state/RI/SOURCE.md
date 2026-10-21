# RI — state education directory sources

Agency: Rhode Island Department of Education (RIDE) — RIDE Data Center Schools Directory

Download date: 2026-10-21

RIDE publishes no directory file. The old eRIDE Schools Directory (eride.ri.gov/SchoolsDirectory) now redirects to a 404 behind Cloudflare. The RIDE Data Center Schools Directory (https://datacenter.ride.ri.gov/Directory, Cloudflare-protected, so headless Chromium was used) has one page per LEA and per school with LEA/school codes, NCES code, address, phone, website and **Contact(s)** with name, title and role (e.g. Superintendent, Principal) — **no emails**. The full listing (70 LEAs, 1,203 school/program entries incl. inactive, home-school, higher-ed and other entity types) was read from the Index page's DataTable (`Index_all_rows.html`, saved) and every LEADetail/SchoolDetail page was fetched (~1 page/sec) and zipped unmodified. Contact names appear on 615 school pages. Nonpublic: RIDE's 'Approved Nonpublic Schools Directory' is a Google Sheet that requires sign-in (HTTP 401) — not collected; nonpublic school pages that exist in the Data Center are included in the zip.

## `RIDE_DataCenter_Directory_pages_html.zip`

Rendered HTML of the RIDE Data Center directory (Index, Index_all_rows, 70 LEA pages, 1,203 school pages).

- URL: https://datacenter.ride.ri.gov/Directory/LEADetail?orgid=<id> and https://datacenter.ride.ri.gov/Directory/SchoolDetail?orgid=<id>
- How obtained: Paged in headless Chromium: Index → full DataTable row list → each LEA and school detail page saved as rendered HTML, zipped.
- Size: 4,394,528 bytes
- Files in zip: Index.html, Index_all_rows.html, LEA_<orgid>.html (70), School_<orgid>.html (1,203).
- Columns: n/a (HTML). Fields per page: name, LEA/school code, type, NCES code, grade span, status, addresses, phone, fax, website, Contact(s): name, Title, Role(s); LEA pages list their schools.
