# WV — state education directory sources

Agency: West Virginia Department of Education (WVDE) — WV Education Directory (wveis.k12.wv.us)

Download date: 2026-10-21

The statewide CSV ("Download all addresses in a comma delimited format" → download.php → "Click here to download") lists every board office and school with address, phone, fax, URL, grades — **no principal names or emails**. Principal names appear only on per-school pages of the directory (not paged). County superintendents (55 counties + special LEAs) are published as an Excel file with name, email, phone. The non-public school listing page on wvde.us exposed no downloadable file.

## `County-Superintendent-List.xlsx`

County superintendents with email, phone, fax, address.

- URL: https://wveis.k12.wv.us/school-directory/County-Superintendent-List.xlsx
- How obtained: Direct link ("Superintendent listing") on https://wveis.k12.wv.us/school-directory/
- Size: 25,109 bytes
- Sheet: Sheet1
- Data rows: 74
- Column count: 10
- Columns: `County`, `Sp Dial *Ext`, `Phone # (304)`, `Fax #`, `Email Address`, `Title`, `Superintendent`, `Address`, `City`, `Zip Code`

## `WV_Education_Directory.csv`

All board offices and schools — addresses/phones only, **no contacts**.

- URL: https://wveis.k12.wv.us/school-directory/download.php?dl
- How obtained: Direct link ("Click here to download" on https://wveis.k12.wv.us/school-directory/download.php). Server filename school_list.csv.
- Size: 149,483 bytes
- Data rows: 907
- Column count: 13
- Columns: `district_id`, `"location_id"`, `"type"`, `county`, `name`, `address`, `city`, `zip`, `zip4`, `phone`, `fax`, `url`, `grades`
