# 2026.09 — Maintenance release

- Maintenance review of `wrestling-event-landing` — a static landing page for "Iron Fist Wrestling — Night of Champions", built as a speculative demo for a client pitch.
- Stack: a single 404-line `index.html` using the Tailwind CDN and Google Fonts (Anton / Bebas Neue / Inter), with no build step and no dependencies. `vercel.json` sets cleanUrls plus X-Content-Type-Options, Referrer-Policy and Permissions-Policy headers.
- Status: public repo, last commit 2026-04-22 (the initial build). Sections shipped: sticky ticket CTA, ticker marquee, hero with countdown, match card, 12-slot talent roster, GA/Ringside/VIP ticket tiers with an Eventbrite embed mount at `#eventbrite-mount`, venue block, FAQ and footer. No live URL is stated in the repo.
- Reviewed September 2026: documentation refreshed and tagged v2026.09. No markup, styling or header-config changes.
- Known gaps visible in the repo: no CHANGELOG before this release, no LICENSE, no package.json (so nothing to version), and the page is still in demo state — the hard-coded event date is `2026-05-17T19:30:00` (now in the past), eight ticket/CTA links are still `href="#"`, the Eventbrite widget slot is empty, and the 12 roster portraits are placeholder divs rather than images.
