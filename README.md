# Astro Portfolio

This is a personal portfolio website built with [Astro](https://astro.build/) and designed for deployment on GitHub Pages.

## Features
- Modern, responsive design
- About, Projects, and Contact sections
- Easy deployment to GitHub Pages

## Getting Started

1. Install dependencies:
   ```bash
   npm install
   ```
2. Start the development server:
   ```bash
   npm run dev
   ```
3. Build for production:
   ```bash
   npm run build
   ```
4. Deploy to GitHub Pages (see the deployment section below).

## Deployment

This project is configured for easy deployment to GitHub Pages using GitHub Actions.

### Automatic Deployment with GitHub Actions
- Deployment is triggered automatically whenever you push to the `main` branch.
- The workflow in `.github/workflows/deploy.yml` builds your site and publishes it to GitHub Pages.
- No manual changes to `astro.config.mjs` are needed; the workflow sets the `site` and `base` values using environment variables at build time.

**To deploy:**
1. Commit and push your changes to the `main` branch:
   ```bash
   git add .
   git commit -m "Your message"
   git push origin main
   ```
2. GitHub Actions will build and deploy your site automatically. You can monitor progress in the Actions tab of your repository.

### Manual Deployment (optional)
If you want to deploy manually, you can build your site and push the `dist/` folder to the `gh-pages` branch yourself.

For more details, see the [Astro GitHub Pages guide](https://docs.astro.build/en/guides/deploy/github/).

---
