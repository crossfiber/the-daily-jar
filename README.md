# The Daily Jar — Website Build

Handcrafted grass-fed tallow skincare by Will & Juju. Early-stage launch storefront.

- Target site URL: none (net-new build)
- Build date: 2026-05-23
- GitHub repo: `crossfiber/the-daily-jar`
- Live GitHub Pages URL: https://crossfiber.github.io/the-daily-jar/ (confirm after deploy)

## Fonts
- Headlines: Fraunces — https://fonts.google.com/specimen/Fraunces
- Body: Hanken Grotesk — https://fonts.google.com/specimen/Hanken+Grotesk
- Combined CSS: https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,400;0,9..144,500;0,9..144,600;0,9..144,700;1,9..144,500&family=Hanken+Grotesk:wght@400;500;600;700&display=swap

## Color palette (source)
- `#F6F0E1` cream page bg — label background
- `#EDE4CF` alt section bg — derived warm cream
- `#FBF7EE` card ivory — derived
- `#2E4A33` forest green (primary CTA + links) — logo script green
- `#16271A` forest-deep (footer) — derived from brand green
- `#7E8C57` sage (eyebrow/botanical) — label sprig green
- `#C2982F` honey gold (decorative accent) — jar icon / heart / "By Will & Juju"
- Per-scent: Rose Glow `#B9637A`, Golden Garden `#D69A2E`, Warm & Cozy `#9C6B4A`

## Design direction (one paragraph)
Warm botanical-apothecary built from The Daily Jar's own label language: cream paper, deep grass-green voice, honey-gold flourishes, botanical sprig dividers, and a per-scent accent system so the three scents read as one collection. Deliberately avoids the cold clinical minimalism of most natural-skincare sites and every common AI tell.

## Placeholders that still need real content
- `[REAL PHOTO NEEDED]` — hero jar shot, per-scent product shots, lifestyle/ritual shot, story shot (Higgsfield images to be dropped in; current build uses the two real owner photos in `assets/` plus styled placeholders).
- `[LOGO ASSET NEEDED FROM CLIENT]` — clean transparent logo (SVG/PNG). The only logo we have is printed on the wood lid photo; not cropped or recreated. Nav/footer use a Fraunces text wordmark for now.
- `[VERIFIED NUMBER NEEDED]` — confirm "400+ jars" before public use; review count/rating.
- `[NEEDED FROM CLIENT]` — phone, email, pickup/delivery address, social handles.

## Hotlinking risks
- None. Both photos are stored locally in `assets/` and re-hosted in the repo. No Squarespace/Wix/Shopify CDN dependencies.

## Reference builds consulted
- JOTL (`C:\Users\accc0\Downloads\JOTL\index.html`) — borrowed mobile drawer, single-open accordion, scroll-snap carousel, static JS form validation, CSS-variable architecture. See `borrowed-patterns.md`. No visual identity borrowed.

## Checkout
Build ships with swappable "Add to Cart / Shop" CTA hooks. Decision (2026-05-23): Stripe Checkout / Payment Links on the custom site, wired to the domain. The Daily Jar is make-to-order with no inventory, so Shopify is unnecessary; Stripe means no monthly platform fee and the design stays fully custom. CTAs route through a single `ORDER_URL` swap point (currently the Google order form). See `design-direction.md`.

## Files
- `index.html` — the build (all CSS/JS inline)
- `assets/` — `jar-trio.jpg`, `lid-logo.jpg` (real owner photos)
- `design-direction.md`, `borrowed-patterns.md`, `credentials.md` (local only)

## Update 2026-05-23: Product photography added (Higgsfield, Nano Banana Pro)
Generated reference-driven, brand-correct, label one-to-one photography and wired it into the live site:
- assets/rose-glow.jpg, assets/golden-garden.jpg, assets/warm-cozy.jpg (scent cards, 1:1)
- assets/hero-golden.jpg (homepage hero, 4:5)
- assets/texture-open.jpg (open-jar whipped-balm shot, "why tallow" band)
- assets/trio-lineup.jpg (bonus collection lineup for marketing/social)
Big label text (brand, scent name, "All-Over Tallow Balm", Good to Know, Net Wt) renders one-to-one. Tiny ingredient print is approximate at full zoom but illegible at web display size. Alternate variants kept locally in _proofs/. Prompt recipe and shot list in photoshoot-plan.md. Remaining placeholders: clean logo asset, phone, email, socials, verified review count.
