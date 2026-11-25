# shizrah_dev

Development environment site, hosted on GitHub Pages.

**Live (dev):** https://shizrah.github.io/shizrah_dev/

## Layout

```
.
├── index.html              # Landing page
├── 404.html                # Custom not-found page
├── assets/css/style.css    # Shared styles
├── robots.txt              # Blocks indexing (dev environment)
├── .nojekyll               # Serve files as-is, skip Jekyll
└── .github/workflows/
    └── pages.yml           # Deploys to Pages on push to main
```

## Deploying

Every push to `main` triggers the **Deploy to GitHub Pages** workflow. Check progress under the repo's **Actions** tab.

One-time setup: **Settings → Pages → Build and deployment → Source: GitHub Actions**.

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Notes

- Pages and `robots.txt` set `noindex` so this dev site stays out of search results. Remove both before turning this into a production site.
- To use a custom domain, add a `CNAME` file containing the domain and configure DNS per GitHub's custom-domain docs.

## License

MIT — see [LICENSE](LICENSE).
