# WASSCEPASSCO — final starter
This project is designed for one-time GitHub Pages deployment from the `main` branch. Supabase handles accounts, database and resource storage, so new PDFs do not require redeployment.

## Setup
1. Create a Supabase project.
2. Run `sql/schema.sql` in Supabase SQL Editor.
3. Create your first account on the site.
4. In Supabase Table Editor, change that account's `profiles.role` to `admin` (or use the SQL update at the bottom of schema.sql).
5. Put the Supabase project URL and public/publishable/anon key in `config.js`.
6. Enable Google provider in Supabase Auth if you want Google login, and configure its OAuth redirect/callback settings.
7. Upload the folder to GitHub `main`.
8. GitHub Settings → Pages → Source: Deploy from a branch → `main` → `/ (root)`.
9. The PWA can then be installed from supported browsers.

## AdSense
The site contains ad slots and privacy/terms pages. Add the exact AdSense code supplied by Google only after an eligible account is approved. Never put a service-role/secret Supabase key in frontend files.

## Admin uploads
The admin dashboard uses Supabase Storage and the `resources` table. New resources are published from the app and do not require a GitHub redeploy.
