# ahmettarikbiyiklioglu.github.io

Source of the personal academic website at https://ahmettarikbiyiklioglu.github.io.
GitHub Pages builds it with Jekyll on every push to `main`; nothing needs to be installed locally.

## How to update

| What | Where |
| --- | --- |
| Add a paper, report or talk | `_data/publications.yml` (new entries go at the top of the relevant list) |
| Change the bio or contact details | `index.md` |
| Change research descriptions | `research.md` |
| Change courses | `teaching.md` |
| Replace the CV | overwrite `assets/pdf/CV_Biyiklioglu.pdf` and update the month in `cv.md` and `index.md` |
| Replace the photo | overwrite `assets/img/biyiklioglu.jpg` (4:5 portrait, about 720 by 900 pixels) |
| Change colors | the six values at the top of `assets/css/style.css` |
| Add or reorder a menu item | `nav` in `_config.yml` |

Edit a file on github.com with the pencil icon and commit; the site rebuilds in about a minute.

## Local preview (optional)

```
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.
