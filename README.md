# Asif Islam — Personal Website

A minimal personal site built with [Astro](https://astro.build/). The homepage presents my resume in HTML, with links to GitHub and LinkedIn and a downloadable PDF copy. The site also includes a Markdown and MDX blog at `/blog`.

## Development

Requirements: Node.js `>=22.23.4` and npm.

```sh
npm install
npx astro dev --background
```

The development site runs at <http://localhost:4321>. Manage the background server with:

```sh
npx astro dev status
npx astro dev logs
npx astro dev stop
```

Build the static site into `dist/` or preview a production build locally:

```sh
npm run build
npm run preview
```

## Project structure

```text
public/Asif_Islam_Resume.pdf   Downloadable resume
src/pages/index.astro          Resume homepage
src/pages/blog/                 Blog index and post routes
src/content/blog/               Markdown and MDX posts
src/layouts/                    Shared blog post layout
src/styles/                     Global styles
```

Add blog posts as Markdown or MDX files in `src/content/blog/`. Astro's file-based routing exposes pages under `src/pages/` as site routes.
