# clip-for-google-tasks-website

Public-facing static site for the **Clip for Google Tasks** Chrome extension.

Hosted via GitHub Pages, served from the custom domain:
<https://clip.ozeo.io/>

(Default Pages URL fallback: <https://jsozeo.github.io/clip-for-google-tasks-website/>)

The custom domain is configured via:

- A `CNAME` file at the repo root containing `clip.ozeo.io`
- A DNS `CNAME` record `clip.ozeo.io → jsozeo.github.io` at the `ozeo.io` registrar
- `Settings → Pages → Custom domain` set to `clip.ozeo.io` with `Enforce HTTPS` enabled

The domain `ozeo.io` is verified in Google Search Console (Domain property,
TXT record), which lets it be used as the OAuth consent screen homepage / privacy /
terms URL in Google Cloud Console.

## Pages

- `index.html` — Marketing homepage
- `privacy.html` — Privacy policy (referenced by the Chrome Web Store listing and the Google OAuth consent screen)
- `terms.html` — Terms of service (referenced by the Google OAuth consent screen)
- `style.css` — Shared styles (auto dark/light via `prefers-color-scheme`)
- `.nojekyll` — Disables Jekyll processing on GitHub Pages so files are served as-is

## Local preview

Any static-file server works. Example:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Related repo

- Extension source: <https://github.com/jsozeo/clip-for-google-tasks> (private)
