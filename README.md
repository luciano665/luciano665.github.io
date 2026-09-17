# Luciano Maldonado — Research Website

A personal academic website built with [Hugo](https://gohugo.io/) and the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme. PaperMod is vendored in `themes/PaperMod`, so the project works after download without initializing a Git submodule.

## Edit the website

Most updates require only Markdown or YAML:

- `data/home.yaml` — homepage introduction, research questions, interests, and updates
- `content/publications/` — one Markdown file per publication or research project
- `content/projects/` — one Markdown file per software project
- `data/career.yaml` — experience and education
- `content/blog/` — blog posts
- `hugo.yaml` — site URL, navigation, metadata, and profile links
- `assets/css/extended/custom.css` — custom visual design layered over PaperMod
- `layouts/` — custom homepage, research cards, project cards, and career timeline
- `static/files/Luciano-Maldonado-CV.pdf` — downloadable CV

Use an existing Markdown file as the template when adding another publication, project, or blog post. Hugo builds list, detail, search, RSS, and archive pages automatically.

## Run locally

Install Hugo Extended 0.146 or newer. Version 0.166.0 is used for the included deployment configuration.

```bash
hugo server -D
```

Open `http://localhost:1313`.

## Build

Before publishing, set `baseURL` in `hugo.yaml` to your real domain. Then run:

```bash
hugo --gc --minify
```

The generated website is written to `dist/`.

## Publish

### GitHub Pages

1. Create a GitHub repository and push this entire project.
2. In **Settings → Pages**, select **GitHub Actions** as the source.
3. The included `.github/workflows/hugo.yml` builds and publishes the site after every push to `main`.

### Netlify

Import the repository into Netlify. The included `netlify.toml` uses Hugo 0.166.0, runs `hugo --gc --minify`, and publishes `dist`.

### Any static host

Run the build locally and upload the contents of `dist/` to the host's public directory.

## Theme

The light/dark theme toggle, responsive foundation, search, metadata, and content conventions come from PaperMod. The single-column profile homepage, monogram, navigation controls, research cards, project list, career timeline, typography, spacing, and color adjustments are custom for this site.
