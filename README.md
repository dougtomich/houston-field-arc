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

Quote requests go to doug.tomich@gmail.com through FormSubmit. The first real submission sends a confirmation email that has to be clicked once. Change the address in `index.html` (`formsubmit.co/...`) when the business has its own inbox.

Netlify project `houston-field-arc` is out of credits, so new deploys there are skipped. The live copy is GitHub Pages until credits are available or the domain is pointed at Pages.
