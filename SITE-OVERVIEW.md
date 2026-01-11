# Digital Wellness Design - Site Overview

## 🎉 Complete Static Website Delivered

Your calm, premium, nature-inspired static website is fully built and ready for deployment to GitHub Pages.

---

## 📄 Pages (11 Total)

### Core Pages
1. **/** (index.html) - Home page with hero, value props, service cards, lead magnet
2. **/about.html** - About Meg with background and comprehensive FAQ
3. **/services.html** - Services overview with all offerings
4. **/contact.html** - Contact page with email info

### Service Detail Pages
5. **/iphone-ritual-reset.html** - $150 | 60-minute session
6. **/iphone-sanctuary-session.html** - Email to apply | Full redesign
7. **/iphone-seasonal-syncs.html** - Coming fall 2025 | Year-long coaching

### Product Page
8. **/sunset-sunrise-sync.html** - $3 | Digital product (iPhone shortcuts)

### NEW Practitioners Page
9. **/practitioners.html** - For wellness practitioners seeking websites/listings

### Legal Pages
10. **/privacy.html** - Privacy policy
11. **/terms.html** - Terms of service

---

## 🎨 Design System

### Colors (Nature-Inspired Palette)
- **Cream** `#FAF8F5` - Primary background
- **Sand** `#E8E3DA` - Borders, subtle backgrounds
- **Sage** `#8B9D83` - Primary brand accent
- **Forest** `#5A6B52` - CTA buttons, links
- **Terracotta** `#C17A5F` - Secondary accent
- **Sunlight** `#F5E6D3` - Warm background sections
- **Sunrise** `#FFD4A3` - Gradient accents
- **Stone** `#6B6557` - Body text
- **Charcoal** `#3A3832` - Headings

### Typography
- **Headings**: Loubag (self-hosted, 600 weight)
- **Body**: Inter (Google Fonts)
- **Spacing**: 8px base unit system
- **Line Heights**: 1.2 (headings), 1.6 (body), 1.8 (relaxed)

### Key CSS Classes
- `.btn-primary` - Forest green CTA buttons
- `.btn-outline` - Outlined buttons for secondary actions
- `.btn-secondary` - Sand-colored buttons
- `.card` - White cards with subtle borders
- `.hero` - Hero sections with gradient background
- `.content-section` - Centered content (max-width: 768px)
- `.bullet-list` - Checkmark bullet lists
- `.feature-block` - Highlighted feature boxes
- `.faq-item` - FAQ styling with sage accents

---

## 📁 Assets

### Fonts
- `/fonts/loubag-semi-bold.ttf` - Primary heading font
- `/fonts/gistesy.ttf` - Available but not currently used

### Illustrations
- `/assets/illustrations/ritual.svg` (3.6MB) - iPhone Ritual Reset
- `/assets/illustrations/sanctuary.svg` (393KB) - iPhone Sanctuary Session
- `/assets/illustrations/seasonal.svg` (1.2MB) - iPhone Seasonal Syncs

### Empty Directories (Ready for Content)
- `/assets/images/` - Add photos, hero images
- `/assets/videos/` - Add hero video with poster

---

## 🔗 Placeholder URLs to Replace

Before going live, replace these placeholder URLs with actual service links:

### Booking & Purchases
- `https://example.com/BOOKING-RITUAL-RESET` → Your Podia/booking link for Ritual Reset
- `https://example.com/BUY-SUNSET-SUNRISE` → Product purchase link for Sunset/Sunrise Sync

### Email Signup
- `https://example.com/EMAIL-SIGNUP` → ConvertKit or email service form action URL

### Email Links (Already Set)
- `mailto:digitalwellnessdesigner@gmail.com` - Contact email (ready to use)

**How to Replace:**
```bash
# Search for placeholders
grep -r "example.com" *.html

# Replace with actual URLs in your editor
```

---

## 🚀 Deployment Instructions

### 1. Push to GitHub
```bash
git add .
git commit -m "Complete redesigned Digital Wellness Design website"
git push origin main
```

