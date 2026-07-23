# Notate — Marketing Copy Extraction (index.html)

Source: `index.html` (the marketing homepage). This is a single static HTML file with no separate component files; all visible text lives in `index.html`. Copy below is quoted verbatim.

## 1. Head metadata

- **`<title>`**: `Notate — Point. Comment. Log.` — 29 characters
- **`<meta name="description">`**: `Capture UI issues directly in your browser and push them to Linear or Jira in seconds. Free to start — $7/mo for unlimited.` — 123 characters
- **Canonical tag**: MISSING (no `rel="canonical"` present)
- **Open Graph tags**:
  - `og:type`: `website` — 7 characters
  - `og:title`: `Notate — Point. Comment. Log.` — 29 characters
  - `og:description`: `Capture UI issues directly in your browser and push them to Linear or Jira in seconds. Free to start — $7/mo for unlimited.` — 123 characters
  - `og:image`: `https://notate.live/og-image.png` — 32 characters
  - `og:url`: `https://notate.live/` — 20 characters
  - (additional, not requested) `og:site_name`: `Notate` — 6 characters
- **Twitter card tags**:
  - `twitter:card`: `summary_large_image` — 19 characters
  - `twitter:title`: `Notate — Point. Comment. Log.` — 29 characters
  - `twitter:description`: `Capture UI issues directly in your browser and push them to Linear or Jira in seconds. Free to start — $7/mo for unlimited.` — 123 characters
  - `twitter:image`: `https://notate.live/og-image.png` — 32 characters
- **JSON-LD structured data blocks**: MISSING (no `application/ld+json` blocks present)
- **`lang` attribute on `<html>`**: `en`
- **`robots` meta tag**: MISSING

## 2. Heading hierarchy

```
H1: Turn screenshots into JIRA tickets in seconds.
  H2: Feedback shouldn't be / a full-time job.
    H3: Reports scattered everywhere
    H3: Endless clarification calls
    H3: No clear ownership
    H3: Impossible to reproduce
  H2: Three steps. / Seamless reporting.
    H3: Point at exactly what's broken
    H3: Context is captured automatically
    H3: One click to Linear or Jira
  H2: Everything you need. / Nothing you don't.
    H3: Spotted to filed, in under 5 seconds.
    H3: One click to Linear and Jira.
    H3: Smaller than a stock photo.
    H3: Context for your agents.
    H3: Free to start. $7/month when you outgrow it.
  H2: Your data stays local by default. / Cloud is opt-in.
  H2: What you'd usually pay $39–$199/month for. / $7.
  H2: Questions, / answered honestly.
  H2: Stop turning UI issues / into long conversations.
    H5: Product
    H5: Compare
    H5: Community
    H5: Legal
```

Flags:
- **Multiple H1s**: None — exactly one H1 (`Turn screenshots into JIRA tickets in seconds.`).
- **Skipped levels**: Yes — the footer jumps from `H2` (`Stop turning UI issues into long conversations.`) straight to `H5` (`Product`, `Compare`, `Community`, `Legal`); H3 and H4 are skipped. There is no `H4` anywhere on the page.
- **Decorative headings**: None are purely decorative; the `.accent` `<span>`s (`in seconds.`, `a full-time job.`, `Nothing you don't.`, `$7.`, `answered honestly.`) are fragments inside their parent headings, not standalone headings.
- **Headings with no searchable noun**: `H2: Everything you need. Nothing you don't.` contains no concrete/searchable product noun. The compare `H2` accent fragment `$7.` and the FAQ `H2` fragment `answered honestly.` also lack nouns in isolation, but each is part of a larger heading that does.
- Note: the H1 uses `JIRA` (all caps); every other occurrence on the page is `Jira`.

## 3. Section-by-section copy inventory

### Section: Hero
- **id**: `top` — **data-screen-label**: `Hero`
- **Eyebrow / kicker**: `Chrome extension`
- **Heading**: `Turn screenshots into JIRA tickets in seconds.` (accent span: `in seconds.`)
- **Subheading (.hero-sub)**: `Capture UI issues directly in your browser and push them to Linear or Jira in seconds. No calls, no screenshots in Slack, no follow-up threads. Free to start — 25 issues, no card required.`
- **Body paragraphs**: MISSING (none beyond subheading)
- **Feature cards / list items**: MISSING (hero has no cards; interactive CTAs and demo mockup text are in Section 4)

