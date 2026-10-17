# SkillLoop release checklist

## Publishable demo

- [x] Vite production build is configured for Vercel (`npm run build` → `dist/`).
- [x] Responsive layout and mobile navigation included.
- [x] App metadata, icon, and web manifest included.
- [x] Baseline security headers configured in `vercel.json`.
- [x] Demo data and browser-only storage limitations disclosed in the interface.
- [ ] Run all manual checks listed in [TESTING.md](./TESTING.md) in a real browser.

## Required before launching a real public marketplace

- [ ] Connect a dedicated production backend and configure environment variables on Vercel.
- [ ] Implement sign-up, sign-in, session management, account recovery, and account deletion.
- [ ] Store profiles, skills, bookings, guilds, and messages in a shared database with server-enforced ownership policies.
- [ ] Add reporting, blocking, moderation, and response procedures.
- [ ] Replace sample ratings, verification labels, locations, member counts, and notifications with verified server data.
- [ ] Implement and test a server-side time-credit ledger with transaction invariants and an audit trail.
- [ ] Publish reviewed Privacy Policy, Terms of Service, community rules, and support contact.
- [ ] Add monitoring, backups, abuse rate limits, and recovery procedures.
- [ ] Complete accessibility, security, and cross-browser checks before allowing real users or exchanges.

SkillLoop should be described as a **demo** until all production items above are complete.