### 2. Enable GitHub Pages
1. Go to your repo: `github.com/digitalwellnessdesign/io`
2. Settings → Pages
3. Source: Deploy from branch `main`
4. Folder: `/ (root)`
5. Save

### 3. Configure Custom Domain
The `CNAME` file is already set to: `www.digitalwellnessdesign.com`

**In your DNS settings, add:**
- CNAME record: `www` → `digitalwellnessdesign.github.io`
- A records for apex (optional):
  - `185.199.108.153`
  - `185.199.109.153`
  - `185.199.110.153`
  - `185.199.111.153`

**In GitHub Pages settings:**
- Set custom domain: `www.digitalwellnessdesign.com`
- Enable "Enforce HTTPS"

Site will be live at: `https://www.digitalwellnessdesign.com`

---

## ✅ Performance & SEO Features

### Already Implemented
- ✅ Semantic HTML5 with proper heading hierarchy
- ✅ All pages have meta tags (title, description, OpenGraph)
- ✅ Canonical URLs pointing to www.digitalwellnessdesign.com
- ✅ Sitemap.xml with all 11 pages
- ✅ Robots.txt allowing all crawlers
- ✅ Self-hosted fonts with font-display: swap
- ✅ Lazy loading on service illustrations
- ✅ Minimal CSS (single file, no frameworks)
- ✅ No JavaScript required
- ✅ Responsive design (mobile-first)
- ✅ Accessible navigation with focus states
- ✅ Prefers-reduced-motion support
- ✅ High contrast mode support

### Optional Enhancements
- Add hero video to `/assets/videos/` with poster image
- Optimize SVG illustrations (currently large but functional)
- Add WebP versions of any photos you upload
- Set up Google Analytics (add tracking code)
- Add schema.org structured data for services

---

## 📊 Content Source of Truth

All copy comes from your Google Sheet CSV:
```
https://docs.google.com/spreadsheets/d/e/2PACX-1vQprHW003Cyvbr2i96uHPIYfzlTVxwTry2I0uWVZ7EGateW_rZY2WI_2_HnUEbWhN_l-sAcuq0CVauH/pub?output=csv
```

### To Update Content:
1. Edit the Google Sheet
2. Keep `page_slug`, `section_id`, `block_order` stable
3. Update HTML files manually to match
4. Commit and push to GitHub

---

## 🎯 Two Target Audiences Served

### 1. Individuals (Primary)
- Remote creatives seeking iPhone wellness redesign
- Clear paths to: Book Ritual Reset, Email for Sanctuary Session, Join email list
- Services: Ritual Reset ($150), Sanctuary Session (email to apply), Seasonal Syncs (coming soon)
- Product: Sunset + Sunrise Sync ($3)

### 2. Wellness Practitioners (NEW)
- Wellness businesses in Triad/NC seeking websites + listings
- Services: Listing Clarity, Simple Site, Full Presence
- Emphasizes: Credibility, clarity, being found, reduced friction
- CTA: Email to express interest

---

## 📧 Contact & Support

- **Email**: digitalwellnessdesigner@gmail.com
- **Website**: www.digitalwellnessdesign.com
- **Repo**: github.com/digitalwellnessdesign/io

---

## 🧪 Pre-Launch Checklist

- [ ] Replace placeholder URLs with actual booking/payment links
- [ ] Test all internal navigation links
- [ ] Test responsive design on mobile, tablet, desktop
- [ ] Verify all forms submit to correct endpoints
- [ ] Check font loading on different browsers
- [ ] Verify illustrations load correctly
- [ ] Run PageSpeed Insights on key pages
- [ ] Test accessibility with screen reader
- [ ] Verify SEO meta tags on all pages
- [ ] Test on Safari, Chrome, Firefox, Edge

---

**Built with**: HTML, CSS, nature's rhythms, and intention
**Optimized for**: Performance, accessibility, and calm user experiences
**Ready to**: Deploy and serve your wellness-focused audiences
