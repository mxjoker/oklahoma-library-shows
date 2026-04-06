# Project Context — Oklahoma Library Shows

## Business Overview
- **Owner:** Joe Coover
- **Business name:** Funky Monkey Events
- **Performer name:** Joe Coover
- **Location:** Oklahoma City, OK
- **Phone:** (405) 431-6625
- **Email:** joe.coover@gmail.com
- **Website ecosystem:**
  - funkymonkeyevents.com — overall brand hub (all services)
  - funkymonkeymagic.com — magic-specific landing page
  - oklahomalibraryshows.com — THIS SITE (library-facing only)

## Brand Identity
- **Logo:** "FUNKY MONKEY" in bold chunky cyan/turquoise with thick black outlines,
  hot pink lightning bolt accent, monkey mascot in pink sunglasses — comic book / pop art style
- **Primary colors:** Bright cyan (#00C2E0), hot pink (#E8306A), navy (#1B2A4A)
- **Style:** Bold, high-energy, warm and friendly but professional
- **Fonts:** Poppins (headings, 900 weight), Lato (body)
- **Tone:** Approachable, energetic, educator-aware — speaks librarian language

## Target Audience
- Children's librarians and library directors in Oklahoma and surrounding states
- Decision-makers spending public funds — risk-averse, budget-conscious
- Planning summer reading programs (January–April booking season)
- Affiliated with CSLP (Collaborative Summer Library Program) theme planning
- Part of Oklahoma Library Association and Oklahoma Department of Libraries networks

## The Six Programs
All programs: $385 per program, 45–60 minutes, in-person, audience: Children (or All Ages)

| Program | ODL Title | Key Feature |
|---------|-----------|-------------|
| Magic Show | Dinosaur Adventure: Magic Show | Tied to 2026 "Unearth a Story" CSLP theme |
| Bubble Show | Professor Buckets Bubble Show | STEAM — science of bubbles, Kid-in-a-Bubble finale |
| Magic Workshop | Hands-on Magic Trick Workshop | Kids learn tricks to perform — builds confidence |
| Balloon Workshop | Hands-on Balloon Twisting Workshop | All ages, tangible creation to take home |
| Story Doodles | Story Doodles Draw-Along | Live drawing + storytelling — unique literacy program |
| Foam Party | Foam Party Celebration | OUTDOOR ONLY — subject to separate foam calendar |

### Foam Party Notes
- Only outdoor show — must be noted clearly everywhere
- Has a separate "foam calendar" managed by Joe
- Booking flow should flag this and note dates are confirmed separately
- Future: may integrate a calendar embed on the foam party page

### Performer Availability Notes (Internal — not shown on site)
- Some shows can be performed by multiple performers simultaneously
- Some shows (e.g. Story Doodles) are single-performer only
- Joe handles scheduling manually — site is inquiry-only, not live booking
- Peak season: 1–20 shows per week during summer (avg ~5–10/week)


## Service Area
- **Primary:** All of Oklahoma — no travel fee in OKC/Tulsa metro areas
- **Secondary (travel fee applies):** Texas, Kansas, Arkansas, Missouri
- Rural Oklahoma libraries are a high-value segment — underserved, reliable demand

## Booking Flow (Key Decisions Made)
1. Site is **inquiry-based, not live booking** — Joe reviews and responds manually
2. Joe may suggest alternative dates in follow-up conversations
3. Booking form collects: library name, contact name/title, email, phone, city, state,
   show requests (show + date + morning/afternoon preference), notes
4. **Show Request Builder** allows multiple shows on multiple dates in one submission
5. Foam Party shows special outdoor alert when selected
6. Live summary shows all requests before submit
7. "Check availability" CTA is persistent — appears in nav and on every page
8. Modal opens from any CTA; pre-selects the show if clicked from a show card
9. Payment note: "We accept purchase orders and checks" — libraries don't use credit cards
10. Response promise: "We respond within 24 hours"

## What Was Deliberately NOT Built (and Why)
- **No real-time availability calendar** — Joe wants human touch to upsell, suggest alternatives
- **No individual library landing pages** — 550+ OK libraries would be unmaintainable
- **No e-commerce/payment processing** — libraries pay by PO or check after the event
- **No separate CSS files** — keeping everything in HTML for simplicity during initial build

## Existing Library References (Real — Use in Testimonials)
| Name | Title | Library System | Phone | Email |
|------|-------|---------------|-------|-------|
| Kelsey Williamson | Youth Services | Norman Public Library East / Pioneer Library System | (405) 794-3773 | kwilliamson@pioneerlibrarysystem.org |
| Jennifer Fuller | — | Eastern Oklahoma Library System, Muskogee | (918) 682-6657 | jfuller@eols.org |

## CSLP Themes
- **2026 (current):** "Unearth a Story" — dinosaur/archaeology theme
- **2027 (upcoming):** "Mysteries Await at Your Library" — mystery, detective, suspense theme
  - All shows being adapted for mystery/detective theme for 2027
  - 2027 SEO campaign underway — see docs/pages/2027-summer-reading.md
  - Update all shows and CSLP banners when transitioning to 2027 season

## SEO Strategy
Full strategy in docs/seo-strategy.md. Summary:
- Primary targets: Oklahoma city/region searches + show-specific keywords
- 2027 campaign: publish 2027 content NOW before any competitor does
- Geographic pages: OKC, Tulsa, Eastern OK, Rural OK, TX (Dallas + Wichita Falls), KS, AR, MO
- Resources hub with email capture for newsletter list building
- Full keyword list and on-page rules in docs/seo-strategy.md

## Annual Maintenance Tasks
- [ ] Update CSLP theme in green banner (top of every page) — new theme each year
- [ ] Update ODL program catalog submissions (Joe submits these separately)
- [ ] Refresh testimonials with new librarian quotes each season
- [ ] Add newly served libraries to the "Libraries We've Served" grid
- [ ] Update pricing if it changes from $385

## Current Build Status
See docs/build-order.md for full prioritized build sequence.

| Page | Status | Notes |
|------|--------|-------|
| index.html (homepage) | ✅ Complete | Needs meta tags + schema added |
| 2027-summer-reading.html | 🔜 Spec ready | **Build this first** — early SEO advantage |
| faq.html | 🔜 Spec ready | Phase 2 |
| service-area.html | 🔜 Spec ready | Phase 2 |
| shows/bubble-show.html | 🔜 Spec ready | Phase 3, priority 1 |
| shows/magic-show.html | 🔜 Spec ready | Phase 3, priority 2 |
| shows/foam-party.html | 🔜 Spec ready | Phase 3, priority 3 |
| shows/story-doodles.html | 🔜 Spec ready | Phase 3, priority 4 |
| shows/magic-workshop.html | 🔜 Spec ready | Phase 3, priority 5 |
| shows/balloon-workshop.html | 🔜 Spec ready | Phase 3, priority 6 |
| locations/tulsa.html | 🔜 Spec ready | Phase 4, priority 1 |
| locations/eastern-oklahoma.html | 🔜 Spec ready | Phase 4, priority 2 |
| locations/oklahoma-city.html | 🔜 Spec ready | Phase 4, priority 3 |
| locations/rural-oklahoma.html | 🔜 Spec ready | Phase 4, priority 4 |
| locations/dallas.html | 🔜 Spec ready | Phase 4, priority 5 |
| locations/wichita-falls.html | 🔜 Spec ready | Phase 4, priority 6 |
| locations/texas.html | 🔜 Spec ready | Phase 4, priority 7 |
| locations/kansas.html | 🔜 Spec ready | Phase 4, priority 8 |
| locations/arkansas.html | 🔜 Spec ready | Phase 4, priority 9 |
| locations/missouri.html | 🔜 Spec ready | Phase 4, priority 10 |
| about.html | 🔜 Spec ready | Phase 5 — needs Joe's story content |
| booking.html | 🔜 Spec ready | Phase 5 |
| contact.html | 🔜 Not started | Phase 5 |
| resources/index.html | 🔜 Spec ready | Phase 5 |
| resources/how-to-book-a-performer.html | 🔜 Spec ready | Phase 5 |
| resources/summer-reading-planning-guide.html | 🔜 Spec ready | Phase 5 |
| sitemap.xml | 🔜 Not started | Technical — build in Phase 1 |
| robots.txt | 🔜 Not started | Technical — build in Phase 1 |
