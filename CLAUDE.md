# Master Cleaning Services Tampa — Project Context

This folder is the live website for **Master Cleaning Services Tampa** — the Florida sister site to the Boston operation. When you (Claude, in any new session) enter this folder, read this file first.

## What lives here

```
tampa-site/
├── index.html                      ← homepage
├── air-duct-cleaning/              ← service page (Florida-tuned)
├── ac-cleaning/                    ← service page (AC coil + blower + drain pan — Tampa specialty)
├── dryer-vent-cleaning/            ← service page
├── chimney-cleaning/               ← service page
├── service-areas/                  ← landing pages by Tampa Bay city
│   ├── index.html
│   ├── tampa/
│   ├── st-petersburg/
│   ├── clearwater/
│   ├── brandon/
│   ├── riverview/
│   └── wesley-chapel/
├── blog/                           ← blog index (posts to be added)
├── contact/                        ← free quote / contact page
├── sitemap.xml
├── robots.txt
└── css/style.css                   ← shared stylesheet (cloned from Boston)
```

## Business facts (memorize before any user-facing copy)

- **Business name:** Master Cleaning Services (Tampa)
- **Phone:** (617) 934-8512 · WhatsApp: https://wa.me/16179348512
- **Email:** Masterinductcleaning@gmail.com
- **Domain (placeholder):** https://masterductcleaningtampa.com — replace with the real Tampa domain when launched
- **GA4 ID:** G-G06E8B465L (currently shared with Boston site — replace if separating analytics)
- **Core services:**
  - Air duct cleaning (negative-pressure extraction with rotary brush agitation)
  - AC / HVAC coil cleaning (evaporator, blower wheel, drain pan — the Tampa specialty)
  - Dryer vent cleaning
  - Chimney cleaning
- **Pricing:** Air duct from $99 · AC coil from $99 · Dryer vent from $79 · Combo (duct+vent) from $149 · Chimney from $99
- **Hours:** Mon–Sun, 7 AM – 9 PM
- **Service area (6 counties):** Hillsborough, Pinellas, Pasco, Sarasota, Manatee, Polk
  - Tampa, St. Petersburg, Clearwater, Brandon, Riverview, Wesley Chapel, Lutz, Land O' Lakes, Plant City, Lakeland, Sarasota, Bradenton, Largo, Pinellas Park, Seminole, Palm Harbor, Dunedin, Tarpon Springs, Apollo Beach, Sun City Center

## Why a separate Tampa site (not just an extension of Boston)

The two markets behave very differently and would compete with each other on Google if hosted under one domain:

- Boston site = duct cleaning + dryer vent + chimney, focused on cold-climate concerns (allergens, pre-1970 homes, heating-season prep)
- Tampa site = AC coil cleaning is the lead service (musty smell, weak cooling, mold), with humidity and oak pollen as the climate angle

Content is **substantially original** on every page — no copy/paste of Boston body text. Schema, titles, descriptions, FAQs, and reviews are unique to Tampa Bay. Layout and CSS are shared because they're brand-level, not content-level.

## SEO / AEO strategy

- Every page targets **city + service** for search intent (e.g., "AC coil cleaning Tampa FL")
- FAQ Q&A on every page mirrors how Tampa homeowners ask AI assistants questions ("Why does my AC smell musty in Tampa?")
- Schema markup on every page: HVACBusiness, Service, FAQPage, BreadcrumbList
- Florida-specific authority signals woven throughout: 75% humidity, 60% indoor mold threshold, oak pollen Dec–May, 2,900 dryer-vent fires/year (USFA), Angi Tampa average $300–$700, NADCA 3–5 year guideline
- Each service-area page has unique neighborhood-specific facts (no boilerplate "we serve [city]" language)

See `seo` and `aeo-boston` skills (the AEO playbook applies — just swap Boston → Tampa).

## Default behavior for new sessions

- If the user asks to **add a city/neighborhood page** → use the existing 6 service-area pages as the template; write unique facts and FAQs for the new city. Don't copy/paste text from another city page.
- If the user asks to **add a blog post** → write 800–1,200 words original Tampa-specific content; do not paraphrase Boston posts. Save under `blog/[slug]/index.html`.
- If the user asks about **SEO** → load the `seo` skill.
- If the user asks about **AEO / AI ranking** → load the `aeo-boston` skill (principles apply; substitute Tampa).
- If the user asks for a brand-new automation agent → ask clarifying questions, then save it as `.{name}-agent/` (mirror the Boston site's pattern).

## Hard rules

- **Never copy body text from the Boston site.** Schema, titles, meta descriptions, FAQs, and section copy must be substantially different. CSS and HTML structure can be shared.
- **Never invent stats.** All Florida facts on the site are sourced (Angi for pricing, USFA for fire stats, NFPA for chimney guidance, NADCA for cleaning frequency).
- **Date for sitemap.xml** must come from `date +%Y-%m-%d` when updated.
- **Hebrew is the user's preferred report language.** Code, file names, and HTML stay in English.

## Open items / TODO

- Replace placeholder domain `masterductcleaningtampa.com` with real Tampa domain when registered
- Decide on Tampa-area phone number — current site uses Boston (617) 934-8512 per user request, but a local 813/727/941 number would help local SEO trust signals
- Set up Google Business Profile for Tampa as a service-area business (not storefront)
- Submit `sitemap.xml` to Google Search Console once domain is live
- Build out blog posts (see `blog/index.html` for planned topics)
- Consider adding a dedicated `mold-removal/` service page given how prominent the Florida humidity angle is
