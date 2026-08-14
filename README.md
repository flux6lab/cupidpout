# CupidPout GitHub Pages site

This folder is a dependency-free static site for the public CupidPout page, Privacy Policy, Terms of Use, and AdMob publisher verification.

## Publish with GitHub Pages

1. Push this repository to GitHub.
2. In **Settings → Pages**, choose **Deploy from a branch**.
3. Select the branch you want to publish (usually `main`) and choose the `/docs` folder.
4. Save. GitHub will show the public Pages URL after deployment.

For a GitHub **project** Pages site, the public URLs will be:

- `https://<github-username>.github.io/<repository>/`
- `https://<github-username>.github.io/<repository>/privacy.html`
- `https://<github-username>.github.io/<repository>/terms.html`
- `https://<github-username>.github.io/<repository>/zh-tw/`
- `https://<github-username>.github.io/<repository>/zh-tw/privacy.html`
- `https://<github-username>.github.io/<repository>/zh-tw/terms.html`
- `https://<github-username>.github.io/<repository>/app-ads.txt`

This deployment is suitable for the public ASO, Privacy Policy, and Terms links.

## Required setup for AdMob verification

AdMob ignores the path portion of the marketing website URL and crawls only the hostname’s root: `https://<hostname>/app-ads.txt`. Therefore, a project Pages URL such as `https://<github-username>.github.io/<repository>/` **cannot** be used by itself for AdMob verification; its `app-ads.txt` is one path too deep.

Choose one of these deployment options for the same files in this folder:

1. **Recommended, no custom domain:** publish the contents of `docs/` to a GitHub user/organization Pages repository named `<github-username>.github.io`. The file then resolves at `https://<github-username>.github.io/app-ads.txt`.
2. **Custom domain:** connect a custom domain to this GitHub Pages project. Ensure that `https://<your-domain>/app-ads.txt` serves this exact file.

Put that root site URL in the App Store listing’s **Marketing URL**. After the app is publicly listed, allow AdMob at least 24 hours to crawl and verify the file.