### Section: Problems
- **id**: `problems` — **data-screen-label**: `Problems`
- **Eyebrow / kicker**: MISSING
- **Heading**: `Feedback shouldn't be a full-time job.` (accent span: `a full-time job.`)
- **Subheading (.section-sub)**: `Most bugs don't take long to fix. Explaining them does.`
- **Body paragraphs**: MISSING
- **Feature cards (4 problem cards; title + body + mockup text):**
  1. Card mockup label: `3 places, 0 tickets`
     - `#design-feedback` · `see screenshot 👀 — subscribe-btn.png` · unread `3`
     - `DM · @mike` · `loom.ly/abc123 — "can you fix this?"` · unread `1`
     - `Email · from Sarah` · `FWD: FWD: Bug report — urgent pls`
     - **Title**: `Reports scattered everywhere`
     - **Body**: `Screenshots in Slack, Looms in DMs, repro steps buried in threads.`
  2. Card mockup label: `Thread · 9 messages`
     - `That yellow button is broken` `10:04`
     - `Which screen?` `10:07`
     - `Checkout I think?` `10:09`
     - `Can you share the URL?` `10:11`
     - **Title**: `Endless clarification calls`
     - **Body**: `Another Zoom just to point at a button that’s three pixels off.`
  3. Card mockup ticket: `ISS-0042 · 4 days ago`
     - Ticket title: `Login broken after latest update`
     - `Assignee` `— unassigned`
     - `Priority` `— none set`
     - `Status` `No status`
     - `Project` `— none`
     - **Title**: `No clear ownership`
     - **Body**: `Bugs in chat carry no assignee, no priority, and no status.`
  4. Card mockup: `Bug report · from Slack` · tag `closed`
     - `URL` `not included`
     - `Browser` `not included`
     - `Viewport` `not included`
     - `Console` `no logs attached`
     - **Title**: `Impossible to reproduce`
     - **Body**: `By the time it’s filed, the selector, viewport, and console are gone.`

### Section: How
- **id**: `how` — **data-screen-label**: `How`
- **Eyebrow / kicker**: MISSING
- **Heading**: `Three steps. Seamless reporting.`
- **Subheading (.section-sub)**: `Designed to disappear once you've started using it.`
- **Body paragraphs**: MISSING
- **Feature cards / list items**: MISSING (the three "steps" are rendered as the three feature rows that follow — see below)

### Section: Feature – Annotate
- **id**: MISSING — **data-screen-label**: `Feature – Annotate`
- **Eyebrow / kicker**: MISSING
- **Heading**: `Point at exactly what's broken`
- **Subheading**: MISSING
- **Body paragraph**: `Click anywhere on the page to place a pin. Notate records the element, its CSS selector, and coordinates — so developers know exactly where to look without a single back-and-forth.`
- **List items (.fbullets)**:
  - `Click-to-pin on any DOM element`
  - `Freehand highlight for area annotations`
  - `Multiple pins per report`
- **Mockup text**: browser URL `staging.myapp.com/checkout`; tip `Button: "Checkout"`; `.btn-primary · data-id="checkout-submit"`; pin badge `1`

### Section: Feature – Context
- **id**: MISSING — **data-screen-label**: `Feature – Context`
- **Eyebrow / kicker**: MISSING
- **Heading**: `Context is captured automatically`
- **Subheading**: MISSING
- **Body paragraph**: `No more "what browser were you on?" Notate silently records everything a developer needs to reproduce the issue — before you even type a word.`
- **List items (.fbullets)**:
  - `Browser, OS, and version`
  - `Full URL with all query parameters`
  - `Viewport size and device type`
  - `Console errors at time of capture`
- **Mockup text (ctx-card)**: heading `Captured context`
  - `URL` `staging.myapp.com/checkout?id=xyz`
  - `Browser` `Safari 17.4` badge `macOS`
  - `Viewport` `1440 × 900`
  - `OS` `macOS 14.4 Sonoma`
  - `Console` `2 errors`
  - `Screenshot` `✓ attached`

### Section: Feature – Integrations Detail
- **id**: MISSING — **data-screen-label**: `Feature – Integrations Detail`
- **Eyebrow / kicker**: MISSING
- **Heading**: `One click to Linear or Jira`
- **Subheading**: MISSING
- **Body paragraph**: `Choose your tracker and hit send. Notate creates a complete, well-structured ticket with the annotated screenshot, your comment, labels, and all captured context — no copy-pasting required.`
- **List items (.fbullets)**:
  - `Native Linear & Jira integrations`
  - `Set project, priority, and assignee`
  - `Screenshot auto-attached as an asset`
- **Mockup text (fint-card)**: heading `Creating ticket`
  - Title: `Checkout button unresponsive on Safari`
  - Tags: `Bug` · `Safari` · `High priority` · `Frontend`
  - Meta row: `staging.myapp.com/checkout · Safari 17.4 · 1440×900 · 2 console errors`
  - Buttons: `Push to Jira` · `Push to Linear`

