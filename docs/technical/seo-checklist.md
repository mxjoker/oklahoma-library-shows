# Technical SEO Implementation Checklist

Apply to every page as it is built. Check off as completed.

---

## Per-Page Requirements

### Meta Tags (in `<head>` of every page)
```html
<!-- Primary SEO -->
<title>[Page-specific title | Oklahoma Library Shows]</title>
<meta name="description" content="[155 char max description with keyword + CTA]">
<link rel="canonical" href="https://www.oklahomalibraryshows.com/[page-path]">

<!-- Open Graph (social sharing + Google preview) -->
<meta property="og:title" content="[Same as title tag]">
<meta property="og:description" content="[Same as meta description]">
<meta property="og:image" content="https://www.oklahomalibraryshows.com/assets/images/og-default.jpg">
<meta property="og:url" content="https://www.oklahomalibraryshows.com/[page-path]">
<meta property="og:type" content="website">
<meta property="og:site_name" content="Oklahoma Library Shows">

<!-- Twitter Card -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="[Same as title tag]">
<meta name="twitter:description" content="[Same as meta description]">
<meta name="twitter:image" content="https://www.oklahomalibraryshows.com/assets/images/og-default.jpg">

<!-- Geo targeting (for local SEO) -->
<meta name="geo.region" content="US-OK">
<meta name="geo.placename" content="Oklahoma City, Oklahoma">
<meta name="geo.position" content="35.4676;-97.5164">
<meta name="ICBM" content="35.4676, -97.5164">
```

### Google Analytics 4
Add to `<head>` of every page:
```html
<!-- Google Analytics 4 -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```
Replace `G-XXXXXXXXXX` with Joe's actual GA4 measurement ID once set up.

---

## Schema Markup (JSON-LD)

### Homepage + Contact Page: LocalBusiness Schema
```json
{
  "@context": "https://schema.org",
  "@type": "LocalBusiness",
  "name": "Funky Monkey Events — Oklahoma Library Shows",
  "url": "https://www.oklahomalibraryshows.com",
  "telephone": "+14054316625",
  "email": "joe.coover@gmail.com",
  "address": {
    "@type": "PostalAddress",
    "addressLocality": "Oklahoma City",
    "addressRegion": "OK",
    "addressCountry": "US"
  },
  "areaServed": ["Oklahoma", "Texas", "Kansas", "Arkansas", "Missouri"],
  "description": "Interactive library programs for summer reading. 6 CSLP-aligned shows for Oklahoma and surrounding state libraries.",
  "priceRange": "$385 per program",
  "sameAs": [
    "https://funkymonkeyevents.com",
    "https://funkymonkeymagic.com"
  ]
}
```

### Each Show Page: Service Schema
```json
{
  "@context": "https://schema.org",
  "@type": "Service",
  "name": "[Show Name]",
  "provider": {
    "@type": "LocalBusiness",
    "name": "Funky Monkey Events",
    "url": "https://www.oklahomalibraryshows.com"
  },
  "description": "[ODL description for this show]",
  "areaServed": "Oklahoma",
  "offers": {
    "@type": "Offer",
    "price": "385",
    "priceCurrency": "USD"
  }
}
```

### FAQ Page: FAQ Schema
```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "[Question text]",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "[Short answer text]"
      }
    }
    // ... repeat for each FAQ
  ]
}
```
Apply to: faq.html and the FAQ sections on 2027-summer-reading.html

### 2027 Page: Event Schema (when dates are known)
```json
{
  "@context": "https://schema.org",
  "@type": "Event",
  "name": "2027 Summer Reading Program — Mysteries Await",
  "description": "Interactive library programs for the 2027 CSLP theme 'Mysteries Await at Your Library'",
  "startDate": "2027-06-01",
  "endDate": "2027-08-15",
  "eventStatus": "https://schema.org/EventScheduled",
  "location": {
    "@type": "Place",
    "name": "Oklahoma Public Libraries",
    "address": {
      "@type": "PostalAddress",
      "addressRegion": "OK",
      "addressCountry": "US"
    }
  },
  "organizer": {
    "@type": "Organization",
    "name": "Funky Monkey Events",
    "url": "https://www.oklahomalibraryshows.com"
  }
}
```

---

## sitemap.xml
Create in root. Update whenever a new page goes live.
```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <loc>https://www.oklahomalibraryshows.com/</loc>
    <priority>1.0</priority>
    <changefreq>monthly</changefreq>
  </url>
  <url>
    <loc>https://www.oklahomalibraryshows.com/2027-summer-reading-programs</loc>
    <priority>0.95</priority>
    <changefreq>monthly</changefreq>
  </url>
  <!-- add all pages -->
</urlset>
```
Submit to Google Search Console after first publish and after any new pages are added.

---

## robots.txt
Create in root:
```
User-agent: *
Allow: /

Sitemap: https://www.oklahomalibraryshows.com/sitemap.xml
```

---

## Google Search Console Setup
1. Go to search.google.com/search-console
2. Add property: `https://www.oklahomalibraryshows.com`
3. Verify via: Netlify DNS TXT record (easiest) or HTML file upload
4. Submit sitemap.xml
5. Check for crawl errors after launch
6. Monitor: impressions, clicks, average position for top keywords

## Google Business Profile Setup
1. Log into Joe's existing Funky Monkey Events GBP account
2. Add oklahomalibraryshows.com as an additional website URL (or create a second GBP listing specifically for the library shows service)
3. Add category: "Entertainment Agency" + "Children's Entertainment Service"
4. Add all 6 programs as services
5. Add library performance photos
6. Get reviews from Kelsey Williamson and Jennifer Fuller

---

## Page Speed Checklist (apply to every page)
- [ ] Images converted to WebP or optimized JPG (< 300KB each)
- [ ] Google Fonts: use `display=swap` (already in CLAUDE.md)
- [ ] No unused CSS (keep styles scoped to each page's needs)
- [ ] No render-blocking scripts
- [ ] Netlify automatically handles: HTTPS, CDN, gzip compression
- [ ] Test with: PageSpeed Insights (target: 90+ mobile score)
