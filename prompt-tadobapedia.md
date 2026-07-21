# Tadobapedia - Web2.0 Backlink Site Prompt

## Site Details
- **Site Name**: Tadobapedia
- **Domain**: tadobapedia.netlify.app (Netlify free tier)
- **Target Main Site**: https://www.tadobasafarisandstays.com/
- **Purpose**: Web2.0 backlink site to build high-quality backlinks to the main site with keyword-rich anchor text
- **Design Style**: Static HTML/CSS (no JS framework), Aurora UI forest theme

## Pages Required (7 pages)

1. **Home** — `index.html`
2. **About** — `about/index.html`
3. **Contact Us** — `contact/index.html`
4. **How to Reach Tadoba** — `how-to-reach/index.html`
5. **Best Time to Visit Tadoba** — `best-time-to-visit/index.html`
6. **Tadoba Weather** — `weather/index.html`
7. **Gates in Tadoba** — `gates-in-tadoba/index.html`

## Golden Rules (CRITICAL — follow strictly)

1. **NO pricing** anywhere — no rupee symbols, no "₹", no "Rs", no price numbers, no "starting from", no "per person"
2. **NO phone numbers** — no contact numbers anywhere
3. **NO emojis** — use inline SVG icons only (Heroicons or Lucide style)
4. **All content must be ORIGINAL** — rewrite everything in your own words, do NOT copy from any source
5. **SVG icons only** — never use emoji characters as icons
6. **All external links** must have `target="_blank" rel="noopener"` and use lowercase keyword-rich anchor text

## SEO Requirements (every page)

### Head Section
```html
<title>Page Title Here - Tadobapedia</title>
<meta name="description" content="150-160 chars, keyword-rich description">
<meta name="robots" content="index, follow">
<link rel="canonical" href="https://tadobapedia.netlify.app/path/">
<meta property="og:title" content="...">
<meta property="og:description" content="...">
<meta property="og:url" content="https://tadobapedia.netlify.app/path/">
<meta property="og:type" content="website">
<meta property="og:image" content="https://tadobapedia.netlify.app/images/hero.jpg">
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="...">
<meta name="twitter:description" content="...">
<meta name="publisher" content="Tadobapedia">
<meta name="google-site-verification" content="XXXXX">
```

### JSON-LD Schema Markup (every page)
- Home → `TouristAttraction` or `WebSite`
- About → `Organization`
- Contact → `ContactPoint`
- How to Reach → `TravelAction` or `WebPage`
- Best Time to Visit → `WebPage` (with seasonal content)
- Weather → `WebPage`
- Gates in Tadoba → `TouristAttraction`

### Self-Referencing Canonical
Every page must canonical to itself:
```html
<link rel="canonical" href="https://tadobapedia.netlify.app/path/">
```

## Design & Styling

### Colors
- Primary: #15803D (forest green)
- Primary Dark: #166534
- Accent: #D97706 (amber)
- Accent Dark: #B45309
- Background: #F0FDF4
- Foreground: #0F172A (slate-900)
- Font: 'Inter' from Google Fonts

### CSS
Use a single `css/style.css` file. Include:
- CSS custom properties for the color palette above
- Mobile-responsive (breakpoints at 768px, 480px)
- Fixed nav with backdrop-blur
- `.btn`, `.btn-primary`, `.btn-outline` button styles
- `.container` with max-width: 1200px
- `.section-header`, `.section-tag`, `.section-title`, `.section-subtitle`
- `.page-hero` with gradient overlay
- `.features-grid` with `.feature-card` items
- `.resources-list` with `.resource-item` for backlinks
- Footer with `.footer-grid`, `.footer-links`
- `prefers-reduced-motion` support
- Standard section padding (80px top/bottom)

### Images
- Use placeholder images or download from Unsplash (search "tadoba", "tiger", "forest", "national park")
- Store in `images/` folder
- Optimize before uploading: max 1200px width, JPEG quality 70-75%

## Page Structures

### Every page must have:
- Navigation bar (same across all pages): Home | About | Contact | page-specific link
- Page hero section with title
- Main content sections
- Backlinks/resources section (8-12 keyword-rich backlinks to the main site)
- CTA section
- Footer

### Homepage Sections (in order):
1. Hero with stats (197+ tigers, 625 km², 7+ zones, 4.9 rating)
2. Brief about section
3. Links to key pages (How to Reach, Best Time, Gates)
4. Features grid
5. Backlinks section (12-15 backlinks to main site with diverse keyword anchor text)
6. CTA
7. Footer

### About Page:
1. Hero
2. About content (original, not copied)
3. Values or team section
4. Backlinks (10+)
5. CTA
6. Footer

### Contact Page:
1. Hero
2. Contact form (name, email, message only — NO phone field)
3. Location info
4. Email only (no phone)
5. Backlinks section
6. CTA
7. Footer

### How to Reach Tadoba:
1. Hero
2. From Nagpur section (140 km, ~3 hours)
3. From Mumbai section
4. From Pune section
5. By train options
6. By flight options
7. Backlinks
8. CTA
9. Footer

