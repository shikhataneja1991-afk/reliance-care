# Reliance Care Solutions — Website Package
### Version 3.0 · March 2025

---

## 📁 Project Structure

```
reliance-care-final/
├── index.html          ← Home page
├── about.html          ← About Us page
├── services.html       ← All Services page
├── programs.html       ← Youth Programs page
├── contact.html        ← Contact Us page
└── README.md           ← This file
```

> **Zero external dependencies.** Every page is fully self-contained — all CSS and JavaScript is inlined directly inside each HTML file. Just drop all files in the same folder and it works on any host.

---

## 🎨 Brand Colors

| Role              | Hex       | Usage                                      |
|-------------------|-----------|--------------------------------------------|
| Dark Teal         | `#004542` | Backgrounds, header, footer, hero overlay  |
| Mid Teal          | `#00766A` | Accents, icons, labels, hover states       |
| Coral (Button 1)  | `#FF7866` | Primary CTAs, cursor, card borders         |
| Amber (Button 2)  | `#FFA801` | Secondary CTAs, badges, stats, stars       |
| Off-white         | `#f4faf9` | Page background                            |
| Dark footer       | `#002220` | Footer background                          |

---

## 🔤 Typography

| Role        | Font               | Weights Used           |
|-------------|--------------------|-----------------------|
| Body / UI   | **DM Sans**        | 300, 400, 500, 600, 700, 800 |
| Headings    | **DM Serif Display** | Regular, Italic      |

Both fonts load from Google Fonts CDN. An internet connection is required for fonts to render correctly. If offline, the browser will fall back to the system sans-serif font.

---

## 📄 Pages Overview

### `index.html` — Home
- Topbar with emergency phone number and address
- Full-bleed real photo hero with dark teal overlay
- Info panel cards (DODD cert, person-centered care, contact)
- About band (dark teal background)
- 6-service preview grid with coral/amber hover animations
- Youth programs section with image + card list
- 4-step process section
- 4-photo gallery strip
- 3-column testimonials
- Coral→Amber gradient CTA band
- Contact form strip
- Full footer with navigation links

### `about.html` — About Us
- Page hero with real photo background overlay
- Mission & story section with team image
- 6-value cards grid (Compassion, Integrity, Inclusion, Excellence, Reliability, Empowerment)
- "Why Choose Reliance" dark band with feature list
- Leadership team (3 cards with photos)
- CTA band

### `services.html` — Our Services
- Page hero
- All 9 services as individual cards:
  1. In-Home Direct Support
  2. Adult Day Services (A.M. & P.M.)
  3. Respite Services
  4. Community Group Activities
  5. Vocational Rehabilitation
  6. Horse & Animal Interactions
  7. On-Call Nurse Services
  8. Non-Medical Transportation
  9. Staff Training (CPI & PFS)
- FAQ accordion (5 questions)
- CTA band

### `programs.html` — Youth Programs
- Page hero (teal gradient)
- Intro section with image
- All 4 youth programs as expanded cards:
  1. CANS Certified Assessment for Children
  2. Group Home Services for Children *(New)*
  3. Emergency Respite Placement for Children *(New)*
  4. Horse & Animal Interactions for Youth
- Safety & Standards dark band
- 4-photo gallery strip
- CTA band

### `contact.html` — Contact Us
- Page hero
- Contact info column (phone, email, address, hours)
- Full contact form with service dropdown
- Quick-link cards (Services, Youth, About, Emergency Line)
- CTA band

---

## ⚙️ JavaScript Features (inline in every page)

| Feature | Description |
|---------|-------------|
| Custom Cursor | Coral dot + amber lagging ring, grows on hover |
| Sticky Header Shadow | Dynamic shadow on scroll |
| Hamburger Menu | Mobile nav toggle with animated X |
| Scroll Animations | IntersectionObserver fade-up with stagger delays |
| FAQ Accordion | Smooth open/close with chevron rotation |
| Form Feedback | Success state + auto-reset after 4.2s |
| Smooth Scroll | Offset-aware anchor scrolling (78px header clearance) |

---

## 📱 Responsive Breakpoints

| Breakpoint   | Layout Changes |
|-------------|---------------|
| ≤ 1024px    | 2-col steps, 2-col testimonials, 2-col footer, 2-col values |
| ≤ 768px     | Single column, hamburger nav, hero panel hidden, 2-col gallery |
| ≤ 480px     | Single-col steps, single-col footer, 2-col quick links |

---

## 🚀 Deployment Instructions

### Option A — Any Static Host (Netlify, Vercel, GitHub Pages)
1. Unzip the package
2. Upload all 5 HTML files + this README to your host
3. Set `index.html` as the default document
4. Done ✅

### Option B — Traditional Web Host (cPanel, FTP)
1. Unzip the package
2. FTP all files into your `public_html` or `www` root
3. Done ✅

### Option C — Local Preview
1. Unzip the package
2. Open `index.html` directly in any browser
3. All pages work without a server

---

## ✏️ How to Update Content

Since CSS and JS are inlined, all edits are made directly in each `.html` file.

**To change a phone number:**
Search all files for `(419) 704-0316` and replace with your new number.

**To change the address:**
Search for `3454 Oak Alley Ct` and replace across all files.

**To change a color:**
Each file's `<style>` block has CSS variables at the top:
```css
:root {
  --dark:  #004542;
  --mid:   #00766A;
  --coral: #FF7866;
  --amber: #FFA801;
}
```
Update these values and the change will apply throughout that page.

**To add a new service card**, copy any `.sc` div block inside `services.html` and update the icon, heading, and description.

---

## 🖼️ Images

All images currently load from **Unsplash CDN** and require an internet connection. To replace with your own photography:

| Location | Current Image | Recommended Size |
|----------|--------------|-----------------|
| Hero (index) | `photo-1576765607924` | 1800×1200px min |
| Youth section | `photo-1503454537195` | 800×600px |
| Gallery strip | 4 × Unsplash photos | 500×280px each |
| About page | `photo-1582213782179` | 700×500px |
| Team photos | 3 × Unsplash photos | 400×210px |

To replace, swap the `src` URL in each `<img>` tag with your own hosted image path.

---

## 📋 Change Log

| Version | Date       | Changes |
|---------|------------|---------|
| 3.0     | Mar 2025   | Brand colors updated: `#004542`, `#00766A`, `#FF7866`, `#FFA801` |
| 3.0     | Mar 2025   | Font changed to DM Sans + DM Serif Display |
| 3.0     | Mar 2025   | All CSS & JS fully inlined — zero external dependencies |
| 3.0     | Mar 2025   | Real hero photo with dark teal overlay (no gradient-only) |
| 3.0     | Mar 2025   | Topbar added with live phone + address |
| 2.0     | Mar 2025   | 5-page structure, Youth Programs expansion |
| 2.0     | Mar 2025   | All new services copy added (9 services total) |
| 1.0     | Mar 2025   | Initial redesign from reliancecaresolutions.com |

---

## 📞 Site Contact Info (as configured)

- **Phone:** (419) 704-0316
- **Email:** info@reliancecaresolutions.com
- **Address:** 3454 Oak Alley Ct., Suite 108, Toledo, OH 43606
- **Hours:** Mon–Fri 9am–5pm · Emergency: 24/7
- **Coverage:** All 88 Ohio Counties · DODD Certified

---

*Built for Reliance Care Solutions · Northwest Ohio*