### Section: Features
- **id**: `features` — **data-screen-label**: `Features`
- **Eyebrow / kicker**: MISSING
- **Heading**: `Everything you need. Nothing you don't.` (accent span: `Nothing you don't.`)
- **Subheading (.section-sub)**: `A focused extension. No accounts, no dashboards, no sales calls.`
- **Feature tiles (title + body + mockup text for each):**
  - **Speed tile**
    - Title: `Spotted to filed, in under 5 seconds.` (a non-breaking space `&nbsp;` sits between `filed,` and `in`)
    - Body: `Entirely client-side. No backend round trips. No AI in the hot path. Just a side panel that opens the instant you call it.`
    - Illustration steps: `Pin element` `0ms` · `Screenshot captured` `+1s` · `Comment added` `+3s` · `Filed to Linear` `+240ms`
    - Stat: `start to filed` `4.24s`
  - **Integrations tile**
    - Title: `One click to Linear and Jira.`
    - Body: `Connect once. After that, every pin is one keystroke from filed — in the right project, with the right labels.`
    - Cards: `Linear` `Connected` · `Jira` `Connected`
  - **Lightweight tile**
    - Title: `Smaller than a stock photo.`
    - Body: `No frameworks in your tabs. No tracking scripts. A quiet extension that wakes up when you call it.`
    - Stat: `900` `KB` `installed`
    - Comparison bars: `Notate` `you` `900 KB` · `Avg stock photo` `3.5 MB` · `Typical web app` `18+ MB`
    - Badge: `0% CPU when idle`
  - **Agent tile**
    - Title: `Context for your agents.`
    - Body: `Every ticket lands structured — URL, viewport, selector, console, screenshot — ready for the next agent to pick up.`
    - Code mockup filename: `bug-report.json`
    - Code contents (verbatim):
      - `"title": "Subscribe button stays loading",`
      - `"url": "/dashboard?plan=pro",`
      - `"selector": "[data-testid=cta]",`
      - `"console": "TypeError: undefined",`
      - `"screenshot": "attached.png"`
      - `// ready for any LLM to repro`
    - Cards: `Claude` · `ChatGPT`
  - **Pricing tile** (id: `pricing`)
    - Heading: `Free to start. $7/month when you outgrow it.`
    - Body: `No seats, no per-user math — a generous free tier, then one flat Pro price.`
    - Free plan: `Free` · `$0` · `No card required`
      - `25 issues, lifetime`
      - `Native Linear & Jira sync`
      - `Unlimited seats`
    - Pro plan: `Pro` · toggle `Monthly` / `Annual` · `$7` `/month` · `Billed monthly` · badge `Save 57%` (hidden until Annual selected)
      - `Unlimited issues`
      - `Everything in Free`
      - `Cancel anytime`
    - Pro plan, Annual state (set by JS toggle): `$3` `/month` · `Billed annually` · badge shown `Save 57%`

### Section: Privacy
- **id**: `privacy` — **data-screen-label**: `Privacy`
- **Eyebrow / kicker**: MISSING
- **Heading**: `Your data stays local by default. Cloud is opt-in.`
- **Subheading (.privacy-sub)**: `Everything stays on your device until you press Send. No Notate server in the path — ever.`
- **Flow diagram text** (container is `aria-hidden="true"`):
  - `Your browser` · `Stays local until you send`
  - Tiles: `Pin + element` · `Screenshot` · `URL + viewport` · `Console errors`
  - Connector badge: `TLS`
  - Destination: `Linear` · `via your OAuth token` · `Direct`
  - Destination: `Jira` · `via your OAuth token` · `Direct`
  - Callout: `Notate servers are never in the data path`
- **Assurances (.privacy-assurances)**:
  - `No server-side storage by default`
  - `Encrypted in transit`
  - `Scoped to your own auth`

### Section: Compare
- **id**: `compare` — **data-screen-label**: `Compare`
- **Eyebrow / kicker**: MISSING
- **Heading**: `What you'd usually pay $39–$199/month for. $7.` (accent span: `$7.`)
- **Subheading (.section-sub)**: `Start free with 25 issues. Need more? It's $7/month flat — no seats, no per-user pricing.`
- **Body / table**: comparison table (see Section 6 for full verbatim content)
- **Note (.compare-note)**: `Pricing and features verified from public vendor pages, June 2026. Plans change — these don't.`

### Section: FAQ
- **id**: `faq` — **data-screen-label**: `FAQ`
- **Eyebrow / kicker**: MISSING
- **Heading**: `Questions, answered honestly.` (accent span: `answered honestly.`)
- **Subheading**: MISSING
- **Body**: Q&A list (see Section 5 for full verbatim content)

