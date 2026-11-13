# Kickbox Bootcamp website

The public website for the Kickbox Bootcamp Android kickboxing-workout app: landing page, FAQ, legal pages, account deletion page, beta sign-up, sign-in/email link pages and referral links that open the app.

| Item | Value |
|---|---|
| Status | Live; last commit 2026-02-28 |
| Repo | github.com/Alia-Rose/kickboxbootcamp-site (public) |
| Stack | Static HTML pages with inline CSS and JS; GitHub Pages (Jekyll, `_config.yml` only to publish `.well-known`); Supabase for app sign-in and the beta sign-up function; Cloudflare Turnstile on the beta form |
| Run / build | No build. Preview: open the HTML files in a browser. Deploy: push to `main` (GitHub Pages publishes automatically) |
| Live at | https://kickboxbootcamp.smallempirestudios.com |
| App | Android, package `com.kickboxbootcamp` on Google Play (closed testing) |

## Pages
| Page | Purpose |
|---|---|
| `index.html` | Landing page with Google Play link |
| `faq.html` | App FAQ (workouts, voice coaching, history, accounts) |
| `privacy-policy.html`, `terms-of-service.html` | Legal (Last Updated: January 6, 2026) |
| `delete-account.html` | Account and data deletion instructions (Google Play requirement, inferred) |
| `beta.html` | Beta tester sign-up form (hidden from search via `robots.txt`) |
| `auth/` | Pages that email links land on (confirm email, magic link, password reset, email change), then hand off to the app |
| `404.html` | Handles referral links `/ref/CODE`: opens the app, or Google Play if not installed |
| `.well-known/assetlinks.json` | Lets Android open this site's links directly in the app and share saved logins |
| `assets/` | Logo and banners for beta invite emails |
| `index-mockup.html` | Old landing page draft, not linked from the site |

## Notes go here when
- FAQ answers change because an app feature changed
- Privacy policy, terms or account deletion wording needs updating
- The beta sign-up form or invite emails change
- Sign-in, email confirmation, password reset or referral links break
- The app leaves closed testing and the landing page needs a public launch update
