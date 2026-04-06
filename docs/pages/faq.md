# Page Spec: FAQ

**File:** `faq.html`
**URL:** `/faq`
**Build Priority:** Phase 2

---

## SEO Targets
- **Primary keyword:** `library summer reading program FAQ oklahoma`
- **Secondary:** `how to book a library performer`, `how much does a library show cost`
- **Title tag:** `FAQ — Library Summer Reading Programs | Oklahoma Library Shows`
- **Meta description:** `Answers to every question librarians ask before booking. Pricing, travel, age ranges, setup, payment, and more. Joe Coover — (405) 431-6625.`

---

## Page Purpose
Captures voice search and featured snippet traffic. Librarians often search phrased as
questions. Answers should be short enough for a snippet (40–60 words) but with a longer
explanation below for context. Add FAQ schema markup to this page.

---

## FAQ Questions (in grouped sections)

### Pricing & Payment
1. **How much do library shows cost?**
   Short: "$385 per program. All six shows are the same price."
   Long: We believe in transparent pricing — no hidden fees or tiered costs. The $385 rate covers a 45–60 minute program for any audience size within range. Travel fees may apply outside the OKC/Tulsa metro area. We accept purchase orders and checks; libraries do not need to pay upfront.

2. **Do you accept purchase orders?**
   Short: "Yes — we accept purchase orders and checks. No credit card required."
   Long: We work with libraries exclusively, and we understand how public institution payments work. Submit your inquiry, get confirmation, then send a PO at your convenience. Payment is typically due after the event.

3. **Is there a travel fee?**
   Short: "No travel fee within the OKC and Tulsa metro areas. Fees vary by distance for other locations."
   Long: Oklahoma City and Tulsa metro libraries can book with no travel surcharge. For libraries in rural Oklahoma or out of state (TX, KS, AR, MO), we calculate travel fees based on distance and may bundle shows on the same route to reduce your per-show cost. See our Service Area page.

4. **Can we book multiple shows at a discount?**
   Short: "We don't offer a percentage discount, but booking multiple shows in one week reduces travel cost across your library system."
   Long: Many library systems in Tulsa and Eastern Oklahoma book 5–10 shows in a single week. By routing multiple branches efficiently, each library's effective cost (including travel) goes down. Mention your system size and we'll build an efficient schedule.

### Booking Process
5. **How far in advance should I book?**
   Short: "As early as possible — spring slots typically fill by February or March."
   Long: Summer 2027 slots are available now. Librarians who book in fall or winter get first pick of dates and times. Peak weeks (late June, early July) book fastest. For Tulsa and Eastern OK library systems that book an entire week, locking in early is especially important.

6. **How does the booking process work?**
   Short: "Submit an inquiry with your preferred shows and dates. Joe responds within 24 hours to confirm or suggest alternatives."
   Long: This site uses an inquiry system — not live booking. Use the Check Availability form to tell us what you want (show, date, morning or afternoon). Joe reviews every request personally and responds within 24 hours with confirmation or alternative date suggestions. There's no back-and-forth calendar chaos.

7. **Can I request multiple shows on the same day or week?**
   Short: "Yes — use the Show Request Builder in the form to add multiple shows in one submission."
   Long: The booking form has a Show Request Builder where you can add as many show requests as you need — different shows, different dates, different time preferences — all in one submission. Ideal for library systems booking multiple branches.

8. **What if my preferred date isn't available?**
   Short: "Joe will suggest nearby alternative dates in his response."
   Long: Joe reviews every inquiry personally and always proposes alternatives if your first-choice date is taken. Most librarians find a workable solution in the first or second exchange. The 24-hour response promise applies to every inquiry.

### The Shows
9. **What age ranges do the shows work for?**
   Short: "Most shows work for ages 4–12. Some programs are all-ages. See each show page for specifics."
   Long breakdown:
   - Magic Show: All ages, families welcome
   - Bubble Show: Ages 4–10 best, but all ages enjoy it
   - Magic Workshop: Ages 7–12 (requires some dexterity)
   - Balloon Workshop: Ages 6+ (younger kids may need help)
   - Story Doodles: Ages 4–10
   - Foam Party: All ages, outdoor only

10. **How much space is needed?**
    Short: "Most shows need a clear performance area of about 10×10 feet plus audience space."
    Long: Indoor shows can work in any standard meeting room or children's section with furniture moved. The Foam Party is the only outdoor-only show and requires outdoor space with a water source nearby. Joe handles all setup and teardown — typically 20–30 minutes.

11. **Is the Foam Party really outdoor only?**
    Short: "Yes — the Foam Party is outdoor only and weather-dependent. It has a separate booking calendar."
    Long: The Foam Party uses foam machines that require outdoor space, a flat surface, and nearby water access. Because of weather dependency, foam party dates are managed separately from the other five shows. When you select Foam Party in the booking form, you'll see a note about the special scheduling process.

12. **Can shows be adapted for the 2027 CSLP theme "Mysteries Await"?**
    Short: "Yes — Joe adapts all shows for the current CSLP theme each year."
    Long: For 2027, every show will incorporate mystery, detective, and suspense elements. The Magic Show becomes a whodunit adventure. The Story Doodles unfolds as a live mystery. Even the Balloon Workshop ties in with detective props. See the 2027 Summer Reading page for full details.

### Logistics
13. **Do you travel outside Oklahoma?**
    Short: "Yes — we serve Texas, Kansas, Arkansas, and Missouri with travel fees."
    Long: Joe regularly performs in Texas (Dallas, Wichita Falls), Kansas, Arkansas, and Missouri. Out-of-state travel fees apply. Bundling multiple shows in one trip is the best way to minimize travel cost. See the Service Area page.

14. **What do I need to provide?**
    Short: "Just the performance space and an audience. Joe brings everything else."
    Long: Joe arrives 20–30 minutes before showtime with all equipment, props, and setup materials. You don't need to provide a microphone, screen, or any supplies (except for the Foam Party, which needs outdoor space and water access). All you need is a room full of excited kids.

15. **Are the shows safe for children with sensory sensitivities?**
    Short: "Joe is experienced working with diverse library audiences. Let us know in advance and we'll accommodate."
    Long: Library audiences are often mixed, and Joe is accustomed to adjusting energy levels, volume, and audience participation to fit the room. If you have known sensory concerns in your audience, note them in the booking form's comments field and Joe will come prepared.

---

## Page Layout
- Group questions under accordion sections by category
- Each answer has a short version (1–2 sentences) visible by default
- "Show more" expands to the long version (optional — can implement as accordion or just show all)
- Sticky "Still have questions? Call (405) 431-6625" bar at bottom

## Schema
Add FAQ schema (application/ld+json) for all 15 questions.
Use the short answer as the `acceptedAnswer` text in schema.