### Section: CTA
- **id**: `cta` — **data-screen-label**: `CTA`
- **Eyebrow / kicker**: MISSING
- **Heading**: `Stop turning UI issues into long conversations.`
- **Subheading (.final-sub)**: `Install Notate. Pin your first bug in the next thirty seconds.`
- **Body paragraphs**: MISSING
- **Meta row (.hero-meta)**: `Chrome 116+` · `Also works on Brave, Arc & Edge`

## 4. Interactive and micro copy

### Buttons and links (label → href)
- `Notate` (nav brand wordmark) → `#top`
- `Why` → `#problems`
- `How it works` → `#how`
- `Features` → `#features`
- `Pricing` → `#pricing`
- `Compare` → `#compare`
- `FAQ` → `#faq`
- `Add to Chrome` (nav CTA, with chip `Free`) → `https://tinyurl.com/notatelive` (target `_blank`)
- Nav hamburger button → aria-label `Open menu` / `Close menu` (toggled)
- Mobile menu: `Why →` → `#problems`
- Mobile menu: `How it works →` → `#how`
- Mobile menu: `Features →` → `#features`
- Mobile menu: `Pricing →` → `#pricing`
- Mobile menu: `Compare →` → `#compare`
- Mobile menu: `FAQ →` → `#faq`
- Mobile menu: `Add to Chrome` (chip `Free`) → `https://tinyurl.com/notatelive`
- `Add to Chrome` (hero, with chip `FREE`) → `https://tinyurl.com/notatelive`
- `See how it works` (hero) → `#how`
- `Marker.io` (compare table header link) → `https://marker.io`
- `BugHerd` (compare table header link) → `https://bugherd.com`
- `Jam.dev` (compare table header link) → `https://jam.dev`
- `Pastel` (compare table header link) → `https://usepastel.com`
- `Monthly` (pricing toggle button) → no href (button)
- `Annual` (pricing toggle button) → no href (button)
- `Push to Jira` (mockup button) → no href
- `Push to Linear` (mockup button) → no href
- `Add to Chrome` (final CTA) → `https://tinyurl.com/notatelive`
- `See how it works` (final CTA) → `#how`
- Footer AI (icon only, aria-label `Ask ChatGPT`) → `https://chatgpt.com/?q=...` (prefilled question)
- Footer AI (icon only, aria-label `Ask Claude`) → `https://claude.ai/new?q=...` (prefilled question)
- Footer AI (icon only, aria-label `Ask Perplexity`) → `https://www.perplexity.ai/search?q=...` (prefilled question)
- `Notate` (footer brand) → `#top`
- `How it works` (footer Product) → `#how`
- `Features` (footer Product) → `#features`
- `FAQ` (footer Product) → `#faq`
- `Marker.io alternative` (footer Compare) → `/compare/marker-io/`
- `BugHerd alternative` (footer Compare) → `/compare/bugherd/`
- `Jam.dev alternative` (footer Compare) → `/compare/jam/`
- `Pastel alternative` (footer Compare) → `/compare/pastel/`
- `Discord` (footer Community) → `https://discord.gg/2hC7Y22J`
- `Reddit` (footer Community) → `https://www.reddit.com/r/notate_app/`
- `Twitter / X` (footer Community) → `https://x.com/notate_app`
- `notate.developer@gmail.com` (footer Community) → `mailto:notate.developer@gmail.com`
- `Privacy` (footer Legal) → `/privacy/`
- `Terms` (footer Legal) → `/terms/`
- `Support` (footer Legal) → `/support/`

### CTAs (primary / secondary)
- `Add to Chrome` — **primary** (appears in nav, hero, mobile menu, and final CTA; all → `https://tinyurl.com/notatelive`)
- `See how it works` — **secondary** (hero and final CTA; → `#how`)

### Nav item labels
`Why` · `How it works` · `Features` · `Pricing` · `Compare` · `FAQ`

### Badges / pills / tags / chips
- `Chrome extension` (hero eyebrow)
- `Free` (nav CTA chip and mobile CTA chip)
- `FREE` (hero primary CTA chip)
- `3 places, 0 tickets` (problem card 1 label)
- `3`, `1` (unread badges, problem card 1)
- `Thread · 9 messages` (problem card 2 label)
- `closed` (problem card 4 tag)
- `macOS` (context card browser badge)
- `Bug` · `Safari` · `High priority` · `Frontend` (integration mockup tags)
- `Connected` (Linear and Jira integration cards)
- `you` (Lightweight tile pill)
- `0% CPU when idle` (Lightweight tile badge)
- `TLS` (privacy flow connector badge)
- `Direct` (Linear and Jira privacy destination badges)
- `Save 57%` (pricing Pro badge)

