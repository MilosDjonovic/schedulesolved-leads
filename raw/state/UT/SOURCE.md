# UT — state education directory sources

Agency: Utah State Board of Education (USBE) — Schools Directory

Download date: 2026-10-21

The directory page builds the CSV in the browser (a `data:application/csv` link) when "Export to CSV file" is clicked; it was clicked in headless Chromium and the download saved ("USBE Schools Directory Export.csv"). Contains 1,220 public/charter and 298 private schools (243 rows have a Closed year). `Principal Name` + `Principal Email` (email filled on 1,417 rows; for some private schools the name is blank and only an email is given). No USBE superintendent export found.

## `USBE_Schools_Directory_Export.csv`

All schools (public, charter, private) with principal/director title, name and email.

- URL: https://www.schools.utah.gov/schoolsdirectory
- How obtained: Browser click on `#exportCSV` (client-side CSV export of the full directory table).
- Size: 483,616 bytes
- Data rows: 1,518
- Column count: 23
- Columns: `District/LEA`, `District #`, `School`, `School #`, `Private`, `Charter`, `T-I Prev.`, `T-I Curr.`, `Grades`, `Address`, `City`, `Zip`, `Map`, `Link`, `Stats`, `Phone`, `Fax`, `Chartered By`, `Opened`, `Closed`, `Principal/Director`, `Principal Name`, `Principal Email`
