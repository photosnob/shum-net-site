# shum.net

A one-page placeholder (the "Quantum Neural Network" 3D animation), moved off the old Apache server to Cloudflare Workers, now with HTTPS. Every push to `main` deploys.

- The page is `public/index.html`, copied unchanged from the old server. It loads three.js and the Outfit font from public CDNs.
- Every address on the domain shows this page (`not_found_handling: "single-page-application"` in `wrangler.jsonc`).
- Email for @shum.net runs on Google Workspace and is set in Cloudflare DNS (MX records); this site doesn't touch it.

Cloudflare build settings: no build command, deploy command `npx wrangler deploy`.