### Placeholder / tooltip / aria-label text
- Placeholder: `Describe what's wrong…` (hero composer textarea)
- aria-label: `Notate` (brand logo SVG)
- aria-label: `Open menu` (nav hamburger; toggles to `Close menu`)
- aria-label: `Billing period` (pricing toggle group)
- aria-label: `Ask ChatGPT` (footer AI link)
- aria-label: `Ask Claude` (footer AI link)
- aria-label: `Ask Perplexity` (footer AI link)
- Tooltips (`title=` attributes): MISSING (none present)

### Text inside the demo / animation mockup (hero)
- Browser URL bar: `🔒` `app.yourcompany.com/dashboard`
- Fake page button: `Subscribe`
- Composer textarea value: `Subscribe button stays in loading state after 3s on Safari`
- Composer hint: `⌘` `+` `↵` `to send`
- Send button: `Send to Linear`
- Success toast: `Successfully sent to Linear`
- (JS-driven typing string, identical to textarea value): `Subscribe button stays in loading state after 3s on Safari`

## 5. FAQ content

1. **Q:** `Is Notate free?`
   **A:** `The first 25 issues are free — no card required. After that, Notate Pro unlocks unlimited issues for $7/month, or $3/month billed annually (save 57%). No seats, no per-user pricing, cancel anytime from Settings → Billing.`

2. **Q:** `Where does my data go?`
   **A:** `Straight from your browser into Linear or Jira, over your own auth. We don't read your pages. We don't store pins in our cloud. We don't keep a copy in your browser either.`

3. **Q:** `Does it work on internal tools and localhost?`
   **A:** `Yes. Notate runs on any page Chrome can open — staging, admin dashboards, localhost, VPN'd internal apps.`

4. **Q:** `What gets attached to the ticket?`
   **A:** `A screenshot, the URL, the viewport, the user agent, the selector path of the element you pinned, and any console errors that happened on the page. Structured so a downstream agent can pick it up without further prompting.`

5. **Q:** `How do I get my team on it?`
   **A:** `Send them the Chrome Web Store link. There's nothing to provision, no SSO to configure, no seats to buy. Each person connects their own Linear or Jira and they're in.`

## 6. Comparison / competitor content

### Comparison table (Compare section, verbatim)

Third-party products named as columns: **Marker.io**, **BugHerd**, **Jam.dev**, **Pastel** (compared against **Notate**). Column header links: Marker.io → `https://marker.io`, BugHerd → `https://bugherd.com`, Jam.dev → `https://jam.dev`, Pastel → `https://usepastel.com`.

| Feature | Notate | Marker.io | BugHerd | Jam.dev | Pastel |
|---|---|---|---|---|---|
| `Pin feedback on any live page` | ✓ | ✓ | ✓ | ✓ | ✓ |
| `Native Linear & Jira integration` | ✓ | ✓ | `Jira on premium tier` | ✓ | `via Zapier` |
| `Auto-attached console & DOM context` | ✓ | `Team plan only` | ✓ | ✓ | ✕ |
| `Structured for downstream AI agents` | ✓ | ✕ | ✕ | `paid add-on` | ✕ |
| `Works on localhost & internal apps` | ✓ | ✓ | `via extension` | ✓ | ✕ |
| `Zero data stored on vendor servers` | ✓ | ✕ | ✕ | ✕ | ✕ |

Table note (verbatim): `Pricing and features verified from public vendor pages, June 2026. Plans change — these don't.`

### Other comparative copy
- Compare section heading: `What you'd usually pay $39–$199/month for. $7.`
- Compare section subheading: `Start free with 25 issues. Need more? It's $7/month flat — no seats, no per-user pricing.`
- Lightweight tile size comparison (not third-party products, but comparative): `Notate` `900 KB` vs `Avg stock photo` `3.5 MB` vs `Typical web app` `18+ MB`
- Footer "Compare" column link labels reference the same third parties: `Marker.io alternative`, `BugHerd alternative`, `Jam.dev alternative`, `Pastel alternative`.
- Footer "Ask AI" prefilled prompts (in link hrefs) also read: `How does it compare to Marker.io and BugHerd?`

**All named third-party products across the page:** Marker.io, BugHerd, Jam.dev, Pastel (direct competitors); Linear, Jira, Zapier (referenced within comparison rows); plus (outside the comparison context) Slack, Loom (loom.ly), Zoom, Safari, macOS, Chrome, Brave, Arc, Edge, Claude, ChatGPT, Perplexity, Discord, Reddit, Twitter / X.

## 7. Footer

