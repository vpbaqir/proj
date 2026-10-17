# SkillLoop

Trade expertise, not cash—connect locally to learn, teach, and grow.

A polished responsive React + Vite prototype for local, time-based skill swaps. Built with an editorial dark/neumorphic interface, subtle mint accents, accessible labels, and responsive layouts.

## What works in this prototype
- Browse and search community skills, filter by category, and sort by distance, rating, and duration
- Browse personalized matching mode (heuristic match based on profile interests)
- Save and unsave skills
- Request a skill exchange with a date, time, and note
- View sessions and status, send demo in-app messages
- Offer a skill, edit a profile, browse/join local guilds
- Responsive mobile navigation, notifications, and basic safety guidance

## Run locally
\`\`\`bash
npm install
npm run dev
\`\`\`

## Build
\`\`\`bash
npm run build
npm run preview
\`\`\`

## Important prototype notes
Data is stored in in-memory React state and resets on refresh. Authentication, real location matching, ID verification, video calls, moderation, persistent storage, notifications, and a real double-entry time-credit ledger are not connected. Never present a demo verification badge or time balance as proof of real identity or transferable credits. Before launch, add a backend (e.g. Supabase), row-level security, server-side validation, abuse reporting, and tests for all credit transactions.
