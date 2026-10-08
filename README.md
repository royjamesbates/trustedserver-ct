# Trusted Server CT Corporation Landing Page

CT Corporation service landing page for Trusted Server (Roy Bates, SPS #1383), Plantation FL. Email-first intake, no portal.

## Live URLs

- Primary: https://trustedserver.us/ct
- GitHub Pages: https://ct.trustedserversop.com (after DNS is pointed)

## Publishing (GitHub Pages)

1. Repo Settings > Pages > Source: Deploy from branch `main`, folder `/ (root)`.
2. Pages will serve `index.html` automatically.

## DNS (GoDaddy) — required for ct.trustedserversop.com

In GoDaddy Domain Manager for trustedserversop.com, add these records:

| Type | Name | Value |
|------|------|-------|
| A | ct | 185.199.108.153 |
| A | ct | 185.199.109.153 |
| A | ct | 185.199.110.153 |
| A | ct | 185.199.111.153 |

- TTL: 1 hour (or default)
- Do NOT add a CNAME for `ct` — GitHub Pages requires A records at the apex subdomain when using a custom domain on a subdomain.
- After saving, DNS propagation takes 5 minutes to a few hours.
- Verify: `nslookup ct.trustedserversop.com` should return the four 185.199.x.x addresses.

## Notes

- The page's canonical URL and structured data point to https://trustedserver.us/ct — update those in index.html if you want the .sop domain to be the canonical.
- Contact: bates@trustedserver.us · 954-515-6450