- **Brand**: `Notate`
- **Tagline paragraph**: `Built by a small team that got tired of pointing at things on Zoom calls. We're solving our own problem first — and yours by extension.`
- **AI section label**: `Ask AI about Notate`
- **AI section link labels (aria-labels; icon-only buttons)**: `Ask ChatGPT` · `Ask Claude` · `Ask Perplexity`
- **Column: Product** (heading `Product`): `How it works` · `Features` · `FAQ`
- **Column: Compare** (heading `Compare`): `Marker.io alternative` · `BugHerd alternative` · `Jam.dev alternative` · `Pastel alternative`
- **Column: Community** (heading `Community`): `Discord` · `Reddit` · `Twitter / X` · `notate.developer@gmail.com`
- **Column: Legal** (heading `Legal`): `Privacy` · `Terms` · `Support`
- **Base line (legal / attribution)**: `© 2026 Notate` · `Made in a browser, for browsers.`
- **Contact details**: email `notate.developer@gmail.com`; Discord `https://discord.gg/2hC7Y22J`; Reddit `https://www.reddit.com/r/notate_app/`; Twitter/X `https://x.com/notate_app`

## 8. Images and media

- **`<img>` elements**: None. The page contains zero `<img>` tags; all in-page imagery is inline `<svg>` or CSS background.
- **`<svg>` with a `<title>` element**: None. No inline SVG uses a `<title>`; SVGs are labelled (if at all) via `aria-label` or are decorative.
- **Content-bearing SVG**:
  - Nav brand logo SVG — accessible name via `aria-label="Notate"` (content-bearing; represents the brand/wordmark). NO ALT (uses aria-label instead).
  - Google Chrome logo SVG (in `Add to Chrome` buttons) — `aria-hidden="true"` (decorative). NO ALT.
  - Linear / Jira / Claude / ChatGPT / Perplexity brand icon SVGs — decorative icons, no text alternative. NO ALT.
  - All other inline SVGs (checkmarks, arrows, cursor, lock, send, etc.) — decorative icons. NO ALT.
- **Background images (CSS)**:
  - `.bg-pattern` — radial-gradient dot texture; decorative. NO ALT.
  - `.bg-glow` — radial-gradient glow; decorative. NO ALT.
  - `.brand-mark` logo — inline SVG data-URI (used as CSS background in two rules); decorative brand mark. NO ALT.
- **Footer brand logo SVG**: `aria-hidden="true"` (decorative; the word `Notate` follows it as text). NO ALT.
- **Referenced media files (in `<head>`, not rendered in body)**:
  - `og:image` / `twitter:image`: `https://notate.live/og-image.png` — social share preview (content-bearing). NO ALT (meta image; alt not applicable).
  - Favicons / icons: `/favicon.ico`, `/icon.svg`, `/favicon-32x32.png`, `/favicon-16x16.png`, `/apple-touch-icon.png` — decorative/brand icons. NO ALT.
  - `/site.webmanifest` — web app manifest (references `icon-192.png`, `icon-512.png`).

## 9. Routing and structure

### Internal links — anchor links (`#…`, same-page)
- `#top` (nav brand, footer brand)
- `#problems` (nav `Why`, mobile menu)
- `#how` (nav `How it works`, mobile menu, hero `See how it works`, final CTA `See how it works`, footer Product)
- `#features` (nav `Features`, mobile menu, footer Product)
- `#pricing` (nav `Pricing`, mobile menu)
- `#compare` (nav `Compare`, mobile menu)
- `#faq` (nav `FAQ`, mobile menu, footer Product)

### Internal links — real routes (`/…`)
- `/compare/marker-io/` (footer `Marker.io alternative`)
- `/compare/bugherd/` (footer `BugHerd alternative`)
- `/compare/jam/` (footer `Jam.dev alternative`)
- `/compare/pastel/` (footer `Pastel alternative`)
- `/privacy/` (footer `Privacy`)
- `/terms/` (footer `Terms`)
- `/support/` (footer `Support`)
- (Resource routes referenced in `<head>`, not navigation): `/favicon.ico`, `/icon.svg`, `/favicon-32x32.png`, `/favicon-16x16.png`, `/apple-touch-icon.png`, `/site.webmanifest`

### Full list of distinct URLs the site currently serves
From `sitemap.xml` (canonical, indexable):
- `https://notate.live/`
- `https://notate.live/changelog/`
- `https://notate.live/support/`
- `https://notate.live/privacy/`
- `https://notate.live/terms/`
- `https://notate.live/compare/marker-io/`
- `https://notate.live/compare/bugherd/`
- `https://notate.live/compare/jam/`
- `https://notate.live/compare/pastel/`

