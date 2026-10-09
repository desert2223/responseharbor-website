# ResponseHarbor website (starter)

Minimal, no-build static website intended for staging review and customer discovery. Includes:

- `/index.html`: responsive marketing landing page (English)
- `/demo/`: scripted interactive English lead-recovery walkthrough
- `/demo/de/`: scripted German lead-recovery walkthrough
- `/assets/`: brand icons and horizontal logo

**Important:** The demo is scripted, not a working SMS, AI, telephony, calendar or CRM integration. No real form submissions are processed. Contact CTA uses a `mailto:` link.

## Preview locally

Run `python -m http.server 8000` in this folder and visit `http://localhost:8000/`.

## Deploy

Works as a static HTML project on Cloudflare Pages / Workers static assets. If using Pages Git integration, connect the GitHub repo and set the production branch to `main`, build output directory to the repository root (or `/` if requested), and no build command required.

**Domain safety:** `responseharbor.eu` DNS is currently at Namecheap with Google Workspace mail records (MX/SPF/DKIM/DMARC). Do not change nameservers before copying and validating these records at the new DNS host. Deploy to a temporary `pages.dev` preview first, then connect the domain.

## Before public launch

1. Verify logo display at 48px and on mobile.
2. Check and polish legal/business identification information relevant to actual commercial activity.
3. Test contact email and all navigation links.
4. Confirm language/copy and the pilot offer.
