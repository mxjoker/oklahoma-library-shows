# Form Spec: Booking Modal + Booking Page Form

Used on: booking modal (all pages) + booking.html (standalone page)

---

## Form Fields

### Librarian Information (Section 1)
| Field | Type | Required | Placeholder |
|-------|------|----------|-------------|
| Library Name | text | ✅ | "Oklahoma City Public Library" |
| Your Name | text | ✅ | "Jane Smith" |
| Your Title | text | ❌ | "Youth Services Librarian" |
| Email | email | ✅ | "jane@yourlibrary.org" |
| Phone | tel | ✅ | "(405) 555-0000" |
| City | text | ✅ | "Oklahoma City" |
| State | select | ✅ | OK (default), TX, KS, AR, MO, Other |

### Show Request Builder (Section 2)
Librarian adds one show at a time. Each "request" has:
| Field | Type | Required | Options |
|-------|------|----------|---------|
| Show | select | ✅ | Magic Show, Bubble Show, Magic Workshop, Balloon Workshop, Story Doodles, Foam Party |
| Preferred Date | date | ✅ | Date picker (must be in future) |
| Time Preference | radio | ✅ | Morning (9am–12pm), Afternoon (1pm–5pm), Flexible |
| [+ Add Another Show] | button | — | Adds another show row |

**Foam Party Alert:**
When "Foam Party" is selected:
→ Show orange alert box:
"⚠️ The Foam Party is outdoor only and weather-dependent. Dates are managed on a separate outdoor calendar. Include your top 2–3 preferred dates in the Notes field and we'll match you to available outdoor slots."

### Live Summary Panel (Section 3 — updates in real time)
Shows as librarian fills in:
```
📋 Your Booking Summary
Library: [Library Name]
Contact: [Name] — [Email]

Requested Shows:
• [Show Name] — [Date] — [Time Pref]
• [Show Name] — [Date] — [Time Pref]

Total: [X] show(s) at $385 each = $[Total] estimated
```
Note: "Estimated total shown for reference. Final confirmation provided by Joe."

### Additional Notes (Section 4)
| Field | Type | Required | Placeholder |
|-------|------|----------|-------------|
| Notes / Special Requests | textarea | ❌ | "Notes about your space, audience size, accessibility needs, or scheduling constraints..." |

### Submission
- CTA: "Send My Booking Request"
- Below button: "We respond within 24 hours. No contracts upfront. Libraries pay by PO or check after the event."
- Small print: "By submitting this form you agree to receive a follow-up email from Funky Monkey Events."

---

## Behavior

### Pre-selection
When modal is opened from a specific show's "Book this show" button:
- Show dropdown pre-selects that show automatically
- Focus goes to the date field

### Multiple Requests
- "Add Another Show" button appends a new show row
- Max requests: no hard limit — but show a warning if more than 10 are added
- "Remove" (×) button on each row after the first

### Validation
- Email: must be valid format
- Date: must be today + 7 days minimum (no same-week bookings — Joe needs lead time)
- Phone: basic format check
- At least one complete show request before submit is allowed

### Success State (after submit)
Replace form content with:
```
✅ Request Received!

Thanks, [Name]! Joe will review your request and respond within 24 hours.

In the meantime:
• Questions? Call (405) 431-6625
• Email: joe.coover@gmail.com
• Explore more programs: [Shows] [2027 Planning]
```

### Error State
If Netlify form fails:
```
Something went wrong. Please email joe.coover@gmail.com directly
or call (405) 431-6625.
```

---

## Netlify Form Implementation
```html
<form name="library-booking" method="POST" data-netlify="true" netlify-honeypot="bot-field">
  <input type="hidden" name="form-name" value="library-booking" />
  <input type="hidden" name="bot-field" /> <!-- honeypot -->
  <!-- fields here -->
</form>
```
Notification goes to: joe.coover@gmail.com
Subject line: "New Library Booking Request — [Library Name]"

---

## Future: HubSpot Migration
When Joe is ready to move to HubSpot:
1. Replace `<form>` with HubSpot embed code
2. Map fields to HubSpot contact properties
3. Set up HubSpot workflow: new submission → automated acknowledgment email → Joe task
4. Keep form field names and structure identical so no retraining needed
