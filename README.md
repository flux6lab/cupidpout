# CupidPout public website

This repository contains the public static website for CupidPout, including:

- the product landing page;
- Privacy Policy and Terms of Use pages in English and Traditional Chinese;
- `app-ads.txt` for advertising verification.

The site is dependency-free and does not collect or process information through the website itself.

## Pages

- English homepage: `index.html`
- Traditional Chinese homepage: `zh-tw/index.html`
- Privacy Policy: `privacy.html` and `zh-tw/privacy.html`
- Terms of Use: `terms.html` and `zh-tw/terms.html`
- Advertising verification: `app-ads.txt`

## GitHub Pages

GitHub Pages should publish the `main` branch from the repository root. The public site URL is:

`https://flux6lab.github.io/cupidpout/`

The site contains only static HTML, CSS, and image assets. There are no build steps, server-side components, forms, or client-side scripts.

## AdMob verification

For AdMob verification, `app-ads.txt` must be available at the root of the public hostname. A project Pages URL such as:

`https://flux6lab.github.io/cupidpout/`

does not make the file available at `https://flux6lab.github.io/app-ads.txt`. Use a user or organization Pages site, or connect a custom domain, and serve the file at `https://your-domain.example/app-ads.txt`. Keep that root URL as the app’s marketing website and leave the file publicly accessible for verification.
