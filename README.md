# HC Olympia — Data

GitHub Pages site: https://meusini.github.io/OlympiaData/

| Page | What | Built by |
|---|---|---|
| `index.html` | Clubs en teams (census): password-locked. Only AES-256-GCM ciphertext is in this repo. | `HockeyCensus/build_page.js` on the box, password typed by hand, never stored |
| `statistiek.html` | Win/draw/loss statistics for Olympia and club comparison. Public results data. | `HockeyField/build_data_site.js`, daily via `refresh-local.ps1` (OlympiaCalendar Refresh task) |

Do not edit `statistiek.html` here: it is a copy of OlympiaCalendar's `index.html` with
`data-site="data"`, overwritten every morning. Change the Statistiek code in
`HockeyField/index.html`.

Schedule, results, teams and standings: https://meusini.github.io/OlympiaCalendar/
