# Kieni’s Finest website

Static site for GitHub Pages. Everything sits in this one folder next to `index.html`.

## Before you publish
Replace the placeholder address with your real site URL (for example `https://yourname.github.io/repo` or your own domain). Run this once in the folder:

    sed -i 's|https://YOUR-SITE-URL|https://your-real-address|g' index.html sitemap.xml robots.txt llms.txt

On a Mac use `sed -i '' ...`. No trailing slash.

## Publish on GitHub Pages
1. Upload every file in this folder to the root of your repository.
2. Settings > Pages > Deploy from a branch > `main` / root.
3. Submit `sitemap.xml` in Google Search Console and Bing Webmaster Tools.

Note: the 404 page uses root-relative paths, so it works best on a custom domain or a user site. On a project site, change `/styles.css` and `/` in `404.html` to include the repo name.
