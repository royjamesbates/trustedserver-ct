# Trusted Server CT Corporation Landing Page

CT Corporation service landing page for Trusted Server (Roy Bates, SPS #1383), Plantation, FL. Email-first intake, no portal.

## Live URLs

- Primary: https://trustedserver.us/ct
- GitHub Pages: https://ct.trustedserversop.com (after DNS is pointed)

## DNS setup (GoDaddy)

1. In GoDaddy Domain Manager, open **trustedserversop.com** → Manage → DNS.
2. Add a **CNAME** record:
   - Host: `ct`
   - Points to: `royjamesbates.github.io`
   - TTL: 1 hour (or default)
3. Save. DNS propagation takes a few minutes to a few hours.
4. Verify: `https://ct.trustedserversop.com` should serve this page.

## GitHub Pages

This repo is published via GitHub Pages from the `main` branch. The `CNAME` file in the repo root tells Pages to serve the custom domain.

## Contact

- Email: bates@trustedserver.us
- Phone: 954-515-6450
- SPS #1383, Broward County, FL