Additional pages present on disk but not in the sitemap:
- `https://notate.live/invite/` — served, but `Disallow: /invite/` in `robots.txt`
- `https://notate.live/uninstall.html` — served, but `Disallow: /uninstall.html` in `robots.txt`
- `https://notate.live/404.html` — error page

Notes: the site is hosted at the custom domain `notate.live` (per `CNAME`). Homepage is NOT listed in the sitemap's internal `/changelog/` link within `index.html` itself (the homepage does not link to `/changelog/` or `/invite/`).

### External links (with domain)
- `https://tinyurl.com/notatelive` — `tinyurl.com` (all `Add to Chrome` CTAs; redirects to the extension)
- `https://marker.io` — `marker.io` (compare table)
- `https://bugherd.com` — `bugherd.com` (compare table)
- `https://jam.dev` — `jam.dev` (compare table)
- `https://usepastel.com` — `usepastel.com` (compare table)
- `https://chatgpt.com/?q=…` — `chatgpt.com` (footer Ask AI)
- `https://claude.ai/new?q=…` — `claude.ai` (footer Ask AI)
- `https://www.perplexity.ai/search?q=…` — `perplexity.ai` (footer Ask AI)
- `https://discord.gg/2hC7Y22J` — `discord.gg` (footer Community)
- `https://www.reddit.com/r/notate_app/` — `reddit.com` (footer Community)
- `https://x.com/notate_app` — `x.com` (footer Community)
- `mailto:notate.developer@gmail.com` — email (footer Community)
- `https://www.googletagmanager.com/gtag/js?id=G-4FFSQR7JYR` — `googletagmanager.com` (analytics script, `<head>`)
- `https://notate.live/og-image.png` — `notate.live` (own domain; og/twitter image)

## 10. Claims audit

### Head metadata
- `Capture UI issues directly in your browser and push them to Linear or Jira in seconds. Free to start — $7/mo for unlimited.` (meta description / og:description / twitter:description)

### Hero
- `Turn screenshots into JIRA tickets in seconds.` (Hero, H1)
- `Chrome extension` (Hero, eyebrow)
- `Capture UI issues directly in your browser and push them to Linear or Jira in seconds.` (Hero, subheading)
- `No calls, no screenshots in Slack, no follow-up threads.` (Hero, subheading)
- `Free to start — 25 issues, no card required.` (Hero, subheading)

### Problems
- `Most bugs don't take long to fix. Explaining them does.` (Problems, subheading)

### Feature – Annotate
- `Click anywhere on the page to place a pin. Notate records the element, its CSS selector, and coordinates — so developers know exactly where to look without a single back-and-forth.` (Feature – Annotate, body)
- `Click-to-pin on any DOM element` (Feature – Annotate, list)
- `Freehand highlight for area annotations` (Feature – Annotate, list)
- `Multiple pins per report` (Feature – Annotate, list)

### Feature – Context
- `Notate silently records everything a developer needs to reproduce the issue — before you even type a word.` (Feature – Context, body)
- `Browser, OS, and version` (Feature – Context, list)
- `Full URL with all query parameters` (Feature – Context, list)
- `Viewport size and device type` (Feature – Context, list)
- `Console errors at time of capture` (Feature – Context, list)

### Feature – Integrations Detail
- `Choose your tracker and hit send. Notate creates a complete, well-structured ticket with the annotated screenshot, your comment, labels, and all captured context — no copy-pasting required.` (Feature – Integrations Detail, body)
- `Native Linear & Jira integrations` (Feature – Integrations Detail, list)
- `Set project, priority, and assignee` (Feature – Integrations Detail, list)
- `Screenshot auto-attached as an asset` (Feature – Integrations Detail, list)

