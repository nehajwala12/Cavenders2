# Cavender's — Complete Company Diagnostic · CreditSwan (edition v2.0, 29 Sep 2026)

Static site, ready to deploy on Vercel as-is. No build step, no framework, no password.

    index.html    the full packet, open access (nav, 16 tabs, 254 exhibits, charts and motion engine inline)
    favicon.svg   swan mark
    favicon.png   swan mark, 512 px, for Apple touch icon
    robots.txt    disallows search-engine indexing
    vercel.json   clean URLs plus noindex / nosniff / referrer headers

## Access

The password gate and encryption have been removed. Anyone with the link can open the packet directly.
Search engines are still asked not to index it (robots.txt, the robots meta tag and the X-Robots-Tag header).
To make it fully public and indexable, delete robots.txt, the `X-Robots-Tag` header in vercel.json and the
`<meta name="robots">` tag in index.html.

## Deploy

Option A — dashboard: vercel.com/new → drag this folder onto the page (or pick it in the file dialog) → Deploy.
Option B — CLI, from inside this folder:

    npx vercel --prod

Either way the packet is served at the project URL (and any custom domain you attach). If Vercel's own
Deployment Protection is on for the project, turn it off in project settings so the URL is open to everyone.

Fonts load from Google Fonts (Cormorant Garamond, Manrope, IBM Plex Mono); the page falls back to Georgia,
system sans and Menlo if that host is blocked.

## Deep links

Every tab, section and exhibit has a stable address, e.g. `/#proposal`, `/#proposal/proposal-timeline`,
`/#financial/ex-12-10`. Tab ids: overview · about · market · competition · brand · customers · employees ·
stores · ecommerce · technology · merchandising · financial · proposal · strategy · assumptions · faq.
