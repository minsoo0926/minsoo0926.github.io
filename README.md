# Personal website

## Publications

Add BibTeX entries to `_bibliography/publications.bib`. All entries automatically
appear in the homepage's Publication section when Jekyll builds, grouped under
year headings with the newest year first.
There is no separate list to update.

For example (replace these sample values with a real publication):

```bibtex
@inproceedings{ha2026example,
  author    = {Ha, Minsoo and Doe, Jane},
  title     = {Your Paper Title},
  booktitle = {Conference Name},
  year      = {2026},
  note      = {Accepted for presentation},
  pdf       = {/assets/papers/your-paper.pdf}
}
```

Use a unique citation key for each entry. `note` and `pdf` are optional.
Use `journal` for journal articles and `booktitle` for conference papers.
Authors are separated with `and`. The `note` field appears after the publication
details. The `url` field supplies a clickable **Link**, with `doi` as a fallback;
the raw URL is not displayed. The optional `pdf` field adds a PDF link.

Authors display in full given-name–family-name order. The name configured in
`scholar.author_name` in `_config.yml` is bolded in the formatted citation.
Keep standard BibTeX author syntax (`Ha, Minsoo`) in the source file.

## Local preview

```sh
bundle install
bundle exec jekyll serve
```

## GitHub Pages

This site uses Jekyll-Scholar, which requires a custom GitHub Actions build.
In the repository's **Settings → Pages → Build and deployment**, choose
**GitHub Actions** as the source. The included workflow rebuilds and deploys
the site on pushes to the default branch, including changes to the BibTeX file.
