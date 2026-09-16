# Iron Fist Wrestling — Night of Champions

Static landing page for a pro wrestling event. Built as a speculative demo for a client pitch.

## Status

Last reviewed: September 2026 · release v2026.09

## Stack

- Single `index.html` — Tailwind CDN, Google Fonts (Anton / Bebas Neue / Inter)
- No build step. Deploy to Vercel / Netlify / GitHub Pages as-is.
- Eventbrite Embedded Checkout slot at `#eventbrite-mount` — drop widget in, done.

## Sections

1. Sticky "Buy Tickets" CTA (top-right, hides on footer)
2. Top bar + ticker marquee
3. Hero — countdown, poster, dual CTAs, social proof
4. Match card — main event + 3 headliners + 4 undercard
5. Talent roster — 12 placeholder portraits
6. Ticket tiers — GA / Ringside / VIP + Eventbrite embed slot
7. Venue — address, doors/bell times, map slot, directions
8. FAQ — 5 entries
9. CTA footer strip + site footer

## Customization

- Event date: `index.html` → `const EVENT = new Date('2026-05-17T19:30:00')`
- Brand colors: Tailwind config — `blood` (#e10600), `volt` (#f5ff2b), `ink` (#0a0a0a), `bone` (#f5f1e8)
- Ticket links: replace `href="#"` on `[data-tier]` buttons with Eventbrite URLs
- Wrestler photos: swap `.aspect-[3/4] bg-ink halftone` divs with `<img>` tags

## Deploy

```bash
vercel --prod
```

Or push to GitHub and connect via Vercel dashboard.
