# VERISEFY API Proxy

Routes `api.idbima.com` → VERISEFY backend with HTTPS termination via Vercel.

## Setup

1. Deploy this repo to Vercel
2. Add `api.idbima.com` as a custom domain in the Vercel project settings
3. Add the DNS record at your domain registrar:
   - Type: CNAME
   - Name: api
   - Value: cname.vercel-dns.com

All requests to `https://api.idbima.com/*` are proxied to the backend.
