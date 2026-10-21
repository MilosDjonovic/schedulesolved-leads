# MO — state education directory sources

Agency: Missouri Department of Elementary and Secondary Education (DESE) — School Directory (MCDS), Data Downloads

Download date: 2026-10-21

Both lists are SQL Server Reporting Services reports in the MCDS portal, linked from https://dese.mo.gov/school-directory/data-downloads. Access path (no login): the report URL first shows the DESE web-apps gateway; its "View Public Applications" button opens the report. In headless Chromium the report parameter was left at its default filter (County) with **Select All** ticked in the multi-value list (562 values), "View Report" was clicked, and the ReportViewer's own export (`$find('rvMCDS').exportReport('EXCELOPENXML')`, i.e. the Export → Excel menu) produced the files. Row 1 of each sheet is the report title, row 2 is the header (unmodified). Building list: principal name/salutation/title + `SCHEMAIL`; district list: superintendent (`SDLNAME`/`SDFNAME`/`SDSALUAT`) + `DIEMAIL`, board president and secretary names, URL. DESE also posts PDF directories ("Missouri School Directory by County/District") — not downloaded since the Excel reports carry the same data. No DESE private-school contact file found.

## `School_Building_List.xlsx`

Public school buildings with principal name, title, years of experience, school email, phone, enrollment.

- URL: https://apps.dese.mo.gov/MCDS/Reports/SSRS_Print.aspx?ReportId=9cebc711-eb02-48bd-ae0e-47f11d8ef9f4
- How obtained: Public SSRS report ("Building List"), all districts selected, Export → Excel (browser download "School Building List.xlsx").
- Size: 590,677 bytes
- Sheet: School Building List
- Data rows: 2,429
- Column count: 34
- Columns: `CTYDIST`, `DNAME`, `SCHNUM`, `SCHNAME`, `SCHADDR1`, `SCHADDR2`, `SCHCITY`, `SCHZIP`, `SCHLPHON`, `SCHLFAX`, `BGRADE`, `EGRADE`, `PRINLN`, `PRINFN`, `PRINMI`, `PRINSAL`, `PRINYREX`, `PRINTITL`, `SCHEMAIL`, `SCHTTEACH`, `SCHENRR`, `SCHENRNR`, `SCHTENR`, `DCOUNTY`, `DSUPAREA`, `MO HOUSE DISTRICTS`, `MO SENATE DISTRICTS`, `US CONGRESSIONAL DISTRICTS`, `ELEM SCHOOL`, `MIDDLE SCHOOL`, `JR HIGH SCHOOL`, `HIGH SCHOOL`, `AVTS`, `ALT SCHOOL`

## `School_District_List.xlsx`

Districts (incl. charter LEAs) with superintendent name + email, board president/secretary, phone, URL.

- URL: https://apps.dese.mo.gov/MCDS/Reports/SSRS_Print.aspx?ReportId=ee8cf509-bf32-455e-b49e-c366a23b37db
- How obtained: Public SSRS report ("District List"), all districts selected, Export → Excel (browser download "School District List.xlsx").
- Size: 295,786 bytes
- Sheet: School District List
- Data rows: 562
- Column count: 56
- Columns: `CTYDIST`, `ELEMDIST`, `DNAME`, `DADDRESS1`, `DADDRESS2`, `DCITY`, `DZIP`, `DCOUNTY`, `DSUPAREA`, `DPYC`, `DPYAV`, `DPYTATL`, `DPHONE`, `DFAX`, `DELEMSN`, `DELEMST`, `DELEMSRS`, `DELEMSNS`, `DELEMSTS`, `DMIDSSN`, `DMIDSST`, `DMIDSSRS`, `DMIDSSNS`, `DMIDSSTS`, `DJRSN`, `DJRST`, `DJRSRS`, `DJRSNS`, `DJRSTS`, `DHIGHSN`, `DHIGHST`, `DHIGHSRS`, `DHIGHSNS`, `DHIGHSTS`, `DTOTSCHL`, `DTOTTECH`, `DTOTRES`, `DTOTNRES`, `DTOTSTU`, `PRESTITL`, `PRESLN`, `PRESFN`, `PRESMI`, `SECTITL`, `SECLN`, `SECFN`, `SECMI`, `SDLNAME`, `SDFNAME`, `SDMINIT`, `SDSALUAT`, `DIEMAIL`, `URL`, `MO HOUSE DISTRICTS`, `MO SENATE DISTRICTS`, `US CONGRESSIONAL DISTRICTS`
