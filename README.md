# clip-for-google-tasks-website

Public-facing static site for the **Clip for Google Tasks** Chrome extension.

Hosted via GitHub Pages at:
<https://jsozeo.github.io/clip-for-google-tasks-website/>

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
