# Release notes

## 2026-07-13 — Privacy policy update: anonymous usage analytics

### What changed

Anonymous usage analytics are now collected **by default** (opt-out), separate from crash diagnostics which remain opt-in.

### Analytics details

- **Events:** `session_start`, `pin_created`, `tracker_push`, `panel_time_spent`
- **Fields:** event name, tracker type, issue type, session duration, anonymous session ID, workspace user ID (signed-in users)
- **Never collected:** ticket content, annotation text, screenshots, screen recordings, page URLs, or any PII
- **Destinations:** Supabase (usage_events table) + PostHog (sub-processor)
- **Opt-out:** Settings → Workspace → Privacy → "Share anonymous usage data" (sets `notateAnalyticsOptOut` in `chrome.storage.local`)

### Privacy policy changes (notate.live/privacy/)

- Added **section 5: Anonymous usage analytics** — explains what is collected, where it goes (Supabase + PostHog), and how to opt out
- Updated **section 6 (Crash and error reporting)** — explicitly noted as opt-in, distinct from default-on analytics
- Updated **section 8 (This website)** — disclosed Google Analytics (GA4) on notate.live
- Updated **section 9 (What we don't do)** — replaced the "no usage analytics" bullet with an accurate statement about no content collection
- Updated **section 10 (Data retention)** — added analytics deletion request instructions
- Updated **TL;DR** — added analytics bullet with opt-out link; labeled Sentry as opt-in
- Bumped effective date to July 13, 2026

### Docs updated

- `docs/CWS_PRIVACY_JUSTIFICATIONS.md` — data type declarations for Chrome Web Store
- `docs/CHROME_WEB_STORE_RELEASE_CHECKLIST.md` — pre-submission checklist with analytics rows

---

## Older entries

_Add entries above this line._
