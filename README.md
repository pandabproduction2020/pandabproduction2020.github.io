# pandabproduction2020.github.io

Domain-root repo for https://pandabproduction2020.github.io/

**Why this repo exists:** AdMob crawls `app-ads.txt` at the **root of the developer
website domain** — `https://pandabproduction2020.github.io/app-ads.txt` — no matter
which URL is listed in the Play Store listing. Project sites (like the `Home` repo)
are only served under `/Home/`, so this user-site repo is the only thing that can
serve the root path.

Contents:

- `app-ads.txt` — the file AdMob reads (publisher `pub-3491303009731035`)
- `index.html` — redirects visitors to the studio site at `/Home/`

Do not delete this repo while AdMob ads are running.
If the publisher ID changes, update this file **and** `Home/app-ads.txt`.
