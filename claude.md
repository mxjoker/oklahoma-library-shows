# Claude Instructions — Oklahoma Library Shows

## Project Overview
This is a dedicated library booking website for Joe Coover (Funky Monkey Events) targeting
librarians in Oklahoma and surrounding states. The site handles summer reading program bookings.
URL: www.oklahomalibraryshows.com

## Your Role
You are building and maintaining this website. Always read this file and context.md before
starting any work. Ask clarifying questions if requirements are unclear before writing code.

## Core Principles
- This site speaks ONLY to librarians — not parents, not schools, not general audiences
- Every design and copy decision should make a librarian's job easier
- The booking flow is intentionally an INQUIRY system (not real-time booking)
- Joe reviews all requests manually and responds within 24 hours to suggest dates
- Keep the site fast, clean, and mobile-friendly at all times

## Tech Stack
- Pure HTML, CSS, JavaScript — no frameworks, no build tools
- Google Fonts: Poppins (headings) + Lato (body) loaded via CDN
- No external JS libraries unless absolutely necessary
- All pages are standalone .html files in the project root

## Design System
Always use these exact CSS variables — never hardcode colors:
```
--cyan:    #00C2E0   (primary brand — headings, CTAs, links)
--cyan-d:  #009AB3   (hover state for cyan elements)
--pink:    #E8306A   (accent — buttons, highlights, show tags)
--pink-d:  #C0165A   (hover state for pink elements)
--navy:    #1B2A4A   (dark backgrounds, nav, hero)
--green:   #2A6041   (CSLP banner, outdoor tags, trust elements)
--white:   #FFFFFF
--cream:   #F7FAFA   (alternating section backgrounds)
--gray:    #5A6A7A   (body copy, secondary text)
--light:   #E8F8FB   (light cyan tint — card backgrounds, tags)
--border:  #D0EBF0   (all borders)
```

## Typography Rules
- Headings: Poppins, font-weight 900 (h1/h2) or 700 (h3/h4)
- Body: Lato, font-size 14–16px, line-height 1.65–1.75
- Section labels: 11–12px, uppercase, letter-spacing 2px, color var(--pink)
- Minimum font size: 12px anywhere on site
- Use clamp() for responsive heading sizes

## Layout Rules
- Max content width: 1100px, centered with margin: 0 auto
- Section padding: 5rem 2rem (desktop), 3rem 1.25rem (mobile)
- All sections alternate between #fff and var(--cream) backgrounds
- Border radius: 16px for cards, 50px for pills/buttons, 10–12px for tags
- Cards always have box-shadow: 0 2px 12px rgba(27,42,74,0.07)

## Navigation
- Fixed nav, height 64px, background var(--navy)
- Logo: "Oklahoma" in var(--cyan), "Library Shows" in var(--pink), Poppins 900
- "Check availability" button always visible in nav — opens booking modal
- On mobile (≤768px): hide nav links except the CTA button

## Booking Modal Rules
- Modal opens on ANY "Check availability" / "Book this show" / "Check foam dates" click
- When opened from a specific show card, that show pre-selects in the first request
- Show Request Builder: librarian adds one show request at a time (show + date + time pref)
- Foam Party auto-shows outdoor alert when selected
- Live summary updates as librarian fills in requests
- Success state shown after form submit (no actual backend yet — placeholder)
- Close on: X button, clicking overlay background, pressing Escape key


## Booking Modal Rules
- Form uses Netlify Forms (data-netlify="true") — submits to joe.coover@gmail.com
- See docs/forms/booking-modal.md for full field spec and Netlify implementation
- Future: migrate to HubSpot (keep field names identical for easy swap)

## File Structure
Full spec in docs/site-architecture.md. Summary:
```
oklahoma-library-shows/
├── index.html                        ✅ COMPLETE (add meta tags + schema)
├── 2027-summer-reading.html          🔜 BUILD FIRST — highest SEO priority
├── faq.html                          🔜
├── service-area.html                 🔜
├── about.html                        🔜
├── booking.html                      🔜
├── contact.html                      🔜
├── sitemap.xml                       🔜
├── robots.txt                        🔜
├── shows/
│   ├── bubble-show.html              🔜 (build first of shows)
│   ├── magic-show.html               🔜
│   ├── foam-party.html               🔜 (outdoor only, foam calendar)
│   ├── story-doodles.html            🔜
│   ├── magic-workshop.html           🔜
│   └── balloon-workshop.html         🔜
├── locations/
│   ├── tulsa.html                    🔜 (build first of locations)
│   ├── eastern-oklahoma.html         🔜
│   ├── oklahoma-city.html            🔜
│   ├── rural-oklahoma.html           🔜
│   ├── dallas.html                   🔜
│   ├── wichita-falls.html            🔜
│   ├── texas.html                    🔜
│   ├── kansas.html                   🔜
│   ├── arkansas.html                 🔜
│   └── missouri.html                 🔜
├── resources/
│   ├── index.html                    🔜
│   ├── how-to-book-a-performer.html  🔜
│   └── summer-reading-planning-guide.html 🔜
├── docs/                             ✅ planning specs (not served to public)
├── claude.md                         ✅ this file
├── context.md                        ✅ project context
└── references.md                     ✅ references and resources
```

## Individual Show Page Template
Every show page must include these sections in order:
1. Nav (same as homepage)
2. CSLP banner (same as homepage)
3. Show hero — large title, one-line hook, "Book this show" CTA
4. Program overview — 2–3 sentence description connecting to CSLP theme
5. What happens — narrative of the show experience
6. Educational connections — CSLP tie-in, STEAM/literacy/learning outcomes
7. Show details grid — duration, age range, audience size, indoor/outdoor, setup time
8. Librarian testimonials — 2–3 specific to this show
9. Photo/video placeholder section
10. "Book this show" CTA band
11. Footer (same as homepage)

## CSLP Theme (Updated Annually)
- **2026 (current):** "Unearth a Story" (dinosaur/archaeology)
- **2027 (upcoming):** "Mysteries Await at Your Library" (mystery/detective/suspense)
Update the green CSLP banner at top of every page each year.
Banner copy: `[Year] CSLP Theme: "[Theme Name]" | Now booking [year] & [year+1]`

## Coding Standards
- Write CSS in <style> blocks within each HTML file (no separate .css files yet)
- Use BEM-inspired class names: .card-header, .card-body, .card-footer
- Mobile-first responsive using @media(max-width: 768px) and @media(max-width: 600px)
- All buttons must have :hover states with transition: 0.2s
- All interactive elements must be keyboard accessible
- Test every page at 375px (mobile) and 1280px (desktop) widths
