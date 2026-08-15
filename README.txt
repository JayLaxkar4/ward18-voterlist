WARD 18 CLOUD WEB APP — SETUP

This package is a cloud-ready, mobile-first PWA using Supabase for authentication and cloud data.

1) Create a Supabase project.
2) Open SQL Editor.
3) Run schema.sql.
4) Run seed.sql.
5) In Authentication > Users, create the private login account(s).
6) In index.html replace:
   YOUR_SUPABASE_URL
   YOUR_SUPABASE_ANON_KEY
   with the project's public URL and anon key.
7) Host the folder on any static HTTPS host (Vercel, Netlify, Cloudflare Pages, GitHub Pages, etc.).
8) Open the URL on iPhone/Android and use "Add to Home Screen".

SECURITY:
- The voter table is protected by Row Level Security.
- Anonymous/public users cannot read the table.
- Only authenticated users can read/update.
- For a real election workflow, keep this app private and do not expose the Supabase service_role key in the browser.

DATA:
827 voter records were imported from the supplied Excel workbook.
