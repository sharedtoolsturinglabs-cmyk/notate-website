# Chrome Web Store — Release Checklist

Pre-submission checklist for Notate CWS releases. Complete every applicable item before submitting to review.

---

## Privacy & data practices (Developer Dashboard → Privacy tab)

Fill in the "Data usage" table in the CWS Dashboard with the values below. Update this file if collection behavior changes.

### Data types collected

| CWS category | Sub-type | Collected | Justification |
|---|---|---|---|
| Personally identifiable information | Name, email, address, phone | **No** | — |
| Personally identifiable information | User IDs | **Yes** (workspace user ID only, signed-in users) | Associate anonymous analytics events with a workspace account |
| Financial and payment information | — | **No** | — |
| Authentication information | Passwords, credentials | **No** | Auth tokens are stored locally only, not transmitted to Notate |
| Personal communications | Emails, messages | **No** | — |
| Location | — | **No** | — |
| Web history | — | **No** | DOM is read locally; URLs are not transmitted |
| User activity | App activity, interaction info | **Yes** | Anonymous usage analytics (see below) |
| Website content | — | **No** | DOM processed locally; never sent to Notate |
| Health information | — | **No** | — |

### User activity — detail

Events and fields collected for anonymous usage analytics:

- `session_start`, `pin_created`, `tracker_push`, `panel_time_spent`
- Tracker type (Linear / Jira), issue type, session duration
- Anonymous session ID; workspace user ID (signed-in users only)

**Never collected:** ticket text, screenshots, page content, recordings.

**Default:** On by default. Opt-out: Settings → Workspace → Privacy → "Share anonymous usage data".

### Crash reporting (Sentry)

- Error messages, stack traces, extension version, browser/OS type, timestamps
- **Opt-in only**

---

## Pre-submission checklist

### Code & functionality
- [ ] All features described in the Store listing work as documented
- [ ] Extension requests only the permissions it actually uses
- [ ] No `eval()` or remote code execution
- [ ] Content Security Policy is correctly set in `manifest.json`

### Privacy
- [ ] `privacy/index.html` on notate.live is up to date and matches current collection behavior
- [ ] CWS Dashboard "Data usage" table matches this document
- [ ] `docs/CWS_PRIVACY_JUSTIFICATIONS.md` is up to date
- [ ] If collection behavior changed, bump the "Last updated" date on the privacy policy

### Store listing
- [ ] Screenshots are current and accurate
- [ ] Description does not make unverifiable claims
- [ ] Version number in `manifest.json` incremented correctly (semver)
- [ ] Changelog entry added to `notate.live/changelog/`

### Testing
- [ ] Tested on latest stable Chrome
- [ ] Tested on Chrome Beta (optional but recommended)
- [ ] Tested fresh install + upgrade from previous version
- [ ] Analytics opt-out toggle verified: events stop after disabling
- [ ] Crash reporting opt-in verified: no Sentry events when disabled

### Post-submission
- [ ] Monitor CWS review status (typically 1–3 business days)
- [ ] Respond promptly to any review questions

---

_Last updated: 2026-07-13_
