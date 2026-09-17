# MR-CAPSULES-CONTENT

Dedicated static content and cover repository for **MR-CAPSULES**.

## Structure
- `content/`: HTML-based CBT study modules and lectures organized by Semester and Block.
- `cover/`: Card cover images and animated GIFs used by the Coverflow carousel.

## Deployment Options
This repository is designed to be deployed to a high-speed Edge CDN:
1. **Cloudflare Pages**: Connect this repository to Cloudflare Pages. Built-in `_headers` ensures cross-origin access and iframe embedding without `X-Frame-Options` restrictions.
2. **Vercel**: Deploy as a static site using `vercel.json`.
3. **GitHub Pages / Raw GitHub / jsDelivr**: Direct access via `https://raw.githubusercontent.com/<owner>/MR-CAPSULES-CONTENT/main/...`.

## Integration with MR-CAPSULES
Set the following environment variable in the main MR-CAPSULES project:
``
GITHUB_CONTENT_REPO=MR-CAPSULES-CONTENT
CONTENT_CDN=https://your-cdn-subdomain.pages.dev
``
