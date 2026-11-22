# Jalandhar Cantt Booth Atlas (AC 37)

`index.html` is the booth dashboard for Jalandhar Cantt: booth map, street map, all booths, target booths,
constituency results and, for each booth, results, electors, families and the voter list.

The page is **password-locked**. It holds personal data from the electoral roll, so the whole page is encrypted
(AES-256-GCM, key from the password via PBKDF2) and opens only after the team password is entered. Ask the
campaign lead for the password. Never commit the password, the unlocked dashboard or the voter list workbook.

Open it from GitHub Pages or download `index.html` and open it in a recent Chrome, Edge, Firefox or Safari.
The map tiles need internet; everything else works offline.

To update: rebuild the dashboard, then run `lock_dashboard.py` (kept with the build scripts) with the same
password file, and replace `index.html`.
