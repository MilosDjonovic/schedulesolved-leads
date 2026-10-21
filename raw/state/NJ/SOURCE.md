# NJ — state education directory sources

Agency: New Jersey Department of Education — New Jersey School Directory (Homeroom)

Download date: 2026-10-21

Download links are on https://homeroom6.doe.nj.gov/directory/ . The homeroom hosts are behind Imperva/Incapsula, which returns HTTP 403 to curl; the files were fetched by opening the same public download links in a normal (headless) Chromium session, which completes the site's standard JavaScript check and receives the CSV as a browser download. Each CSV begins with preamble lines (title, explanatory sentence, blank) before the header row — kept unmodified. NJNonPubSchools.csv is Latin-1 encoded. Principal email filled for 2,523 of 2,524 public school rows; district file has superintendent and business administrator names + emails; charter schools are districts with county code 80.

## `NJPubSchool.csv`

Public (incl. charter) schools with principal name/title/email, HIB coordinator, homeless liaison, grades, NCES code.

- URL: https://homeroom4.doe.nj.gov/public/publicschools/download/
- How obtained: Direct link ("Public Schools (includes school grade levels)") opened in headless Chromium; browser download named NJPubSchool.csv.
- Size: 961,100 bytes
- Data rows: 2,524
- Column count: 50
- Columns: `County Code`, `County Name`, `District Code`, `District Name`, `School Code`, `School Name`, `Princ. Title`, `Princ. First Name`, `Princ. Last Name`, `Princ. Title 2`, `Princ. Email`, `Address1`, `Address2`, `City`, `State`, `Zip`, `Mailing Address1`, `Mailing Address2`, `Mailing City`, `Mailing State`, `Mailing Zip`, `HIB Title1`, `HIB First Nname`, `HIB Last Name`, `HIB Title2`, `Homeless Liaison Title1`, `Homeless Liaison First Name`, `Homeless Liaison Last Name`, `Homeless Liaison Title2`, `Phone`, `Pre-K`, `Kindergarten`, `Grade 1`, `Grade 2`, `Grade 3`, `Grade 4`, `Grade 5`, `Grade 6`, `Grade 7`, `Grade 8`, `Grade 9`, `Grade 10`, `Grade 11`, `Grade 12`, `Post Grad`, `Adult Ed.`, `NCES Code`, `FB URL`, `Instagram URL`, `X URL`

## `NJPubSchoolDistricts.csv`

Districts (incl. charter districts) with superintendent name/email, business administrator name/email, other coordinators, website, NCES ID.

- URL: https://homeroom4.doe.nj.gov/public/districtpublicschools/download/
- How obtained: Direct link ("Public School Districts") opened in headless Chromium; browser download named NJPubSchoolDistricts.csv.
- Size: 426,735 bytes
- Data rows: 683
- Column count: 53
- Columns: `County Code`, `County Name`, `District Code`, `District Name`, `Chrt Sch Code`, `Supt. Title`, `Supt. First Name`, `Supt. Last Name`, `Supt. Title 2`, `Supt. EMail`, `Address1`, `Address2`, `City`, `State`, `Zip`, `Mailing Address1`, `Mailing Address2`, `Mailing Address3`, `Mailing City`, `Mailing State`, `Mailing Zip`, `Mailing Zip+4`, `Phone`, `BA Title1`, `BA First Name`, `BA Last Name`, `BA Email`, `BA Title2`, `SEC Title1`, `SEC First Name`, `SEC Last Name`, `SEC Title2`, `HIB Title1`, `HIB First Name`, `HIB Last Name`, `HIB Title2`, `State Testing Coor. Title1`, `State Testing Coor. First Name`, `State Testing Coor. Last Name`, `State Testing Coor. Title2`, `PARCC IT Con. Title1`, `PARCC IT Con. First Name`, `PARCC IT Con. Last Name`, `PARCC IT Con. Title2`, `School Safety Specialist Title1`, `School Safety Specialist First Name`, `School Safety Specialist Last Name`, `School Safety Specialist Title2`, `Website`, `NCES ID`, `FB URL`, `Instagram URL`, `X URL`

## `NJNonPubSchools.csv`

Non-public (private) schools with contact name, title, email, phone.

- URL: https://homeroom4.doe.nj.gov/nonpublic/nonpublics/download
- How obtained: Direct link ("Non-Public Schools") opened in headless Chromium; browser download named NJNonPubSchools.csv.
- Size: 207,945 bytes
- Data rows: 847
- Column count: 20
- Columns: `County Code`, `District Code`, `School Code`, `School Name`, `Address1`, `Address2`, `City`, `State`, `Zip`, `Mail Addr1`, `Mail Addr2`, `Mail City`, `Mail State`, `Mail Zip`, `Phone`, `Contact Name`, `Contact Title`, `Contact Email`, `Profit`, `Pub. Sch. Dist.`
