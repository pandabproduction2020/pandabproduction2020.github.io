# pandabproduction2020.github.io

The pandab studio website, served at the root of the domain:

- **Home page:** https://pandabproduction2020.github.io/
- **Policies:** https://pandabproduction2020.github.io/policy/capybaraflow/
- **app-ads.txt:** https://pandabproduction2020.github.io/app-ads.txt ← the file AdMob crawls

## Why the repo has this exact name

This is a GitHub **user-site** repo: a repo named `<username>.github.io` is the only
repo GitHub serves at the **domain root**. That matters because AdMob looks for
app-ads.txt at the root of the developer website domain, no matter which URL is in
the Play Store listing — and a normal project repo (e.g. `Home`) is only served
under `/<repo>/` paths, where AdMob never looks.

## Structure

```
index.html                         home page (studio site)
app-ads.txt                        AdMob authorized sellers (pub-3491303009731035)
img/                               icons & store badges
policy/
  capybaraflow/
    index.html                     Privacy Policy · Terms · Data deletion
    test-devices.json              UMP test device list (fetched by the app)
```

## Editing

Push to `main` — the site republishes in about a minute.

To add a new game: create `policy/<app-slug>/index.html` (copy `capybaraflow` as a
template) and add a card in `index.html`. If the AdMob publisher ID ever changes,
update `app-ads.txt`.
