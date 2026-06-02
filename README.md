# PsychAD Consortium website

Source for the PsychAD Consortium website, published at <https://psych-ad.org/>.

Maintained by Donghoon Lee ([@hoondy](https://github.com/hoondy)).

## About

The PsychAD Consortium seeks to deepen our understanding of neuropsychiatric symptoms (NPS) in Alzheimer's disease (AD), related dementias (ADRD), and serious mental illnesses (SMIs) by exploring shared and distinct biological pathways underlying these disorders. By combining epidemiological data with advanced multi-omic and systems biology approaches, PsychAD aims to uncover biomarkers and therapeutic targets that can improve diagnosis, prognosis, and treatment of NPS. The work is supported by the National Institute on Aging via [PAR-23-207](https://grants.nih.gov/grants/guide/pa-files/PAR-23-207.html) and RFA-MH-19-510.

## Site structure

A static [Jekyll](https://jekyllrb.com/) site deployed with GitHub Pages.

| Path | Purpose |
| --- | --- |
| `_pages/` | Page content: home, Research, Data, People, Grants, 404 |
| `_data/navigation.yml` | Top navigation menu |
| `_includes/` | Custom `<head>` snippets, footer, and reveal script |
| `assets/css/main.scss` | Custom design system (brand palette, hero, cards, tables) |
| `assets/images/` | Logos, figures, icons, and journal marks |
| `_config.yml` | Global site configuration |

The visual design lives in [`assets/css/main.scss`](assets/css/main.scss), which defines the brand color palette (derived from the network-brain logo), typography, hero, stat band, cards, and table styling.

## Local development

GitHub Pages builds the site automatically on push to `master`. To preview changes locally you need **Ruby 3.x** (the `github-pages` gem does not support Ruby 2.x or 4.x):

```bash
bundle install
bundle exec jekyll serve
```

Then open <http://localhost:4000/>.

> Note: when viewing a built page directly from `_site/` via a `file://` URL the styles will appear broken, because the site uses absolute (`/assets/...`) paths. Always preview through `jekyll serve` (or any local web server) instead.

## Useful links

- [Jekyll documentation](https://jekyllrb.com/docs/)
- [Configuring GitHub Pages with Jekyll](https://jekyllrb.com/docs/github-pages/)
