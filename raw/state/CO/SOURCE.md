# CO — state education directory sources

Agency: Colorado Department of Education (CDE) — Directory data (cedar.cde.state.co.us) and Superintendents directory

Download date: 2026-10-21

The CDE "downloadable mailing labels" page (https://www.cde.state.co.us/cdereval/downloadablemailinglabels, now redirecting to https://ed.cde.state.co.us/cdereval/related) offers address/phone files with **no person names or emails** (district file has only an `Email Domain`). Superintendent contacts are published by CDE as a public Smartsheet view titled "(NEW) Public District/BOCES Contact List (View Only)", linked as "View the directory" from https://ed.cde.state.co.us/superintendents . The Smartsheet view has no export, so the sheet's data payload (the `fa_loadContainer` AJAX response the viewer loads, Smartsheet's JavaScript/array format, with cells as `'<Column name>',0,'<value>'` sequences) was captured in headless Chromium and saved byte-for-byte as a .txt file. It contains ~209 unique email addresses (superintendent and other district/BOCES contacts), titles, district codes, addresses.

## `CDE_Public_District_BOCES_Contact_List_smartsheet_fa_loadContainer.txt`

Superintendent / district & BOCES contact list (raw Smartsheet payload).

- URL: https://app.smartsheet.com/b/publish?EQBCT=0addfc75c63b4c0293fcb2f05340b724
- How obtained: Opened the published Smartsheet in headless Chromium; saved the body of the viewer's POST `https://app.smartsheet.com/b/publish?formName=ajax&formAction=fa_loadContainer` response.
- Size: 1,390,275 bytes
- Columns seen in payload: School District, Dist. Size (PK-12), County, Mailing Address, City, State, Zip, Title, (name and email columns), Congressional District, district code, setting.
- Rows: 201 district/BOCES records (count of `School District` cells).

## `District_Addresses-en.xlsx`

Districts/BOCES — address, phone, fax, email domain. **No names/emails.**

- URL: https://cedar.cde.state.co.us/edulibdir/District%20Addresses-en.xlsx
- How obtained: Direct link ("District Public Contact Information (XLS)")
- Size: 67,659 bytes
- Sheet: District Addresses
- Data rows: 181
- Column count: 16
- Columns: `District Code`, `Organization Type`, `District Name`, `Congressional District`, `County Name`, `County Code`, `Physical Address`, `City`, `State`, `Zipcode`, `Mailing Address`, `Phone`, `Fax`, `Email Domain`, `District Size`, `District Setting`

## `School_Addresses-en.xlsx`

Public schools — address, phone, grades. **No contacts.**

- URL: https://cedar.cde.state.co.us/edulibdir/School%20Addresses-en.xlsx
- How obtained: Direct link ("Public Schools Contact Information (XLS)")
- Size: 215,081 bytes
- Sheet: School Addresses
- Data rows: 1,885
- Column count: 14
- Columns: `District Code`, `District Name`, `School Code`, `Charter Y/N`, `School Name`, `Physical Address`, `City`, `State`, `Zip Code`, `Mailing Address`, `Phone`, `Low grade`, `High grade`, `Congressional District`

## `Non-Public_School_Addresses-en.xlsx`

Non-public (private) schools — address, phone. **No contacts.**

- URL: https://cedar.cde.state.co.us/edulibdir/Non-Public%20School%20Addresses-en.xlsx
- How obtained: Direct link ("Non Public Schools Contact Information (XLS)")
- Size: 112,183 bytes
- Sheet: Non-Public School Addresses
- Data rows: 666
- Column count: 15
- Columns: `District Code`, `District Name`, `School Code`, `School Name`, `Physical Address`, `City`, `State`, `Zip Code`, `Mailing Address`, `Phone`, `Low grade`, `High grade`, `Congressional District`, `Recently Active`, `24-25 SY NEW CODE`
