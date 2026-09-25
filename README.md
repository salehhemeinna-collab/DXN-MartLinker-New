# DXN MartLinker — Minimal Independent Apps

Two completely independent static apps using the same Supabase project.

## Customer
Deploy `/customer` as the root of the test site `www.martlinker.com`.

## Admin
Deploy `/admin` as a separate Cloudflare Pages project/domain. Do not deploy it to `dxn.martlinker.com`.

Production `dxn.martlinker.com` remains untouched.

Each app intentionally has only 3 files: `index.html`, `app.js`, `*.css`. Supabase uses the public publishable client key in the browser; service-role secrets are not included.
