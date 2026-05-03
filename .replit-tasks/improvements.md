# Replit Agent Task Spec — Trapables

## Instructions for Replit Agent
You are enhancing this NYC streetwear storefront. Read this file carefully before touching any code.
Commit all changes with prefix "replit: " and push to main when done.

## Current State
The site has excellent design (dark aesthetic, purple accent, Bebas Neue display font).
Products exist: beanie-purple, beanie-white, hat-orange, hat-red, hoodie-white, pants-black, tracksuit-blue, varsity-jacket.
The JS has product data but no real checkout flow.

## Stack Rules (non-negotiable)
- Static HTML/CSS/JS only — no framework needed
- Payments → Snipcart (free tier, add to cart + checkout)
- Newsletter → Klaviyo free tier embed form
- No Vercel — deploy on Cloudflare Pages

## Tasks

### 1. Product Data — Fill Out All Products
Update the JS product array with real descriptions and correct pricing:
```
Varsity Jacket — "Old school NYC energy. Wool body, leather sleeves, embroidered Trapables crest." — $120
Tracksuit Blue — "Two-piece street set. Relaxed fit, elastic cuffs, zip pocket." — $85
Hoodie White — "Premium heavyweight fleece. Dropped shoulders, kangaroo pocket, embroidered logo." — $65
Pants Black — "Relaxed cargo joggers. Six pockets, tapered leg, drawstring waist." — $55
Hat Orange — "5-panel structured cap. Snapback, embroidered T logo, one size fits all." — $35
Hat Red — "Classic 6-panel cap. Curved brim, adjustable strap, embroidered Trapables wordmark." — $30
Beanie Purple — "Ribbed knit beanie. Folded cuff, embroidered logo patch, one size." — $25
Beanie White — "Clean white ribbed beanie. Street staple. Embroidered black logo." — $22
```

### 2. Size Selector
Add size dropdown (XS/S/M/L/XL/XXL) to each clothing product card before add-to-cart.
Hats and beanies: show "One Size" (no selector).

### 3. Real Cart & Checkout (Snipcart)
- Add Snipcart CDN to `<head>`
- Convert "Add to Cart" buttons to Snipcart buy buttons with correct data attributes
- Test that cart opens and checkout flow works
- Snipcart key: use placeholder `YOUR_SNIPCART_KEY` (Markus will replace)

### 4. Drop Countdown Timer
In the "UPCOMING DROP" section, add a live countdown timer to: July 4, 2026 (Independence Day capsule drop).
Display: DD days HH:MM:SS in the existing neon styling.

### 5. Newsletter Section
Above the footer, add an email capture section:
- Headline: "GET FIRST ACCESS"
- Subhead: "Drop alerts. Early access. No spam. Just the movement."
- Embed a Klaviyo popup trigger button (use placeholder list ID)

### 6. About Section — Expand Copy
Replace the existing about section with:
```
BORN IN THE STREETS OF NYC

Trapables started with one idea: NYC culture deserves gear that actually looks like NYC.
Not corporate streetwear. Not fast fashion. Real pieces for real people who live this city.

We drop limited runs — never restocking. When it's gone, it's gone.
Every piece is designed in New York. Every stitch tells a story.

If you know, you know. If you don't — you're about to find out.
```

### 7. Instagram Grid
In the "ON THE GRAM" section, replace placeholder with a link to @trapables Instagram.
Add CTA: "FOLLOW @TRAPABLES" button linking to https://instagram.com/trapables

### 8. SEO Meta Tags
Add to `<head>`:
- `<meta name="keywords" content="NYC streetwear, Trapables, New York hoodie, limited drop, street culture">`
- `<link rel="canonical" href="https://trapables.com">`
- Open Graph tags for social sharing

### 9. Mobile Polish
- Test all breakpoints (320px, 375px, 768px, 1024px)
- Ensure cart drawer works on mobile
- Size selector is touch-friendly (min 44px tap target)