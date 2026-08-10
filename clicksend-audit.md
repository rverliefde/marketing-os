# ClickSend.com — UI Pattern Inventory

**Site:** https://www.clicksend.com
**Audited:** 2026-05-29
**Method:** Page scrape + markdown conversion across 8 representative URLs spanning every distinct template (homepage, product landing, sub-product/use-case, pricing, solutions overview, industries overview, industry detail).

> **Coverage note:** Unlike the ClickSend *blog*, the marketing site is server-rendered, so full body content was captured — including FAQ accordions, step sections, pricing tables, and interactive components. This inventory is therefore body-complete (no JS-render gap).

---

## 1. Page Templates

**8 distinct templates** identified:

| # | Template | Example URL | Purpose |
|---|----------|-------------|---------|
| T1 | **Homepage** | `/` | Company positioning, multi-section magazine layout |
| T2 | **Product landing** | `/en/sms/` | Top-level product (SMS/MMS/Rich Messaging) |
| T3 | **Sub-product / use-case landing** | `/en/sms/sms-marketing/` | Feature-specific (Bulk, Email-to-SMS, SMS API, SMS Marketing) |
| T4 | **Pricing** | `/en/pricing/` | Multi-product pricing with calculators |
| T5 | **Solutions overview** | `/en/solutions/` | Card-grid directory of use cases |
| T6 | **Industries overview** | `/en/industries/` | Card-grid directory of industries |
| T7 | **Detail page (industry/solution)** | `/en/industries/healthcare/` | Long-form narrative for one industry/solution |
| T8 | **External sub-apps** | `dashboard.`, `developers.`, `integrations.`, `help.`, `blog.`, `status.`, `trust.` | Separate subdomains (login, docs, marketplace, help, blog, status) |

**Pattern:** Two families — **overview/directory templates** (T5, T6: scannable card grids) and **detail/narrative templates** (T2, T3, T7: long-form, alternating rows, FAQs). All share one global header/footer shell.

---

## 2. Navigation Patterns

### Global Header (all pages)
- **Logo:** ClickSend, top-left → home.
- **Primary nav with mega-menu dropdowns:**
  - **Products** ▾ — Business SMS (→ Bulk SMS, Email to SMS, SMS API, SMS Marketing), Business MMS, Rich Messaging
  - **Integrations**
  - **Developers**
  - **Pricing**
  - **Resources** ▾ — Solutions, Industries, Help Guides, Blog, Videos, Contact Us
- **Right-side utility cluster:**
  - **Language / region selector** — "English – Global" with flag icon (→ `/en/region-select/`)
  - **Login** button (→ `dashboard.clicksend.com/login`)
  - **Sign Up** button (→ `dashboard.clicksend.com/signup`)
- **Mobile:** hamburger collapse.