### Features
- `A focused extension. No accounts, no dashboards, no sales calls.` (Features, subheading)
- `Spotted to filed, in under 5 seconds.` (Features, Speed tile title)
- `Entirely client-side. No backend round trips. No AI in the hot path. Just a side panel that opens the instant you call it.` (Features, Speed tile body)
- `start to filed` `4.24s` (Features, Speed tile stat)
- `One click to Linear and Jira.` (Features, Integrations tile title)
- `Connect once. After that, every pin is one keystroke from filed — in the right project, with the right labels.` (Features, Integrations tile body)
- `Smaller than a stock photo.` (Features, Lightweight tile title)
- `No frameworks in your tabs. No tracking scripts. A quiet extension that wakes up when you call it.` (Features, Lightweight tile body)
- `900 KB installed` (Features, Lightweight tile stat)
- `Notate` `900 KB` / `Avg stock photo` `3.5 MB` / `Typical web app` `18+ MB` (Features, Lightweight tile comparison bars)
- `0% CPU when idle` (Features, Lightweight tile badge)
- `Context for your agents.` (Features, Agent tile title)
- `Every ticket lands structured — URL, viewport, selector, console, screenshot — ready for the next agent to pick up.` (Features, Agent tile body)
- `// ready for any LLM to repro` (Features, Agent tile code mockup)
- `Free to start. $7/month when you outgrow it.` (Features, Pricing tile heading)
- `No seats, no per-user math — a generous free tier, then one flat Pro price.` (Features, Pricing tile body)
- `$0` `No card required` (Features, Pricing tile, Free plan)
- `25 issues, lifetime` (Features, Pricing tile, Free plan)
- `Native Linear & Jira sync` (Features, Pricing tile, Free plan)
- `Unlimited seats` (Features, Pricing tile, Free plan)
- `$7` `/month` `Billed monthly` (Features, Pricing tile, Pro plan)
- `$3` `/month` `Billed annually` `Save 57%` (Features, Pricing tile, Pro plan annual state)
- `Unlimited issues` (Features, Pricing tile, Pro plan)
- `Everything in Free` (Features, Pricing tile, Pro plan)
- `Cancel anytime` (Features, Pricing tile, Pro plan)

### Privacy
- `Your data stays local by default. Cloud is opt-in.` (Privacy, heading)
- `Everything stays on your device until you press Send. No Notate server in the path — ever.` (Privacy, subheading)
- `Stays local until you send` (Privacy, flow diagram)
- `via your OAuth token` (Privacy, Linear and Jira destinations)
- `Notate servers are never in the data path` (Privacy, callout)
- `No server-side storage by default` (Privacy, assurances)
- `Encrypted in transit` (Privacy, assurances)
- `Scoped to your own auth` (Privacy, assurances)

### Compare
- `What you'd usually pay $39–$199/month for. $7.` (Compare, heading)
- `Start free with 25 issues. Need more? It's $7/month flat — no seats, no per-user pricing.` (Compare, subheading)
- `Pin feedback on any live page` — Notate ✓, Marker.io ✓, BugHerd ✓, Jam.dev ✓, Pastel ✓ (Compare, table)
- `Native Linear & Jira integration` — Notate ✓, Marker.io ✓, BugHerd `Jira on premium tier`, Jam.dev ✓, Pastel `via Zapier` (Compare, table)
- `Auto-attached console & DOM context` — Notate ✓, Marker.io `Team plan only`, BugHerd ✓, Jam.dev ✓, Pastel ✕ (Compare, table)
- `Structured for downstream AI agents` — Notate ✓, Marker.io ✕, BugHerd ✕, Jam.dev `paid add-on`, Pastel ✕ (Compare, table)
- `Works on localhost & internal apps` — Notate ✓, Marker.io ✓, BugHerd `via extension`, Jam.dev ✓, Pastel ✕ (Compare, table)
- `Zero data stored on vendor servers` — Notate ✓, Marker.io ✕, BugHerd ✕, Jam.dev ✕, Pastel ✕ (Compare, table)
- `Pricing and features verified from public vendor pages, June 2026. Plans change — these don't.` (Compare, note)

### FAQ
- `The first 25 issues are free — no card required.` (FAQ, Q1)
- `After that, Notate Pro unlocks unlimited issues for $7/month, or $3/month billed annually (save 57%).` (FAQ, Q1)
- `No seats, no per-user pricing, cancel anytime from Settings → Billing.` (FAQ, Q1)
- `Straight from your browser into Linear or Jira, over your own auth.` (FAQ, Q2)
- `We don't read your pages. We don't store pins in our cloud. We don't keep a copy in your browser either.` (FAQ, Q2)
- `Yes. Notate runs on any page Chrome can open — staging, admin dashboards, localhost, VPN'd internal apps.` (FAQ, Q3)
- `A screenshot, the URL, the viewport, the user agent, the selector path of the element you pinned, and any console errors that happened on the page. Structured so a downstream agent can pick it up without further prompting.` (FAQ, Q4)
- `Send them the Chrome Web Store link. There's nothing to provision, no SSO to configure, no seats to buy.` (FAQ, Q5)
- `Each person connects their own Linear or Jira and they're in.` (FAQ, Q5)

### CTA
- `Install Notate. Pin your first bug in the next thirty seconds.` (CTA, subheading)
- `Chrome 116+` (CTA, meta row)
- `Also works on Brave, Arc & Edge` (CTA, meta row)

### Footer
- `Built by a small team that got tired of pointing at things on Zoom calls. We're solving our own problem first — and yours by extension.` (Footer, tagline)
- `Made in a browser, for browsers.` (Footer, base line)
- `© 2026 Notate` (Footer, base line)
