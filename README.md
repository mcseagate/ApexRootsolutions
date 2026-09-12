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

## LifeOS Finance

A personal finance planning app. Works with no account; bank and card linking
is a separate, optional feature, off by default and read-only through Plaid.

| Page | URL |
| --- | --- |
| Privacy Policy | https://mcseagate.github.io/ApexRootsolutions/lifeos-finance/privacy/ |
| Terms of Use | https://mcseagate.github.io/ApexRootsolutions/lifeos-finance/terms/ |
| Support | https://mcseagate.github.io/ApexRootsolutions/lifeos-finance/support/ |

## AscendFlare

An app-marketing platform (web). Analyses public store listings, drafts
recommendations, ads and posts, and publishes only after per-item approval.

| Page | URL |
| --- | --- |
| Privacy Policy | https://mcseagate.github.io/ApexRootsolutions/ascendflare/privacy/ |
| Terms of Service | https://mcseagate.github.io/ApexRootsolutions/ascendflare/terms/ |
| Support | https://mcseagate.github.io/ApexRootsolutions/ascendflare/support/ |

The application also serves the same documents itself at `/legal/privacy` and
`/legal/terms` (source: `src/app/legal/` in the `martintel` repository, with the
operator facts in `src/lib/legal.ts`). The two copies must say the same thing:
edit the app first, then mirror here in the same commit. The DPA and
sub-processor list live only in the app.

## Layout

Each product owns a directory, because each collects different things and
promises different things about them. A second product adds a sibling directory
rather than editing anything here.

```
index.html                       the list above
style.css                        shared by every page
berean-scroll/
  index.html  privacy/  terms/  support/
lifeos-finance/
  index.html  privacy/  terms/  support/
```

## Publishing

Settings → Pages → **Deploy from a branch** → `main` → `/ (root)`.

`.nojekyll` is present so the files are served exactly as written rather than
being run through Jekyll.

## Company details — use these verbatim in every product

These belong in every application's privacy policy and terms, unchanged. They are
recorded here so a new product is not drafted from memory or from a template that
has drifted.

> Apex Root Solutions LLC, a limited liability company organised under the laws
> of the State of Delaware, with its registered office in Wilmington, New Castle
> County, Delaware, and its principal place of business in Cedar Hill, Dallas
> County, Texas.

**Governing law and venue.** Texas law, with exclusive venue in the state and
federal courts of Dallas County, Texas — subject to the two standard exceptions:
either party may seek injunctive relief anywhere competent, and mandatory local
consumer law is never displaced.

Texas rather than Delaware is deliberate. Delaware is the state of organisation
and governs the company's internal affairs; the agreement with a user is governed
where the company actually does business and where a dispute would be heard.

**Contact.** support@apsoluts.com

## Before submitting to either store

Both documents should be reviewed by counsel before release. They are written to
be accurate about what each app does, but accuracy about behaviour is not the
same as legal sufficiency in every jurisdiction a store ships to.
