# Vastu Weave Architects

Static, mobile-first architectural portfolio website for Vastu Weave Architects.

## Stack

- HTML5, CSS, Tailwind CDN, and vanilla JavaScript
- Lottie/dotLottie CDN players
- Decap CMS with Netlify Identity and Git Gateway
- Web3Forms contact delivery
- Netlify free-tier deployment

## Local preview

Serve this folder instead of opening `index.html` with `file://`:

```bash
python -m http.server 8000
```

Open `http://localhost:8000`. Alternatively use `npx serve .`.

## Logo and media

The supplied logo animation belongs at `/public/lottie/logo-intro.json`. Project photographs belong under `/public/images/projects/`; Lottie walkthroughs belong under `/public/lottie/projects/`. Update paths in `content/projects.json`.

## Netlify

1. Push this repository to GitHub.
2. In Netlify, choose **Add new site → Import an existing project**.
3. Select the GitHub repository.
4. Leave the build command empty.
5. Set the publish directory to `.`.
6. Deploy.

Enable Netlify Identity and Git Gateway, set registration to Invite only, and invite the owner. The CMS is available at `/admin.html`.

## Contact form

The Web3Forms access key is in `content/settings.json`. Web3Forms sends submissions to `Vastuweavearchitects@gmail.com`. Confirm a real test submission after deployment. Replace the supplied Maps URL with a Google Maps iframe embed URL if the map does not render.

## SEO

The initial canonical URL is `https://vastuweave.netlify.app`. Update `content/settings.json`, `sitemap.xml`, and social metadata when a custom domain is connected. Submit the sitemap in Google Search Console.

## Before launch

Replace all `[EDIT: ...]` placeholders, add real project assets, complete the legal pages, test contact delivery, test `/admin.html`, and run Lighthouse on mobile.
