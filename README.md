# ShelfBee Website

Marketing site and legal pages for [shelfbee.app](https://shelfbee.app), served via GitHub Pages.

## Structure

```
docs/
├── index.html       # Landing page
├── privacy.html     # Privacy policy (required for App Store)
├── terms.html       # Terms of use
├── support.html     # Support & FAQ page
└── CNAME            # Custom domain: shelfbee.app
```

## GitHub Pages setup

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to: `Deploy from a branch` → `main` → `/docs`
4. GitHub will provision HTTPS automatically via Let's Encrypt

## Custom domain DNS (Namecheap / your registrar)

Add these A records pointing to GitHub Pages:

| Type | Host | Value |
|------|------|-------|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | yourusername.github.io |

DNS propagation takes up to 48 hours. GitHub Pages will show a green checkmark once SSL is provisioned.

## App Store Connect URLs to set

- **Privacy policy URL:** `https://shelfbee.app/privacy`
- **Support URL:** `https://shelfbee.app/support`
- **Marketing URL:** `https://shelfbee.app`

## To update

Edit files in `docs/`, commit, and push to `main`. GitHub Pages deploys within ~60 seconds.
