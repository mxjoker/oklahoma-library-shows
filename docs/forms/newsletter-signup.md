# Form Spec: Newsletter / Summer Planning List Signup

Used on: resources/index.html (primary), resources/summer-reading-planning-guide.html (gate),
optionally in footer or as exit-intent on any page.

---

## Purpose
Build Joe's summer library email list so that returning and new librarians can be reached
directly each spring with:
- 2027 booking open announcements
- New show updates
- Early-access availability

---

## Form Fields

### Minimal Version (footer / sidebar use)
| Field | Type | Required |
|-------|------|----------|
| Name | text | ✅ |
| Email | email | ✅ |
| Library Name | text | ✅ |
| [Subscribe] button | — | — |

### Full Version (resource gate on planning guide page)
| Field | Type | Required |
|-------|------|----------|
| First Name | text | ✅ |
| Email | email | ✅ |
| Library Name | text | ✅ |
| State | select | ❌ | OK, TX, KS, AR, MO, Other |
| [Get the Free Guide] button | — | — |

---

## Value Proposition
Headline: `Get the Free Summer Reading Program Planning Guide`
Subhead: `Plus early access to booking dates before they open to the public.`
Small print: `No spam. Just one or two emails each season. Unsubscribe anytime.`

---

## Behavior

### On Submit
1. Netlify Form captures the submission
2. Success message shown:
   > "You're on the list! Check your email — the planning guide is on its way."
3. Joe manually (or via Mailchimp) sends the PDF planning guide to new subscribers
4. Joe's follow-up sequence (manual for now):
   - Welcome email with PDF link
   - September: "2027 booking is now open — here are your early access dates"
   - February: "Spring reminder — summer slots are filling up"

### Gate Behavior (planning guide page only)
- Page shows first 2 sections of the guide preview
- Rest of content is blurred with form overlay
- On submit: form hides, full content unlocks on page
- PDF download link appears

---

## Netlify Form Implementation
```html
<form name="newsletter-signup" method="POST" data-netlify="true" netlify-honeypot="bot-field">
  <input type="hidden" name="form-name" value="newsletter-signup" />
  <input type="hidden" name="bot-field" />
  <!-- fields here -->
</form>
```
Notification: joe.coover@gmail.com
Subject line: "New Newsletter Signup — [Library Name]"

---

## Future: Mailchimp or HubSpot Integration
When ready to automate:
1. Replace Netlify form with Mailchimp embedded form OR HubSpot form
2. Set up automated welcome sequence (2–3 emails)
3. Create a "Summer Library" list segment separate from general FME contacts
4. Map library name and state fields to custom properties for segmentation
