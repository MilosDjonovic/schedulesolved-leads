# DC — state education directory sources

Agency: District of Columbia — OSSE (Office of the State Superintendent of Education) SLED School Directory; DC GIS (Office of the Chief Technology Officer) education layers

Download date: 2026-10-21

DC has no state file with principal emails. OSSE's SLED School Directory (Cloudflare-protected; exported in headless Chromium via its "Export To Excel File" button, generated client-side) gives official state school/LEA IDs, phone, charter status — **no names**. DC GIS layers (ArcGIS MapServer, each under the 1,000-record limit so one query per layer returns everything; `returnGeometry=false`): Charter Schools layer has `DIRECTOR` (school leader name) for SY 2026-2027; Public Schools (DCPS) and Independent (private) Schools layers have addresses/phones/websites only. DCPS principal names are only on dcps.dc.gov school pages (not collected).

## `DCGIS_Charter_Schools.json`

Public charter school campuses with DIRECTOR name, phone, website, LEA/school IDs.

- URL: https://maps2.dcgis.dc.gov/dcgis/rest/services/DCGIS_DATA/Education_WebMercator/MapServer/1/query?where=1%3D1&outFields=*&returnGeometry=false&f=json
- How obtained: ArcGIS REST query (single page; 149 features < maxRecordCount 1000).
- Size: 121,282 bytes
- Data rows: 149
- Column count: 31
- Columns: `NAME`, `ADDRESS`, `DIRECTOR`, `PHONE`, `AUTHORIZER`, `GRADES`, `ENROLLMENT`, `WEB_URL`, `AUTHORIZAT`, `MYSCHOOL`, `SCHOOL_YEA`, `LEA_NAME`, `LEA_ID`, `SCHOOL_NAM`, `SCHOOL_ID`, `SCHOOLCODE`, `GRADES_1`, `LATITUDE`, `LONGITUDE`, `FACILITY_ID`, `CLUSTER_`, `WARD`, `ZIPCODE`, `MAR_ID`, `XCOORD`, `YCOORD`, `SE_ANNO_CAD_DATA`, `GLOBALID`, `CREATED`, `EDITED`, `OBJECTID`

## `DCGIS_Public_Schools.json`

DCPS schools — address, phone, website, IDs. **No contacts.**

- URL: https://maps2.dcgis.dc.gov/dcgis/rest/services/DCGIS_DATA/Education_WebMercator/MapServer/5/query?where=1%3D1&outFields=*&returnGeometry=false&f=json
- How obtained: ArcGIS REST query (single page; 123 features).
- Size: 106,626 bytes
- Data rows: 123
- Column count: 34
- Columns: `NAME`, `ADDRESS`, `FACUSE`, `LEVEL_`, `STATUS`, `PHONE`, `TOTAL_STUD`, `SSL`, `GIS_ID`, `WEB_URL`, `BLDG_NUM`, `SCH_PROG`, `CAPITALGAINS`, `CAPACITY`, `YEAR_BUILT`, `SQUARE_FOOTAGE`, `POPULATION_PLAN`, `LONGITUDE`, `LATITUDE`, `SCHOOL_YEA`, `LEA_NAME`, `LEA_ID`, `SCHOOL_NAM`, `SCHOOL_ID`, `GRADES`, `MAR_ID`, `XCOORD`, `YCOORD`, `ZIPCODE`, `FACILITY_ID`, `GLOBALID`, `CREATED`, `EDITED`, `OBJECTID`

## `DCGIS_Independent_Schools.json`

Independent (private) schools — address, phone, website. **No contacts.**

- URL: https://maps2.dcgis.dc.gov/dcgis/rest/services/DCGIS_DATA/Education_WebMercator/MapServer/3/query?where=1%3D1&outFields=*&returnGeometry=false&f=json
- How obtained: ArcGIS REST query (single page; 80 features).
- Size: 35,397 bytes
- Data rows: 80
- Column count: 16
- Columns: `ID`, `NAME`, `ADDRESS`, `TELEPHONE`, `WEB_URL`, `GIS_ID`, `MAR_ID`, `XCOORD`, `YCOORD`, `LATITUDE`, `LONGITUDE`, `ZIPCODE`, `CREATED`, `EDITED`, `GLOBALID`, `OBJECTID`

## `OSSE_School_Directory-10_21_2026.xlsx`

OSSE LEA/School Directory — state IDs, phone, address, grades. **No names.**

- URL: https://sled.osse.dc.gov/vPage/SchoolDirectory/298/91189
- How obtained: Headless Chromium click on "Export To Excel File" (client-side export, download named "School Directory-10_21_2026.xlsx").
- Size: 21,001 bytes
- Sheet: Sheet1
- Data rows: 254
- Column count: 8
- Columns: `School Name`, `State School ID`, `LEA Name`, `LEA ID`, `Telephone Number`, `Charter Status`, `Address`, `Grades Served`
