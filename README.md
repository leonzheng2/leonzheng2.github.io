# leonzheng2.github.io

Source of Léon Zheng's academic website, https://leonzheng2.github.io, built with Jekyll on GitHub Pages from the [AcademicPages](https://github.com/academicpages/academicpages.github.io) template (a fork of [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/), MIT licensed, see `LICENSE`).

## Where the content lives

- `_pages/about.md`: home page, including the News list
- `_pages/publications.md`, `_pages/talks.md`, `_pages/code.md`: the other top-level pages
- `_data/navigation.yml`: top navigation links
- `_thesis/`, `_journal/`, `_conference/`, `_preprint/`: one Markdown file per publication (front matter only)
- `_talks/`: one Markdown file per talk
- `files/`: slides, posters and images linked from the pages
- `images/profile.jpg`: avatar; other files in `images/` are favicons
- `_config.yml`: site settings and author profile

## Run locally

```
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.
