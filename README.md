# Alesha Designs — GitHub Pages Website

This is a static website package for Alesha Designs.

## Files included

- `index.html` — public landing page
- `start.html` — audit-start page routing clients to the secure intake form
- `privacy.html` — starter privacy notice
- `terms.html` — starter service terms
- `styles.css` — full site styling
- `favicon.svg` — simple AD browser icon
- `CNAME` — custom domain setting for GitHub Pages

## Intended business system

This website is the public-facing site only.

Use:

- GitHub Pages for `aleshadesigns.com`
- Fillout for secure intake, file uploads, and Stripe payment
- Google Drive / Google Workspace for client file storage
- Shopify only as the domain registrar until you transfer the domain elsewhere

## Button routing

The current intake button points to:

```text
https://forms.aleshadesigns.com/start
```

Set that subdomain inside Fillout after your Fillout form is created.

## GitHub Pages setup

1. Create a public GitHub repository named `alesha-designs-site`.
2. Upload all files from this folder into the root of the repository.
3. Go to the repository's **Settings → Pages**.
4. Set source to deploy from the main branch and root folder.
5. Under custom domain, enter:

```text
aleshadesigns.com
```

6. Enable HTTPS after DNS is recognized.

## Shopify DNS setup

Inside Shopify:

Settings → Domains → aleshadesigns.com → DNS settings

For apex domain, add GitHub Pages A records:

```text
@  A  185.199.108.153
@  A  185.199.109.153
@  A  185.199.110.153
@  A  185.199.111.153
```

For www:

```text
www  CNAME  creativefaestudio.github.io
```

If GitHub Pages gives a different default domain, use that value instead.

DNS changes can take up to 24 hours.

## Legal note

The privacy and terms pages are starter operating copy, not legal advice. Have final policy language reviewed before launch.
