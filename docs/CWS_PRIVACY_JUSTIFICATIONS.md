# Chrome Web Store — Privacy Justifications

This document maps each data type Notate declares in the Chrome Web Store Developer Dashboard to its purpose and handling. Update it whenever collection behavior changes.

---

## Data types declared

### 1. Website content

**Declared?** No — Notate reads the active tab's DOM to identify pinned elements and generate CSS selectors, but this content is processed locally and never transmitted to Notate's servers.

### 2. User activity

**Declared?** Yes — **Anonymous usage analytics**.

| Field | What | Why |
|---|---|---|
| `session_start` | Extension opened | Understand engagement |
| `pin_created` | A pin was dropped | Track core feature adoption |
| `tracker_push` | Ticket exported (includes which tracker: Linear or Jira, and issue type) | Understand integration usage |
| `panel_time_spent` | Seconds panel was open | Gauge session depth |
| Anonymous session ID | Random ID per session | Deduplicate events |
| User ID | Only for signed-in workspace users | Associate events with workspace (not individual identity) |

**Not collected:** annotation text, ticket titles/descriptions, screenshot pixel data, screen recording data, page content, URLs visited.

**Destinations:** Supabase (operator-controlled database) + PostHog (sub-processor, product analytics only).

**Default:** Collected by default. User can opt out at Settings → Workspace → Privacy → "Share anonymous usage data" (sets `notateAnalyticsOptOut` in `chrome.storage.local`).

### 3. Crash reports (Sentry)

**Declared?** Yes — **Crash and error reporting**.

| Field | What |
|---|---|
| Error message + stack trace | Technical crash details |
| Extension version | Identify affected release |
| Browser + OS | Environment context |
| Timestamp | When the error occurred |

**Not collected:** annotation content, screenshots, page content.

**Destination:** Sentry (sub-processor).

**Default:** **Opt-in only.** Users must explicitly enable crash reporting.

### 4. Authentication tokens (Linear / Jira)

**Declared?** Yes — stored locally on the user's device (`chrome.storage.local`). Never transmitted to Notate servers.

### 5. User-created annotations

Stored locally in `chrome.storage.local`. Not transmitted to Notate. Transmitted to Linear or Jira only when the user explicitly exports a ticket.

---

## Justification for default-on analytics

Anonymous usage analytics are on by default because:
1. The data is strictly metadata — no content, no PII beyond an anonymous session ID.
2. It is essential for a small team to understand which features are actually used without relying on support tickets alone.
3. Users are informed at onboarding and can opt out immediately with a single toggle.
4. The collection is disclosed in the privacy policy (section 5) and in the CWS data-use disclosure.

---

## Sub-processors

| Sub-processor | Purpose | Privacy policy |
|---|---|---|
| PostHog | Product analytics aggregation | https://posthog.com/privacy |
| Sentry | Crash and error reporting | https://sentry.io/privacy/ |
| Supabase | Usage event storage | https://supabase.com/privacy |
| GitHub Pages | Website hosting | https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement |
| Google Analytics | Website analytics (notate.live only) | https://policies.google.com/privacy |

---

_Last updated: 2026-07-13_
