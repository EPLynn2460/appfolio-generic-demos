# Service Pros — Embedded Booking Mockup

White-label booking flow Amenify can embed inside PMS partner resident portals
(AppFolio, Yardi, RealPage, Buildium, etc.) for move-in / move-out cleaning.

Live mockup: a single static `index.html` — no build step, no framework. Vercel
deploys it as-is.

## Local preview

Just open `index.html` in a browser. Or:

```bash
npx serve .
```

## Deploy

This is a static site. Push to GitHub, import in Vercel, deploy. No build
command, no output directory — Vercel auto-detects.

## What's inside

A 5-step interactive flow rendered inside a replicated 2B Living / AppFolio
portal shell:

1. **Landing** — pitch, social proof, *Powered by Amenify* mark
2. **Choose service** — unit info pre-pulled from PMS; Simple / Plus / Deep / Move-Out tiers; add-ons
3. **Schedule** — date + arrival window, tied to move event
4. **Pay** — Stripe-style card form, ToS opt-in
5. **Confirmation** — booking ID, what-happens-next

## Replicating for other PMS partners

Only three things change per partner: sidebar palette, top brand mark, footer.
The booking flow itself is partner-agnostic.
