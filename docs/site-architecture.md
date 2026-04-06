# Site Architecture — Oklahoma Library Shows

## URL Structure
Base: `https://www.oklahomalibraryshows.com`

```
/                                        → index.html
/about                                   → about.html
/booking                                 → booking.html
/contact                                 → contact.html
/faq                                     → faq.html
/service-area                            → service-area.html
/2027-summer-reading-programs            → 2027-summer-reading.html

/shows/magic-show                        → shows/magic-show.html
/shows/bubble-show                       → shows/bubble-show.html
/shows/magic-workshop                    → shows/magic-workshop.html
/shows/balloon-workshop                  → shows/balloon-workshop.html
/shows/story-doodles                     → shows/story-doodles.html
/shows/foam-party                        → shows/foam-party.html

/locations/oklahoma-city                 → locations/oklahoma-city.html
/locations/tulsa                         → locations/tulsa.html
/locations/eastern-oklahoma              → locations/eastern-oklahoma.html
/locations/rural-oklahoma                → locations/rural-oklahoma.html
/locations/texas                         → locations/texas.html
/locations/dallas                        → locations/dallas.html
/locations/wichita-falls                 → locations/wichita-falls.html
/locations/kansas                        → locations/kansas.html
/locations/arkansas                      → locations/arkansas.html
/locations/missouri                      → locations/missouri.html

/resources                               → resources/index.html
/resources/summer-reading-planning-guide → resources/summer-reading-planning-guide.html
/resources/how-to-book-a-performer       → resources/how-to-book-a-performer.html

/sitemap.xml                             → sitemap.xml
/robots.txt                              → robots.txt
```

---

## Page Inventory (29 pages + 2 files)

### Core Pages (5)
| File | Purpose | SEO Priority |
|------|---------|--------------|
| index.html | Homepage — brand, social proof, all shows | High |
| about.html | Joe's story, credentials, why libraries trust him | Medium |
| booking.html | Dedicated booking page with full form | High |
| contact.html | Contact info + quick form | Medium |
| service-area.html | Map/list of coverage + travel fee structure | High |

### Campaign Pages (1)
| File | Purpose | SEO Priority |
|------|---------|--------------|
| 2027-summer-reading.html | Ranks for 2027 + "Mysteries Await" searches NOW | **Highest** |
| faq.html | Featured snippet + voice search capture | High |

### Show Pages (6)
| File | 2026 Name | SEO Focus |
|------|-----------|-----------|
| shows/magic-show.html | Dinosaur Adventure Magic Show | "magic show library oklahoma" |
| shows/bubble-show.html | Professor Buckets Bubble Show | "bubble show library program" |
| shows/magic-workshop.html | Hands-on Magic Workshop | "magic workshop library kids" |
| shows/balloon-workshop.html | Balloon Twisting Workshop | "balloon workshop library oklahoma" |
| shows/story-doodles.html | Story Doodles Draw-Along | "story doodles library program" |
| shows/foam-party.html | Foam Party Celebration | "foam party library event oklahoma" |

### Location Pages (10)
| File | Focus | Key Angle |
|------|-------|-----------|
| locations/oklahoma-city.html | OKC metro | Metropolitan + Pioneer library systems, no travel fee |
| locations/tulsa.html | Tulsa metro | Tulsa City-County Library, bulk booking week, no travel fee |
| locations/eastern-oklahoma.html | Eastern OK | EOLS cluster, bulk week, route efficiency |
| locations/rural-oklahoma.html | Rural OK statewide | Mileage savings from clustering, underserved angle |
| locations/texas.html | Texas overview | State-level, links to city sub-pages |
| locations/dallas.html | Dallas metro | Specific DFW library targeting |
| locations/wichita-falls.html | Wichita Falls | Smaller city, easier to rank for |
| locations/kansas.html | Kansas | State overview |
| locations/arkansas.html | Arkansas | State overview |
| locations/missouri.html | Missouri | State overview |

### Resources (3)
| File | Content | Gate |
|------|---------|------|
| resources/index.html | Resources hub + download menu | None |
| resources/summer-reading-planning-guide.html | Full planning guide for librarians | Email signup |
| resources/how-to-book-a-performer.html | Budget justification guide | Free, no gate |

---

## Navigation Map

### Primary Nav (desktop — all pages)
```
Oklahoma Library Shows [logo]
Shows ▾ | Locations ▾ | About | Resources | [Check Availability button]
```

### Shows dropdown
```
Magic Show
Bubble Show
Magic Workshop
Balloon Workshop
Story Doodles
Foam Party
```

### Locations dropdown
```
Oklahoma City  |  Tulsa  |  Eastern Oklahoma  |  Rural Oklahoma
Texas  |  Kansas  |  Arkansas  |  Missouri
```

### Mobile nav (≤768px)
```
[Hamburger menu] + [Check Availability button always visible]
```

---

## Internal Linking Strategy

### From Homepage →
- All 6 show pages (cards in shows section)
- OKC, Tulsa, Eastern OK, Rural OK (in service area section)
- 2027 summer reading page (in hero or dedicated banner)
- Resources (in footer or dedicated section)
- Booking (persistent nav CTA + hero CTA)

### From Each Show Page →
- Booking modal (hero CTA + bottom CTA band)
- 2027-summer-reading.html (inline contextual link in educational connections section)
- 2 other related show pages (in "You might also like" section at bottom)
- service-area.html (in show details grid near price)

### From Each Location Page →
- All 6 show pages
- Booking.html
- service-area.html
- Other nearby location pages (e.g. OKC links to Tulsa and Rural OK)

### From 2027 Page →
- All 6 show pages (with "2027 adaptation" teaser per show)
- booking.html
- resources/index.html

### From Resources →
- All show pages (contextual)
- 2027-summer-reading.html
- booking.html
- Newsletter signup form

---

## Sitemap Priority Values
```xml
/ → priority 1.0
/2027-summer-reading-programs → priority 0.95
/shows/* → priority 0.9
/locations/* → priority 0.8
/booking → priority 0.85
/resources/* → priority 0.7
/about, /contact, /service-area, /faq → priority 0.6
```
