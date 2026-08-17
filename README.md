# mahanbalooei.github.io

Personal academic website for Mahan Balooei — MSc Bioinformatics student, University of Bologna.

Built with [Astro](https://astro.build) using the [Astro Cactus](https://github.com/chrismwilliams/astro-theme-cactus) theme (MIT licensed, see `LICENSE`).

## Structure

- `src/pages/index.astro` — Home
- `src/pages/research.astro` — Research
- `src/pages/publications.astro` — Publications
- `src/pages/cv.astro` — CV
- `src/site.config.ts` — site title, description, nav links
- `public/cv/CV_Mahan_Balooei.pdf` — downloadable CV

## Commands

| Command             | Action                                      |
| :------------------- | :------------------------------------------- |
| `npm install`         | Install dependencies                        |
| `npm run dev`         | Start local dev server at `localhost:4321`  |
| `npm run build`       | Build the production site to `./dist/`      |
| `npm run preview`     | Preview the production build locally        |
| `npm run check`       | Run Astro + Biome checks                    |

## Deployment

Pushing to `main` triggers `.github/workflows/deploy.yml`, which builds the site and pushes the compiled output to the `gh-pages` branch (created automatically on first run). In the repository's **Settings → Pages**, the source must be set to **Deploy from a branch**, with branch `gh-pages` and folder `/ (root)`.

The `gh-pages` branch is generated content only — never edit it directly or commit source files to it. All source changes go on `main`.
