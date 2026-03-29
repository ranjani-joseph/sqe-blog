# SQE Blog Revenue Kit

This starter project turns the revenue plan into a simple static site and a set of operating assets for a software quality engineering blog aimed at QA/SDET job seekers.

## Repository layout

- `site/`: public-facing website pages that GitHub Pages will publish
- `assets/lead-magnet/`: downloadable lead magnet copy
- `assets/email/`: welcome and nurture email sequence
- `assets/content/`: blog content calendar and post briefs
- `assets/outreach/`: promotion and outreach templates
- `assets/offers/`: pricing and offer definitions
- `.github/workflows/deploy-pages.yml`: GitHub Pages deployment workflow

## GitHub Pages deployment

This repo is set up to deploy the `site/` folder with GitHub Actions.

1. Create a new GitHub repository and push this project to the `main` branch.
2. In GitHub, open `Settings` -> `Pages`.
3. Under `Build and deployment`, choose `GitHub Actions`.
4. Push future updates to `main` and GitHub will redeploy automatically.

The published homepage will come from `site/index.html`.

## Suggested next steps

1. Update contact details, booking link, and email signup destination in the HTML files.
2. Turn the lead magnet markdown into a PDF and link it from the signup flow.
3. Write and publish the first two posts from the content calendar.
4. Start outreach using the included templates and collect the first beta testimonials.
