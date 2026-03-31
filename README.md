# SeveranceClarity.com

Plain-English severance agreement analysis service.

## DNS Setup (Namecheap → GitHub Pages)

Add these records in Namecheap → Advanced DNS:

| Type   | Host | Value                  |
|--------|------|------------------------|
| A      | @    | 185.199.108.153        |
| A      | @    | 185.199.109.153        |
| A      | @    | 185.199.110.153        |
| A      | @    | 185.199.111.153        |
| CNAME  | www  | jaredleiman.github.io  |

## Stripe Payment Links
Replace in index.html:
- `STRIPE_QUICK_LINK` → Quick Explainer $147 payment link
- `STRIPE_FULL_LINK`  → Full Breakdown $347 payment link

## Stack
- Hosting: GitHub Pages
- Domain: Namecheap
- Payments: Stripe
- File Intake: Jotform
- Email: Resend (hello@severanceclarity.com via ImprovMX forwarding)
- Automation: Zapier
- Orders: Notion
- API: Cloudflare Worker → Anthropic Claude
