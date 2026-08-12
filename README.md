# Unidle — website

Landing, support, and privacy pages for the Unidle macOS app, served with
GitHub Pages. Static HTML and one stylesheet; no build step.

The app source lives in a separate repository.

## Pages

| Page | Purpose |
|---|---|
| `index.html` | Landing page |
| `privacy.html` | Privacy policy — required by App Store Connect |
| `support.html` | Support page — required by App Store Connect |

## Before submitting to the App Store

Replace `SUPPORT_EMAIL_PLACEHOLDER` in `privacy.html` and `support.html` with a
real, monitored address. Apple rejects submissions whose support contact does
not resolve.

```bash
grep -rn SUPPORT_EMAIL_PLACEHOLDER .
```

## Local preview

```bash
python3 -m http.server 8000
```
