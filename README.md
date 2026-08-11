# From Big Time Series Forecasting to Foundation Models for Structured Data

The landing page for the VLDB 2026 tutorial, live at <https://vldb-fmsd-tutorial.github.io/>.

Presented by **Xiyuan Zhang** (Amazon Web Services) and **Yuyang "Bernie" Wang** (NTT DATA AIVista).
Co-authored with Abdul Fatir Ansari, Christos Faloutsos and George Karypis.

Tutorial paper: PVLDB 19(12): 4939–4943, 2026 · [doi:10.14778/3827998.3828154](https://doi.org/10.14778/3827998.3828154)

VLDB 2026 · 31 August – 4 September · The Westin Boston Seaport District. The session slot is
announced with the full program.

## Repository layout

This is a single static page with no build step, no JavaScript, and no third-party requests —
it renders offline and serves real HTML to crawlers and link-preview bots.

```
index.html          the page (layout in one <style> block in the head)
_ds/modernist-*/    the Modernist design system; styles.css is the only stylesheet
assets/fonts/       Archivo, self-hosted as two variable-font subsets
.nojekyll           required: Jekyll would otherwise skip the _ds/ directory
```

To preview locally:

```sh
python3 -m http.server 8000
```

GitHub Pages serves the `master` branch directly. There is no CI: committing to `master`
publishes the site.

## History

Before this, the repository held a copy of the [al-folio](https://github.com/alshedivat/al-folio)
Jekyll site used for the ICLR 2026 TSALM workshop, kept as a starting point. That state is
preserved on the `archive/tsalm-jekyll` branch and in the commit history; the now-unused
`gh-pages` branch still holds its last build.

## Licensing

The page content and markup are © the tutorial authors. Archivo is used under the
SIL Open Font License 1.1 — see `assets/fonts/OFL.txt`.
