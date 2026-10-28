# Contributing

Thanks for helping keep this index useful! Pull requests that add, fix or update entries are welcome.

## What to add
- **Open-source code is required** (unless the entry is a survey/review paper or a toolbox with documentation). Entries without a public implementation will be removed.
- Prefer methods with a peer-reviewed or arXiv paper and a maintained, publicly accessible repository.
- Put the entry in the most specific existing section. If none fits, propose a new section in the PR description.

## Row format
Use the table schema of the section you are editing and keep columns aligned with the neighbouring rows.

```
|Name|[Authors. "Title." Venue (Year).](paper-link)|[Python](code-link)|
```

- Label the code link with its language (`Python`, `R`, `Julia`, ...) or `Code` if mixed.
- Prefer stable links: DOI or arXiv abstract pages over publisher PDFs, and `https://` everywhere.
- Use `NA` only for a column that genuinely has no value (e.g. a toolbox without a paper).
- Use consistent casing: NeurIPS, arXiv, ICML, ICLR.

## Before opening a PR
- Check that every new link resolves. The `Links` GitHub Action runs [lychee](https://github.com/lycheeverse/lychee) on every PR.
- Do not leave commented-out rows in the README; git history keeps removed entries.
- Keep one entry per pull request commit where practical, with a short description of why it belongs.
