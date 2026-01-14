# Kickbox Bootcamp Website

Website and deep link handler for the Kickbox Bootcamp Android app.

## Live URL

https://kickboxbootcamp.smallempirestudios.com

## Structure

```
/
├── index.html              → Landing page & referral link handler
├── privacy-policy.html     → Privacy Policy
├── terms-of-service.html   → Terms of Service
├── CNAME                   → Custom domain config
└── .well-known/
    └── assetlinks.json     → Android App Links verification
```

## URLs

| Resource | URL |
|----------|-----|
| Landing Page | https://kickboxbootcamp.smallempirestudios.com |
| Privacy Policy | https://kickboxbootcamp.smallempirestudios.com/privacy-policy.html |
| Terms of Service | https://kickboxbootcamp.smallempirestudios.com/terms-of-service.html |
| Referral Links | https://kickboxbootcamp.smallempirestudios.com/ref/CODE |

## Setup

### DNS Configuration

Add this CNAME record at your domain registrar:

```
Type: CNAME
Name: kickboxbootcamp
Value: alia-rose.github.io
```

### GitHub Pages

1. Go to repo Settings → Pages
2. Source: Deploy from branch `main`
3. Custom domain: `kickboxbootcamp.smallempirestudios.com`
4. Enable "Enforce HTTPS"

### Android App Links

Replace `REPLACE_WITH_YOUR_SHA256_FINGERPRINT` in `.well-known/assetlinks.json` with your app's SHA-256 certificate fingerprint from Google Play Console.

Find it at: Google Play Console → Your App → Setup → App signing → SHA-256 certificate fingerprint
