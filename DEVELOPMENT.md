# Development

Plain HTML and CSS, with no build step or JavaScript required. The site uses the After Hours layout, Blue Hour palette, Sora headings, and DM Sans body text.

## Local preview

From the repository root:

```sh
python3 -m http.server 4173 --bind 127.0.0.1
```

Open [the local preview](http://127.0.0.1:4173/).

## Editing

- `index.html` contains the page content and metadata.
- `styles.css` contains the layout, responsive rules, and theme.
- `shir.jpg` is the portrait; photographer credit is retained in the README.
- Fonts load from Google Fonts, with local fallback fonts.
- After changing `styles.css`, update its `?v=` value in `index.html` so browsers load the new version.

## Deployment

GitHub Pages publishes the `main` branch from the repository root. `.nojekyll` keeps this a plain static site. Pushes to `main` trigger deployment automatically.

Current URL: [shir22.github.io/askshir-website](https://shir22.github.io/askshir-website/).

The intended custom domain is `askshir.com`; DNS configuration is still pending. The README links to the custom domain. Once connected, enable HTTPS for it.