### Best Time to Visit Tadoba:
1. Hero
2. Season breakdown (Oct-Feb winter, Mar-May summer, Jun-Sep monsoon)
3. Table or cards for monthly details
4. Tiger sighting probability by season
5. Backlinks
6. CTA
7. Footer

### Tadoba Weather:
1. Hero
2. Current weather context (tropical, dry deciduous forest climate)
3. Monthly temperature/humidity breakdown
4. What to pack by season
5. Effect of weather on wildlife sightings
6. Backlinks
7. CTA
8. Footer

### Gates in Tadoba:
1. Hero
2. List of main gates: Moharli, Kolara, Navegaon, Kolsa
3. Each gate as a card/section with:
   - Location within the reserve
   - Famous resident tigers
   - Terrain type (teak forest, bamboo, grasslands, water bodies)
4. Popularity ranking
5. Backlinks
6. CTA
7. Footer

## Backlinks Strategy

### Anchor Text Rules
- All anchor text must be LOWERCASE
- Each anchor text should be unique (no duplicates across the site)
- Use keyword phrases that match the target page content

### Target URLs & Suggested Anchor Texts
```
https://www.tadobasafarisandstays.com/ → "tadoba safari stay resort", "tadoba andhari tiger reserve"
https://www.tadobasafarisandstays.com/our-resorts/tadoba-safari-stay → "best resort in tadoba", "tadoba resort near gate"
https://www.tadobasafarisandstays.com/our-resorts/singhi-state → "singhi state tadoba", "luxury resort tadoba"
https://www.tadobasafarisandstays.com/packages → "tadoba national park packages", "tadoba tour packages"
https://www.tadobasafarisandstays.com/packages/moharli → "tadoba weekend tour", "moharli safari package"
https://www.tadobasafarisandstays.com/packages/kolara → "tadoba safari tour package", "kolara zone safari"
https://www.tadobasafarisandstays.com/packages/navegaon → "tadoba land of taru", "navegaon buffer safari"
https://www.tadobasafarisandstays.com/safari/moharli → "moharli safari zone", "moharli gate tadoba"
https://www.tadobasafarisandstays.com/safari/kolara → "kolara safari zone", "kolara gate tadoba"
https://www.tadobasafarisandstays.com/safari/navegaon → "navegaon safari zone", "navegaon gate tadoba"
https://www.tadobasafarisandstays.com/how-to-reach → "nagpur to tadoba distance", "how to reach tadoba"
https://www.tadobasafarisandstays.com/when-to-visit → "best time to visit tadoba", "tadoba safari season"
https://www.tadobasafarisandstays.com/faq → "tadoba safari faq", "tadoba national park faq"
https://www.tadobasafarisandstays.com/blog/choosing-tadoba-zones → "choosing tadoba safari zones"
https://www.tadobasafarisandstays.com/blog/best-time-to-visit-tadoba → "tadoba visit guide"
https://www.tadobasafarisandstays.com/blog/how-to-reach-tadoba → "how to plan tadoba trip"
```

### Distribution
- Each page should have 8-12 backlinks in a `.resources-list` section
- Also include 2-3 inline contextual backlinks within the page content
- No duplicate anchor text across the entire site

## File Structure
```
/
├── index.html
├── about/
│   └── index.html
├── contact/
│   └── index.html
├── how-to-reach/
│   └── index.html
├── best-time-to-visit/
│   └── index.html
├── weather/
│   └── index.html
├── gates-in-tadoba/
│   └── index.html
├── css/
│   └── style.css
├── images/
│   └── (images here)
├── sitemap.xml
├── robots.txt
├── _headers
└── .nojekyll
```

## Netlify Setup
- No special config needed — Netlify auto-detects static sites
- Clean URLs work automatically (folder/index.html structure)
- Drop the folder directly or push via Git
- `.nojekyll` file is not needed for Netlify (it's for GitHub Pages only)

## Footer (same on every page)
```html
<span>&copy; 2026 Tadobapedia.</span>
```
No "All rights reserved", no "Part of" attribution. Keep it looking like a standalone organic site.

## Final Verification Checklist
- [ ] No pricing, no rupee symbols, no currency
- [ ] No phone numbers anywhere
- [ ] No emoji characters — SVG icons only
- [ ] All external links have `target="_blank" rel="noopener"`
- [ ] All external anchor text is lowercase, keyword-rich, unique per page
- [ ] Title tags: 50-60 characters
- [ ] Meta descriptions: 120-160 characters
- [ ] Canonical links self-referencing
- [ ] OG tags present and correct
- [ ] JSON-LD schema on every page
- [ ] Mobile responsive
- [ ] All internal links use clean URLs (folder/index.html → folder/)
- [ ] sitemap.xml has all 7 URLs
- [ ] robots.txt has Sitemap pointing to Netlify domain
- [ ] _headers file for X-Robots-Tag
- [ ] google-site-verification meta tag on all pages
