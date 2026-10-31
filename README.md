# Houston Field Arc

One-page site for Houston Field Arc, mobile welding and fabrication in Greater Houston.

Domain: houstonfieldarc.com (Porkbun, registered 2026-10-22, paid through 2027-10-22).
Netlify project: houston-field-arc (`93487816-dbce-4fc9-bd5d-badd1b97b81f`).
GitHub: dougtomich/houston-field-arc.

No build step. Publish directory is the repo root.

## Still blank on purpose

- Phone number. Every quote path is the form until a real number is confirmed.
- No license line, years-in-business, or reviews. Do not add those until they are real.

## Point houstonfieldarc.com at Netlify

The domain still shows Porkbun’s parking page until both of these are done.

1. Netlify → project **houston-field-arc** → Domain management → Add domain → `houstonfieldarc.com`. Add `www.houstonfieldarc.com` too. Set the apex as primary.
2. In Porkbun DNS for that domain, remove the parking records and add:
   - `www` — CNAME — `houston-field-arc.netlify.app`
   - `@` — ALIAS (Porkbun supports this) — `apex-loadbalancer.netlify.com`
3. Wait for Netlify to issue the certificate. HTTPS can take a few minutes after DNS is correct.

Quote form name is `quote`. Submissions land in Netlify Forms. Success page is `/thanks`.
