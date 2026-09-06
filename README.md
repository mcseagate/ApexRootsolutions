# Apex Root Solutions — published product documents

The privacy policies, terms of use and support pages for Apex Root Solutions LLC
applications, served by GitHub Pages.

They are public because both app stores require a privacy policy at a URL a
reviewer can open, and a link that 404s fails review.

## Berean Scroll

A Bible reading, study, teaching and community app.

| Page | URL |
| --- | --- |
| Privacy Policy | https://mcseagate.github.io/ApexRootsolutions/berean-scroll/privacy/ |
| Terms of Use | https://mcseagate.github.io/ApexRootsolutions/berean-scroll/terms/ |
| Support | https://mcseagate.github.io/ApexRootsolutions/berean-scroll/support/ |

The same values are configured in the app itself, in `Config/Release.xcconfig`
(iOS) and `app/build.gradle.kts` (Android). Changing a URL here means changing it
there in the same breath: a released build carries whatever it was built with,
for as long as it stays installed on a phone.

## Layout

Each product owns a directory, because each collects different things and
promises different things about them. A second product adds a sibling directory
rather than editing anything here.

```
index.html                       the list above
style.css                        shared by every page
berean-scroll/
  index.html  privacy/  terms/  support/
```

## Publishing

Settings → Pages → **Deploy from a branch** → `main` → `/ (root)`.

`.nojekyll` is present so the files are served exactly as written rather than
being run through Jekyll.

## Before submitting to either store

Berean Scroll's Terms of Use section 15 (Governing law) contains two deliberate
placeholders, marked in red on the page: the state in which Apex Root Solutions
LLC is organised, and the county and state for venue. They were left blank rather
than guessed. Both documents should be reviewed by counsel before release.
