# truecom-web-landing

Landing page for [truecom.ai](https://truecom.ai) — the agent commerce gateway.

## What this is

Static HTML/CSS landing page for Truecom, deployed via GitHub Pages at `truecom.ai`.
All content is drawn from the codebase fact-file and positioning research — no fabricated stats.

## Deploy

GitHub Pages serves from `main` branch root (`/`). The `CNAME` file points GitHub Pages
to the `truecom.ai` apex domain.

To update the page: edit `index.html`, commit, and push to `main`. Pages redeploys automatically.

## DNS

To make `truecom.ai` resolve to GitHub Pages, add these A records at your DNS registrar:

```
truecom.ai.   A   185.199.108.153
truecom.ai.   A   185.199.109.153
truecom.ai.   A   185.199.110.153
truecom.ai.   A   185.199.111.153
```

Also add a `www` CNAME pointing to `relayOne.github.io` if you want the www subdomain to work.

GitHub may take a few minutes to issue the TLS certificate after DNS propagates.

## Source

- Gateway: `github.com/RelayOne/TrustPlane`
- SDK (TS): `@truecom/sdk` on npm
- SDK (Go): `github.com/RelayOne/truecom-sdk-go`
- SDK (Python): `truecom` on PyPI
