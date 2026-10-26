# M10 — Spencer Conway

A standalone Quarto website project. The original portfolio at the repository root is unchanged.

## Preview and render

Open this folder in RStudio or Positron, then run in the Terminal:

```bash
quarto preview
quarto render
```

Requires Quarto 1.8 or later. No R or Python packages are needed to render this version.

## Add the required personal photo

Put your photo at `assets/spencer.jpg`. In `index.qmd`, replace the entire `.profile-placeholder` fenced div with:

```markdown
![Spencer Conway](assets/spencer.jpg){width=220px}
```

Remove the draft status note in `submission.qmd` only once the photo and live links have been verified.

## Publish using the existing Pages configuration

Render M10, then copy the contents of `M10/_site/` to the repository's `m10/` directory. Commit source and rendered output. Existing GitHub Pages branch publishing must serve the repository root. If Pages is not enabled, go to Settings > Pages and choose main / (root). The intended URL is listed in submission.qmd.

## Data

`data/instagram-demo.csv` is invented practice data, not client results or Case 31. Dashboard cards, SVG chart, and summary table are static summaries of this CSV. If the data changes, recalculate all three before rendering. Sample engagement rate is 638 / 10000 * 100 = 6.38%.

## Structure

- Four navbar pages: index.qmd, cep.qmd, styling.qmd, listings.qmd
- Actual dashboard: dashboard.qmd
- Listing entries: projects/*.qmd
- Theme: theme.scss and styles.css
- Submission: submission.qmd and its rendered HTML

References are linked on the relevant pages to the official Quarto documentation.
