# My Logo Works - Ready Project (SEO + Netlify CMS)

This ZIP contains a ready-to-deploy static site with Netlify CMS admin files and basic SEO improvements.
Unzip into your project folder and push to GitHub. Then deploy to Netlify (or overwrite your current repo).

## What is included
- index.html (SEO meta tags, OG tags, JSON-LD)
- style.css, script.js
- admin/index.html (Netlify CMS entry)
- admin/config.yml (Netlify CMS config - uses git-gateway)
- images/ (empty - used for uploads)
- posts/ (empty - used for posts)
- sitemap.xml, robots.txt
- README.md (this file)

## Steps to use (simple)
1. Unzip and **replace** files with your real site content (if needed).
2. Commit & push to your GitHub repository:
   ```bash
   git add .
   git commit -m "Add SEO + Netlify CMS admin"
   git push origin main
   ```
3. In Netlify, connect your repo (if not yet connected) and deploy.
4. Enable **Identity** and **Git Gateway** in Netlify site settings (Identity -> Services -> Git Gateway).
5. Invite yourself via Identity -> Users -> Invite user (use your GitHub email). Accept invite.
6. Visit `https://<your-netlify-site>.netlify.app/admin/` to log in and use the CMS.

## Submit site to Google
1. Go to Google Search Console: https://search.google.com/search-console
2. Add a property for `https://your-site.netlify.app/` (or your custom domain).
3. Verify ownership (Netlify or HTML verification). Then request indexing of the homepage URL.
4. You can also submit the sitemap: `https://your-site.netlify.app/sitemap.xml`

## Notes & tips
- Remove `meta name="robots" content="noindex"` if present to allow indexing.
- Keep admin/ blocked in `robots.txt` so search engines do not index the CMS UI.
- For best SEO: write unique page titles, meta descriptions, and publish content (posts/pages).
