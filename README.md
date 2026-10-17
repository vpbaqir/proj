# SkillLoop

SkillLoop is a responsive, dark/neumorphic web preview for a community where people exchange knowledge instead of paying cash. The current release is designed to be deployed publicly as an interactive product demo.

## Included

- Responsive discover, community, saved-skills, sessions, messages, and profile screens
- Search, category filters, distance sorting/filtering, rating sorting, session-duration and experience-level filters
- Add a sample skill, request a sample session, edit the local profile, join sample guilds, and create a guild
- Keyboard shortcuts: `Ctrl/⌘ + K` focuses skill search; `Esc` closes open overlays
- Local-browser persistence for profile changes, saved skills, sessions, messages, and guild membership
- Accessible form types, visible keyboard focus, live date defaults, app icon, web manifest, social metadata, and baseline security headers

## Run locally

Requires Node.js 22.12 or later.

```bash
npm install
npm run dev
```

## Build and preview

```bash
npm run build
npm run preview
```

Vercel is configured to run `npm run build` and publish the Vite `dist/` folder.

## Important release boundary

**This is a browser-local demo, not yet a shared multi-user marketplace.** The sample profiles, ratings, locations, and existing conversation are illustrative. Edits persist in the visitor's browser only. No real booking request, message, identity verification, location lookup, notification, or time-credit transaction is sent to another person. Browser storage can be cleared by the user and does not sync to another device.

Before presenting SkillLoop as a real community service, connect a dedicated backend for authentication and account recovery, a shared database with row-level security, server-validated booking and messaging, abuse reporting/moderation, privacy/terms pages, backups, and a tested time-credit ledger. Do not treat the sample ratings or verification icons as trust signals. Do not use a service-role API key in frontend code.

See [TESTING.md](./TESTING.md) and [RELEASE_CHECKLIST.md](./RELEASE_CHECKLIST.md) before public launch.
