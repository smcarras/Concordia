# Concordia Strategic website

Static site: five HTML pages, one stylesheet and two images. No build step.

- `index.html` – Home
- `capabilities.html`, `market-entry.html`, `about.html`, `contact.html`
- `assets/styles.css`, `assets/warsaw-hero.jpg`, `assets/lykke-logo.png`
- `_headers` – caching and security headers for Cloudflare Pages

Every page carries `<meta name="robots" content="noindex">`. Remove that line from each page when the site should appear in search results.

## Deploy on Cloudflare Pages

1. Push this folder to a GitHub repository.
2. In the Cloudflare dashboard open Workers & Pages, create a Pages project and connect the repository.
3. Framework preset: None. Build command: leave empty. Build output directory: `/`.
4. Deploy. Add the custom domain under the project's Custom domains tab.
