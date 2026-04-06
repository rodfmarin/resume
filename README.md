# Resume Site

This folder contains a static resume site intended for GitHub Pages or any basic static file host.

## Files

- `index.html`: resume landing page
- `styles.css`: site styles
- `assets/rodrigo-marin-resume.txt`: downloadable text resume
- `assets/README.md`: asset naming guidance for PDF and DOCX files
- `.github/workflows/deploy-pages.yml`: GitHub Pages deployment workflow
- `.nojekyll`: disables Jekyll processing on GitHub Pages

## Publish setup

This repo is set up to deploy with GitHub Actions when you push to `main`.

### Recommended repository options

If you want the site at a repository-specific Pages URL:

- Create a repo such as `resume`
- Push this folder to that repo
- Your site URL will be similar to `https://rodfmarin.github.io/resume/` after Pages is enabled

If you want the site at your root GitHub Pages URL:

- Use a repo named `rodfmarin.github.io`
- Put these files at the repository root
- Your site URL will be `https://rodfmarin.github.io/`

## GitHub Pages steps

1. Add `rodrigo-marin-resume.pdf` and `rodrigo-marin-resume.docx` to the `assets` folder.
2. Create a GitHub repository and push this project to the `main` branch.
3. In GitHub, open repository Settings, then Pages.
4. Under Build and deployment, set Source to `GitHub Actions`.
5. Push to `main` and let the workflow deploy the site.

## Notes

- The current site links to your GitHub profile at `https://github.com/rodfmarin`.
- If you publish this to a non-root Pages path like `/resume/`, the current relative links will still work.
- If you later add a custom domain, GitHub Pages can support that with a `CNAME` file.