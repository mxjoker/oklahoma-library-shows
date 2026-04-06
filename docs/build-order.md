# Build Order — Oklahoma Library Shows

Ordered by SEO impact × effort ratio. Build in this sequence.

---

## Phase 1 — Technical Foundation (do before any new pages)
These don't require content but unlock all future SEO value.

| Task | File | Why First |
|------|------|-----------|
| Add meta tags to index.html | index.html | Site is live but currently invisible to Google |
| Create robots.txt | robots.txt | Tells crawlers what to index |
| Create sitemap.xml | sitemap.xml | Speeds up indexing of all pages |
| Add LocalBusiness schema | index.html + contact.html | Local SEO signal |
| Set up Netlify Forms on booking modal | index.html | Form submissions currently go nowhere |
| Set up Google Analytics 4 | All pages (shared nav script) | Need baseline data before traffic arrives |
| Connect to Google Search Console | External | Verify domain, submit sitemap |
| Link site on FME Google Business Profile | External (GBP dashboard) | Fastest local SEO signal |

---

## Phase 2 — High-Value SEO Pages (build immediately)

### 1. `2027-summer-reading.html` ← **Build this first**
- Targets "2027 summer reading program" before ANY competitor
- Low competition right now, high competition later — early advantage is huge
- Can go live with minimal content and expand over time
- See: docs/pages/2027-summer-reading.md

### 2. `faq.html`
- Targets voice search and featured snippets
- Covers questions librarians actually Google
- Easy to write, no photos needed
- See: docs/pages/faq.md

### 3. `service-area.html`
- Currently missing — several keywords rely on this page existing
- Enables rural cluster links and travel fee transparency
- See: docs/pages/service-area.md

---

## Phase 3 — Show Pages (all 6, in this order)

Priority based on search volume + differentiation opportunity:

| Order | Page | Reason |
|-------|------|--------|
| 1 | bubble-show.html | "Bubble show" is a high-volume, differentiated search |
| 2 | magic-show.html | Most common show type — lots of competing searches |
| 3 | foam-party.html | Unique — only outdoor option, strong summer keyword |
| 4 | story-doodles.html | Unique program, low competition, easy to rank |
| 5 | magic-workshop.html | Workshop keyword is strong for literacy-focused librarians |
| 6 | balloon-workshop.html | Completes the set, lower search volume |

See: docs/pages/shows/ for individual specs.

---

## Phase 4 — Location Pages (build in this order)

| Order | Page | Reason |
|-------|------|--------|
| 1 | locations/tulsa.html | Bulk-booking behavior — high ROI per booking |
| 2 | locations/eastern-oklahoma.html | Same bulk-booking behavior, underserved online |
| 3 | locations/oklahoma-city.html | Largest market, highest search volume |
| 4 | locations/rural-oklahoma.html | Unique cost-savings angle, no competition |
| 5 | locations/dallas.html | Largest out-of-state market |
| 6 | locations/wichita-falls.html | Easy to rank for, close to border |
| 7 | locations/texas.html | State overview page (links to Dallas + WF) |
| 8 | locations/kansas.html | State overview |
| 9 | locations/arkansas.html | State overview |
| 10 | locations/missouri.html | State overview |

See: docs/pages/locations/ for individual specs.

---

## Phase 5 — Supporting Pages

| Page | Notes |
|------|-------|
| about.html | Joe's story, credentials, photos — needs Joe's input |
| resources/index.html | Hub page — can go live with 1 resource then expand |
| resources/how-to-book-a-performer.html | Free content, no email gate — good backlink target |
| resources/summer-reading-planning-guide.html | Gated — email capture — builds newsletter list |
| booking.html | Dedicated booking page (modal exists on all pages, this is a standalone version) |
| contact.html | Simple — low effort, complete the site |

---

## Phase 6 — Annual Maintenance (each January)
- [ ] Update CSLP theme banner on all pages
- [ ] Update show names/descriptions for new theme year
- [ ] Archive current year 2027 page → create 2028 page
- [ ] Update ODL program descriptions in references.md
- [ ] Refresh testimonials with new librarian quotes
- [ ] Add newly served libraries to homepage + location pages
- [ ] Re-submit sitemap.xml to Google Search Console

---

## Status Tracker
| Page | Spec Written | Built | Live | SEO Tags | Schema |
|------|-------------|-------|------|----------|--------|
| index.html | ✅ | ✅ | ✅ | ❌ | ❌ |
| 2027-summer-reading.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| faq.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| service-area.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| shows/bubble-show.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| shows/magic-show.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| shows/foam-party.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| shows/story-doodles.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| shows/magic-workshop.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| shows/balloon-workshop.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| locations/tulsa.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| locations/eastern-oklahoma.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| locations/oklahoma-city.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| locations/rural-oklahoma.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| locations/dallas.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| locations/wichita-falls.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| locations/texas.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| locations/kansas.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| locations/arkansas.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| locations/missouri.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| about.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| booking.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| contact.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| resources/index.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| resources/how-to-book-a-performer.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| resources/summer-reading-planning-guide.html | ✅ | ❌ | ❌ | ❌ | ❌ |
| sitemap.xml | ❌ | ❌ | ❌ | — | — |
| robots.txt | ❌ | ❌ | ❌ | — | — |
