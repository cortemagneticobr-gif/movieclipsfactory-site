# movieclipsfactory-site

The official public page for **MovieClipsFactory**, a personal desktop
application. This repository holds only the site: the application's source
lives elsewhere and is not published here.

The site exists because the developer portals of TikTok and Meta require a
public website, a Terms of Service URL and a Privacy Policy URL before an
application can be registered at all.

Live at <https://cortemagneticobr-gif.github.io/movieclipsfactory-site/>

## What is here

```
index.html            home - what the application is, and what it is not
privacy.html          Privacy Policy
terms.html            Terms of Service
data-deletion.html    Data deletion and data handling
pt/                   the same four pages in Portuguese
assets/               icon and stylesheet
tiktok*.txt           platform ownership-verification files (see below)
.nojekyll             so GitHub Pages serves files and folders verbatim
```

## Platform ownership-verification files

TikTok verifies that you own a URL by generating a file and asking you to serve
it at the root of the site. Two are already here, and that is not a mistake:
**TikTok issues a separate signature per configuration**, so the production app
and each sandbox get their own file. Both are verified.

To add another, drop the file in the root of this repository and commit; it is
then served at the site root. `.nojekyll` is present precisely so GitHub Pages
does not filter such files out. Do not rename them and do not edit their
contents - the check compares them byte for byte.
## Editing

The content of both languages is generated from one source, `gerar.py`, because
the real risk of a bilingual legal site is one version saying something the
other does not. That script is kept with the application's source rather than
here; if you edit a page by hand, edit its counterpart in the other language in
the same commit.

## Honesty note

The home page states, in the product's own words, that MovieClipsFactory is a
personal tool for its operator's own accounts, and quotes the line from
TikTok's Content Sharing Guidelines that lists that use case as not acceptable
for audited access. That is deliberate. The application uses the unaudited
draft path (`video.upload`) instead, where the person finishes the post inside
the TikTok app.

If you edit this site, do not remove that paragraph in order to pass a review.
A page that describes this application as a hosted multi-user service would be
false, and passing a review by being something else is not passing it.
