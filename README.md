# SQE Career Lab

This repository is now a Jekyll site for a software quality engineering blog aimed at QA/SDET job seekers. It includes public pages, starter blog posts, and the business assets that support the coaching funnel.

## Repository layout

- `_config.yml`: Jekyll site configuration
- `_layouts/`: shared Jekyll layouts
- `_posts/`: starter blog content
- `assets/css/`: site styling
- `assets/lead-magnet/`: downloadable lead magnet copy
- `assets/email/`: welcome and nurture email sequence
- `assets/content/`: blog content calendar and post briefs
- `assets/outreach/`: promotion and outreach templates
- `assets/offers/`: pricing and offer definitions
- `.github/workflows/deploy-pages.yml`: GitHub Pages deployment workflow

## Run locally with Docker

This project is configured to run with the official `jekyll/jekyll:4` Docker image.

### Option 1: Docker Compose

```bash
docker compose up
```

Then open `http://localhost:4000/sqe-blog/`.

### Option 2: Direct Docker command

```bash
docker run --rm \
  -p 4000:4000 \
  -p 35729:35729 \
  -v "$PWD:/srv/jekyll" \
  jekyll/jekyll:4 \
  jekyll serve --livereload --host 0.0.0.0 --port 4000 --force_polling
```

## GitHub Pages deployment

The GitHub Actions workflow builds the Jekyll site and deploys the generated `_site` output to GitHub Pages.

1. Open the repository `Settings` -> `Pages`
2. Set `Build and deployment` to `GitHub Actions`
3. Push to `main` and GitHub will rebuild the site automatically

## Suggested next steps

1. Update contact details, booking link, and email signup destination in the Jekyll pages.
2. Replace placeholder testimonials with real beta client feedback.
3. Add the remaining posts from the content calendar into `_posts/`.
4. Turn the lead magnet markdown into a PDF and attach it to your email platform.
