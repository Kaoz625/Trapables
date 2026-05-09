# Replit Agent Task: Trapables

## Goal
Build out Trapables into a fully functional NYC street culture merch store with AI-powered ordering, authentic NYC tone throughout, and a Supabase + Cloudflare Pages stack.

## Tasks
1. Design and build a homepage with hero section: bold NYC street culture aesthetic, graffiti-inspired typography, dark background, gold/neon accents
2. Create a Products/Shop page with grid layout showing merch items (hoodies, tees, hats, accessories) — use realistic placeholder products with names, prices, and images
3. Implement an AI ordering assistant chatbot (OpenAI GPT-4o) that helps users pick gear based on their vibe, size, and NYC neighborhood — embed as a floating chat widget
4. Build a product detail page with size selector, color picker, quantity input, and "Add to Cart" button
5. Implement a shopping cart (localStorage or Zustand state) with item list and checkout CTA
6. Add a checkout flow placeholder that collects name, email, shipping address — wire up to Supabase `orders` table
7. Create a `street_culture_manifesto` landing section: short brand story copy, NYC street art photography placeholders, bold pull quotes
8. Add Instagram feed placeholder section (link to @trapables or @nyctailblazers)
9. Implement Supabase auth (email magic link) for order history
10. Set up Supabase schema: `products`, `orders`, `order_items`, `users` tables with RLS policies
11. Style with authentic NYC street tone — copy should feel like it was written by someone from Brooklyn, not a corporate brand
12. Deploy static frontend to Cloudflare Pages, API routes via Cloudflare Workers or a Coolify backend

## Tech Stack
- React 18 + TypeScript
- Vite
- Tailwind CSS
- Supabase (auth, database, storage for product images)
- OpenAI GPT-4o (AI ordering assistant)
- Cloudflare Pages (frontend) + Coolify (if backend needed)
- Zustand (cart state)

## Deploy Target
Cloudflare Pages for frontend. Backend API on Coolify if needed. Never Vercel.

## Done When
- [ ] Homepage hero loads with NYC street culture aesthetic
- [ ] Products grid shows at least 6 placeholder items with prices
- [ ] AI chat widget opens and responds to product questions
- [ ] Cart state persists across page navigations
- [ ] Supabase schema is created with products/orders tables
- [ ] Checkout form submits to Supabase orders table
- [ ] All changes pushed to `Kaoz625/Trapables` main branch
