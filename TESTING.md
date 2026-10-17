# SkillLoop smoke tests

Run the following after each code change. This checklist is a test plan; items are not marked passed merely because the app builds.

## Core UI

- [ ] Load Discover at desktop width and at 320px, 375px, and tablet widths.
- [ ] Navigate through Discover, My sessions, Saved skills, Community, Guilds, Messages, and My profile.
- [ ] Check for horizontal overflow, clipped controls, and usable touch targets on mobile.
- [ ] Confirm keyboard focus is visible and `Esc` closes overlays.
- [ ] Confirm `Ctrl/⌘ + K` returns to Discover and focuses the search box.

## Interactions

- [ ] Search by skill name, category, tag, and member name; clear search.
- [ ] Apply category, distance, duration, and experience filters; reset filters.
- [ ] Sort by nearest, rating, and session length.
- [ ] Save and unsave a skill; confirm Saved skills updates.
- [ ] Create a skill and verify it appears in Discover.
- [ ] Request a sample session and verify My sessions updates.
- [ ] Edit profile; verify the profile name, initials, and city update.
- [ ] Join/leave a sample guild and create a custom guild.
- [ ] Send a message; empty or whitespace-only messages should not be appended.
- [ ] Refresh the page and verify browser-local changes persist.
- [ ] Confirm all pages show the demo notice and no action implies a real message or booking was sent.
- [ ] Verify date inputs reject dates earlier than today.

## Build and deployment

- [ ] Run `npm install` and `npm run build`.
- [ ] Inspect the latest Vercel deployment and open the deployed site after the build succeeds.
- [ ] Inspect browser DevTools console and network panel for runtime errors and failed assets.
- [ ] Verify the icon, manifest, social metadata, and configured security headers.
- [ ] Check keyboard use and screen-reader labeling for dialogs, menus, and forms.
