# HI — state education directory sources

Agency: Hawaii State Department of Education (HIDOE) — School Directory (hawaiipublicschools.org)

Download date: 2026-10-21

Hawaii is a single statewide district (the State Superintendent heads HIDOE). HIDOE publishes no directory file; each school has a page under https://hawaiipublicschools.org/schools/<slug>/ showing **Principal name**, island, complex area, grades, address, phone, fax, website (no emails). The list of school pages was taken from the site's public WordPress REST endpoint (`/wp-json/wp/v2/schools`, 258 entries, saved as JSON), then all 258 pages were fetched one per second and zipped unmodified. Public charter schools are under the separate State Public Charter School Commission and are not in this list. No HIDOE private-school contact file.

## `HIDOE_school_pages_html.zip`

HTML school pages (258), each with a 'Principal:' line.

- URL: https://hawaiipublicschools.org/schools/<slug>/
- How obtained: Paged: 258 school page URLs from the REST index, fetched with curl at 1 request/second; saved as <slug>.html and zipped.
- Size: 7,391,755 bytes
- Files in zip: 258 HTML pages; 258/258 contain 'Principal:'.
- Columns: n/a (HTML). Fields per page: school name, Principal, Island, Complex Area, Division/level, Grade Levels, address, phone, fax, website.

## `HIDOE_wp-json_schools_index.json`

Index of school pages (id, slug, link, title, modified).

- URL: https://hawaiipublicschools.org/wp-json/wp/v2/schools?per_page=100&page=1..3&_fields=id,slug,link,title,modified
- How obtained: WordPress REST API, 3 pages of 100, combined into one JSON array.
- Size: 53,948 bytes
- Rows: 258
- Columns: `id`, `slug`, `link`, `title`, `modified`
