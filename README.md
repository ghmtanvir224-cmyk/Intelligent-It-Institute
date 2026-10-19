# Intelligent IT Institute - starter (UNTESTED foundation)
Included: brand config, Zod schemas (BD mobile), API routes (honeypot, rate limit, no fake success), Supabase schema + RLS, AdmissionForm.
NOT included yet: app layout/pages, Tailwind setup, admin UI, blog, student portal.

## Setup
1. `npx create-next-app@latest` (TypeScript, Tailwind, App Router, src/), copy these files over, `npm i zod react-hook-form @hookform/resolvers @supabase/supabase-js server-only`.
2. Create a Supabase project; run `supabase/schema.sql` in the SQL editor.
3. Copy `.env.example` to `.env.local` and fill it (service role key stays server-side).
4. Make an admin: sign up, then `insert into profiles (id, role) values ('<auth user uuid>', 'admin');`
5. `npm run dev`
