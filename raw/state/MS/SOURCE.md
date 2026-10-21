# MS — state education directory sources

Agency: Mississippi Department of Education (MDE) — District Directory

Download date: 2026-10-21

> **Use restriction stated by MDE on the page:** "We respectfully request that individuals only use the email addresses below for official school business. The addresses should not be used for solicitations by vendors or bulk email campaigns." Review before using these addresses for sales outreach.

The directory exists only as an HTML page (updated 9/14/2026), with one entry per district / charter school / special state school / agricultural high school: superintendent name and title, mailing address, phone, fax, email, website (~143 unique email addresses). mdek12.org returns HTTP 403 to curl, so the page was opened in headless Chromium and its rendered HTML saved unmodified. No MDE school-level principal file or private-school contact file was found.

## `MDE_District_Directory_page.html`

District Directory (HTML page).

- URL: https://mdek12.org/dd/
- How obtained: Rendered page saved from headless Chromium (curl gets 403).
- Size: 115,719 bytes
- Rows: ~150 district/charter/state-school entries (143 unique emails).
- Fields per entry (HTML text, not columns): district name (county), superintendent name, title, mailing address, phone, fax, email, website.
