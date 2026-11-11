# LoyaAI – AI Agents Marketplace

Next.js 14 (App Router) · Supabase · Stripe · Tailwind · shadcn/ui-style components · Vercel-ready

## Run
```bash
npm install
cp .env.example .env.local   # fill in keys (optional: site runs on seed data without them)
npm run dev
```

## Connect services
- **Supabase**: run `supabase/schema.sql` in the SQL editor, insert rows from `lib/agents.ts`, add URL + anon key to `.env.local`.
- **Stripe**: add `STRIPE_SECRET_KEY`. `/api/checkout` creates a hosted Checkout session.
- **Deploy**: push to GitHub, import in Vercel, add the same env vars.

## Built so far
- `/` Homepage · `/store` Store with category, price and rating filters
- Live "Try Now" demos: `public/demos/chat.html` (scripted, swap for real agent endpoints)
- Nav links to /demos, /blog, /dashboard, /login are placeholders until those pages are built.
