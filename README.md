# URL Shortener

A simple static URL shortener/redirector that runs entirely on GitHub Pages.

## How It Works

Uses GitHub Pages' 404.html feature for client-side redirects. When someone visits a short link, the 404 page intercepts it and redirects to the configured URL.

## Adding Redirects

Edit `redirects.json` and add your short code and target URL:

```json
{
  "redirects": {
    "shortcode": "https://your-long-url.com"
  }
}
```

Commit and push - GitHub Pages updates automatically.

## Deployment

1. Push to GitHub
2. Enable GitHub Pages in Settings → Pages
3. Set source to main branch, root folder

Done. Your short links will be at `https://username.github.io/repo/shortcode`
