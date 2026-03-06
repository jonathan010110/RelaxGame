# RelaxGame - SvelteKit on GitHub Pages

This project is configured as a fully static SvelteKit app using `@sveltejs/adapter-static`.

## Stack

- Node.js
- Vite
- SvelteKit
- Static adapter (`@sveltejs/adapter-static`)

## Static Build Configuration

`svelte.config.js` is configured to:

- output pages to `build`
- output assets to `build`
- use `fallback: 'index.html'` for SPA routing
- use `paths.base = '/RelaxGame'` in production for GitHub Pages

## Scripts

```json
"scripts": {
  "dev": "vite dev",
  "build": "vite build",
  "preview": "vite preview"
}
```

## Local Development

```bash
npm install
npm run dev
```

## Build Locally

```bash
npm run build
```

Build output is written to `build/`.

## GitHub Actions Deployment

Workflow file: `.github/workflows/deploy.yml`

The workflow:

- triggers on push to `main`
- installs dependencies
- runs `npm run build`
- uploads `build/`
- deploys to GitHub Pages

## Enable Pages in GitHub

1. Open repository settings on GitHub.
2. Go to `Pages`.
3. Set `Source` to `GitHub Actions`.

After that, each push to `main` deploys automatically.

Expected site URL:

`https://jonathan010110.github.io/RelaxGame/`