### Secondary navigation patterns
- **Breadcrumb chevrons** on sub-product pages (e.g. Business SMS › SMS Marketing).
- **Product tabs** on pricing (SMS / MMS / Voice / Email / Fax / Post).
- **Code-sample language tabs** on homepage (NodeJS, Python, Java, C#, PHP, Ruby, Swift).
- **In-page CTA anchors** linking out to dashboard signup / book-a-demo.
- No breadcrumbs on overview or detail pages beyond the sub-product chevron.

---

## 3. Hero Types

| Hero | Where | Composition |
|------|-------|-------------|
| **H-A: Split marketing hero** | Homepage (T1) | Headline ("Business Communications. Solved.") + subhead + dual CTA ("Get sending for free" / "Book a demo") + dev link, large product imagery on right, **customer logo strip** below (PepsiCo, Re/Max, Denton County, F45, Specsavers, GoStudent). |
| **H-B: Product hero** | Product / sub-product (T2, T3) | Headline + subhead + primary CTA ("Start trial" / "Get Started for Free") + benefit bullets + illustration/handset mockup. "No credit card" microcopy. |
| **H-C: Directory hero** | Overview pages (T5, T6) | Compact: page title ("Solutions" / "Industries") + one-line subhead + single CTA ("Get Sending For Free") + **review badge** ("2026 Best Value SMS Gateway, 5 stars"). |
| **H-D: Detail hero** | Detail pages (T7) | Title ("Text Messaging for Healthcare") + subhead + industry icon + primary CTA + "Contact Us" secondary + review badge. |
| **H-E: Pricing hero** | Pricing (T4) | Promo banner ("50% extra free on first top-up") above headline ("Send and save on _SMS pricing_") + value props (volume discounts, no subscriptions, free inbound). |

---

## 4. Card Types

| Card | Used in | Fields |
|------|---------|--------|
| **C1: Product card** | Homepage | Title + headline + 3-bullet feature list + dual CTA ("Get Sending" / "Read API Docs"). 3-up. |
| **C2: Capability card** | Product page (T2) | Icon + heading + description + right-chevron + sub-links. Stacked vertically. |
| **C3: Benefit card** | Homepage, sub-product | Icon + heading + short text (e.g. "Global 24/7 Support", "99.95% Uptime SLA", "98% open rate"). 3-up. |
| **C4: Solution card** | Solutions overview (T5) | Icon (bell/padlock/rocket) + title + 1–2 sentence description + whole-card link. Flat grid. |
| **C5: Industry card** | Industries overview (T6) | Industry SVG icon + title + (minimal/no description) + card link. **3–4 column grid, ~24 cards.** |
| **C6: Pricing tier card** | Pricing (T4) | Tier name (Boost/Growth/Scale/Enterprise) + savings % + per-message rate + min top-up + value prop + "Free trial" CTA. 4 horizontal tiers. |
| **C7: SMS template card** | Detail page (T7) | Pre-written message with `{variables}` + **"Copy Text" button**. |

**Cross-cutting:** Cards are icon-led and benefit-oriented. Two consistent CTA conventions inside cards: a **business path** ("Get Sending"/"Get Started") and a **developer path** ("Read API Docs").

---

## 5. CTAs

| CTA | Type | Copy | Placement |
|-----|------|------|-----------|
| **Sign Up / Login** | Header buttons | — | Global nav (every page) |
| **"Get sending for free" / "Get Started for Free"** | Primary | Repeated 2×+ per page | Hero + end-of-page banner |
| **"Book a demo"** | Secondary | → `try.clicksend.com/en/book-a-demo/` | Homepage hero |
| **"Read API Docs"** | Tertiary/dev | → `developers.clicksend.com` | Product cards, dev sections |
| **"Visit Dashboard" / "Visit Marketplace"** | Tertiary | — | Homepage feature sections |
| **"Free trial" / "Try for free"** | Primary | On every pricing tier + product section | Pricing (T4) |
| **"Speak to the sales team"** | Secondary | Enterprise tier | Pricing |
| **"Register your interest"** | Primary | Rich Messaging (RCS/WhatsApp/Messenger) | Homepage product card |
| **End-of-page banner** | Section CTA | "Get Sending with ClickSend" / "Let's do this" / "Questions" + "Join over 90,000 customers…" | Bottom of nearly every template |

**Pattern:** Single dominant conversion goal — **free trial signup** (`dashboard.clicksend.com/signup`) — reinforced by (a) persistent header button, (b) hero CTA, (c) a near-universal closing banner. A consistent **dual-path** secondary funnel: *developers* → API docs, *enterprise* → book demo / sales.

---

## 6. Footer Structure

Consistent across all pages:

- **Brand block:** ClickSend logo + **region selector** ("English (World)" + region-select link) + address ("Level 8, 150 Lonsdale Street, Melbourne VIC 3000") with location/building icons.
- **Link columns:**
  - **Company** — About, Careers, Why Choose ClickSend, Partnership program, Affiliate program
  - **Products** — SMS, MMS, Rich Messaging
  - **Pricing** — SMS/MMS Pricing, Rich Messaging Pricing
  - **API & Docs** — Blog, API Docs, Developer Portal, Security, Trust Centre, Knowledge base
  - **Contact Us** — Support, Service Status, Legal / GDPR
- **Social icons:** X (Twitter), LinkedIn, Facebook, Instagram
- **Legal bar:** "Privacy & Legal" + "© 2026 ClickSend"

*(Note: footer mirrors the blog footer but adds Affiliate program / Why Choose ClickSend and a region selector; Trust Centre points to `trust.sinch.com`.)*

---

## 7. Recurring UI Elements

- **Trust signals (heavily recurring):** Trustpilot reference, Capterra & G2 badges, "2026 Best Value SMS Gateway" 5-star review badge, "99.95% uptime SLA", "Over 90,000 customers", "billions of messages", "Global 24/7 Support".
- **Customer logo strip** — 6 brand logos in homepage hero.
- **Review badge** — star-rated award badge on overview/detail heroes.
- **Language/region selector** — header (flag) + footer (text link).
- **Tabs** — code-language tabs (home), product tabs (pricing).
- **FAQ accordion** — expandable Q&A on sub-product (T3, ~7 Qs) and product pages (T2 shows static-expanded format); compliance/best-practice oriented.
- **How-it-works numbered steps** — 3-step centered sequence with graphics (sub-product pages).
- **Alternating image/text feature rows** — detail & sub-product pages.
- **"Copy Text" button** — on pre-written SMS template cards (detail pages).
- **Pricing calculators** — currency dropdown + volume estimator slider (pricing).
- **Promo banners** — top-of-page offer bars with "[T&Cs apply]" (pricing).
- **Deprecation notices** — collapsible sunset notices for Voice/Email/Fax/Post (pricing), redirecting to Mailgun/Sinch.
- **Benefit-bullet checklists** — blue-check feature lists.
- **Icon system** — SVG icons throughout (nav, cards, social, chevrons, industry/solution glyphs).
- **Sidebar-less, full-width** layout on every template.

### Notable observations
- **No interactive testimonial carousel** observed — social proof is delivered via logo strips, stats, and third-party badges rather than embedded quotes.
- **Detail pages favor narrative over visual cards** — long-form problem/solution copy + copy-paste templates, fewer icon blocks.
- **Pricing is the most component-dense template** — tabs + slider + currency selector + tier cards + included-benefits matrix + deprecation accordions.

---

## 8. Quick Findings Summary

1. **One global shell** (mega-menu header + region-aware footer) wraps two template families: scannable **overview grids** (solutions, industries) and long-form **detail/product narratives**.
2. **Relentless single funnel:** every template opens and closes with a free-trial CTA; "Join over 90,000 customers" is the recurring closing refrain.
3. **Dual-audience CTAs:** business ("Get Sending") and developer ("Read API Docs") paths coexist on most product surfaces; enterprise gets a sales/demo path.
4. **Trust-signal saturation:** Trustpilot/Capterra/G2, award badge, uptime SLA, and customer-count stats appear across nearly every template.
5. **Card design is icon-led and benefit-first** — consistent across product, solution, industry, and benefit variants.
6. **Pricing is uniquely interactive** (tabs, currency dropdown, volume slider) and carries multi-product + deprecation logic the rest of the site doesn't.
7. **i18n is first-class** — `/en/` path prefix, header flag selector, footer region-select; pricing localizes currency.

---

## Appendix — Crawled & Discovered URLs

**Templates audited:**
`/` · `/en/sms/` · `/en/sms/sms-marketing/` · `/en/pricing/` · `/en/solutions/` · `/en/industries/` · `/en/industries/healthcare/`

**Top-level nav / products:**
`/en/products/` · `/en/sms/` · `/en/sms/bulk-sms/` · `/en/sms/email-to-sms/` · `/en/sms/sms-gateway-api/` · `/en/sms/sms-marketing/` · `/en/mms/` · `/en/rich-messaging/` · `/en/pricing/` · `/en/solutions/` · `/en/industries/`

**Solution detail pattern:** `/solutions/{slug}/` — e.g. `/solutions/alerts-and-notifications/`, `/solutions/2-factor-authentication-otp/` (~10 cards)

**Industry detail pattern:** `/en/industries/{slug}/` — ~24 industries incl. automotive, banking-finance, beauty-hair, call-centres, ecommerce, education, emergency-services, government, healthcare, human-resources, information-technology, insurance, manufacturing, marketing, not-for-profit, real-estate, restaurants-bars, retail, sport-fitness, telecommunications, transport-logistics, travel-hotels, utilities.

**Company / footer:** `/en/company/` · `/en/careers/` · `/en/clicksend-comparison/` · `/en/partnership-program/` · `/en/affiliate-program/` · `/en/security/` · `/en/legal/` · `/en/region-select/` · `/en/help/`

**External subdomains:** `dashboard.clicksend.com` (login/signup) · `developers.clicksend.com` (+ `/docs/`) · `integrations.clicksend.com` · `help.clicksend.com` · `blog.clicksend.com` · `status.clicksend.com` · `trust.sinch.com` · `try.clicksend.com/en/book-a-demo/`

**Social:** twitter.com/ClickSendSMS · linkedin.com/company/clicksend · facebook.com/Click.Send.SMS · instagram.com/clicksend
