# Page Spec: Booking Page

**File:** `booking.html`
**URL:** `/booking`

---

## SEO
- **Primary keyword:** `book oklahoma library entertainer`
- **Secondary:** `oklahoma library show booking form`, `funky monkey events booking`, `library summer reading program booking oklahoma`
- **Title tag:** `Book a Library Show | Oklahoma Library Shows — Funky Monkey Events`
- **Meta description:** `Submit a booking inquiry for your Oklahoma library's summer reading program. Joe responds within 24 hours. $385 per program. Purchase orders accepted. (405) 431-6625.`

---

## Page Purpose
The dedicated booking page for librarians who land here from search or direct links.
It contains the same form as the modal but in a standalone full-page format — better for
librarians who want to read and fill out the form without a modal overlay.

Also useful for: direct links in email, direct links from Joe's GMB listing, and librarians
who bookmark it for easy access during planning season.

---

## Sections

### 1. Page Hero (minimal)
- **H1:** `Book Your Library Program`
- Short intro: "Submit your inquiry and Joe will respond within 24 hours with availability
  and confirmed dates. All 6 programs available for 2026 and 2027."
- No nav clutter — keep focus on the form

### 2. The Booking Form (main content)
Same fields as booking modal. See docs/forms/booking-modal.md for full field spec.

Form layout on this page:
- Left column (40%): form fields
- Right column (60%): summary panel (same live summary as modal)

Or: single-column full-width form with summary below (mobile-first approach)

### 3. What Happens After You Submit
Mini 3-step process below the form:
1. Joe reviews your request (within 24 hours)
2. You receive a confirmation or alternative date suggestion
3. Joe shows up — you pay by PO or check after the event

### 4. Contact Info
- "Rather call or email directly?"
- Phone: (405) 431-6625
- Email: joe.coover@gmail.com
- "We respond to all inquiries within 24 hours"

---

## Netlify Form Setup
- Form name: `library-booking`
- Required fields: library name, contact name, email, phone, city, state, at least one show request
- Hidden field: `form-name` = `library-booking`
- Success state: replace form with thank-you message
- Spam protection: Netlify honeypot field (built in)
- Notification: goes to joe.coover@gmail.com

---

## Notes
- The booking modal on every other page and this standalone page should share the same
  form field structure so Joe only gets one format of inquiry regardless of entry point
- If Joe later routes to HubSpot, replace the Netlify form action with HubSpot embed
