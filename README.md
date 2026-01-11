# Digital Wellness Design Website

A calm, premium, nature-inspired static website for Digital Wellness Design — helping remote creatives redesign their iPhone screens for wellness.

## 🌿 Overview

This is a static HTML/CSS website with:
- Clean, semantic HTML5
- Custom CSS with nature-inspired color palette
- Self-hosted typography (Loubag for headings)
- Responsive design with mobile-first approach
- Performance-optimized for 90+ PageSpeed scores
- Accessible navigation and semantic structure

## 📁 Project Structure

```
/
├── index.html              # Home page
├── about.html              # About Meg Feil
├── services.html           # Services overview
├── iphone-ritual-reset.html
├── iphone-sanctuary-session.html
├── iphone-seasonal-syncs.html
├── sunset-sunrise-sync.html
├── practitioners.html      # For wellness practitioners
├── contact.html
├── privacy.html
├── terms.html
├── sitemap.xml
├── robots.txt
├── CNAME
├── styles/
│   └── global.css         # All CSS styles
├── fonts/
│   ├── loubag-semi-bold.ttf
│   └── gistesy.ttf
├── assets/
│   ├── illustrations/
│   │   ├── ritual.svg
│   │   ├── sanctuary.svg
│   │   └── seasonal.svg
│   ├── images/            # Add hero images, photos here
│   └── videos/            # Add hero video here
└── README.md
```

## 🎨 Design System

### Colors
- **Cream**: `#FAF8F5` (background)
- **Sand**: `#E8E3DA` (borders, alt backgrounds)
- **Warm Gray**: `#9D9789`
- **Stone**: `#6B6557` (body text)
- **Charcoal**: `#3A3832` (headings)
- **Sage**: `#8B9D83` (primary brand)
- **Forest**: `#5A6B52` (CTA buttons)
- **Terracotta**: `#C17A5F` (accents)
- **Sunlight**: `#F5E6D3` (warm backgrounds)
- **Sunrise**: `#FFD4A3` (gradients)

### Typography
- **Headings**: Loubag (self-hosted, semi-bold)
- **Body**: Inter (Google Fonts fallback)
- **Spacing**: 8px base unit system
- **Line heights**: 1.2 (tight/headings), 1.6 (body), 1.8 (relaxed)

## ✏️ Content Updates via CSV

All page content is sourced from this Google Sheet (published as CSV):
```
https://docs.google.com/spreadsheets/d/e/2PACX-1vQprHW003Cyvbr2i96uHPIYfzlTVxwTry2I0uWVZ7EGateW_rZY2WI_2_HnUEbWhN_l-sAcuq0CVauH/pub?output=csv
```

### How to Update Content

1. **Edit the CSV/Google Sheet**
   - Update copy in the `content` column
   - Keep `page_slug`, `section_id`, and `block_order` intact
   - Add new rows following the existing structure

2. **Apply Changes to HTML**
   - Fetch the updated CSV
   - Update corresponding HTML files manually
   - Match content by `page_slug` + `section_id` + `block_order`

3. **Preserve Voice**
   - Keep Meg's authentic voice
   - Refine for clarity, not for hype
   - Minimal new copy beyond what's in the CSV

### CSV Structure
```
page_slug | page_title | section_id | block_order | block_type | content | cta_text | cta_url | notes
```

## 🚀 Deployment to GitHub Pages

### Initial Setup

1. **Push to GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Digital Wellness Design website"
   git branch -M main
   git remote add origin https://github.com/digitalwellnessdesign/io.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Source: Deploy from branch `main`
   - Folder: `/ (root)`
   - Save

3. **Custom Domain Setup**
   - Add a `CNAME` file to root with:
     ```
     www.digitalwellnessdesign.com
     ```
   - In your DNS settings, add:
     - CNAME record: `www` → `digitalwellnessdesign.github.io`
     - A records for apex domain (if needed):
       - `185.199.108.153`
       - `185.199.109.153`
       - `185.199.110.153`
       - `185.199.111.153`
   - In GitHub Pages settings, set custom domain to `www.digitalwellnessdesign.com`
   - Enable "Enforce HTTPS"

### Making Updates

1. **Edit files locally**
2. **Commit changes**
   ```bash
   git add .
   git commit -m "Update: description of changes"
   git push
   ```
3. **GitHub Pages auto-deploys** (usually within 1-2 minutes)

## 🔗 External Service Placeholders

The following URLs need to be replaced with actual booking/payment links:

- **Ritual Reset booking**: `https://example.com/BOOKING-RITUAL-RESET`
- **Sunset/Sunrise product**: `https://example.com/BUY-SUNSET-SUNRISE`
- **Email signup form**: `https://example.com/EMAIL-SIGNUP`
- **Sanctuary Session**: Email to `digitalwellnessdesigner@gmail.com`
- **Seasonal Syncs**: Coming soon

### How to Update External Links

1. Search files for placeholder URLs (e.g., `example.com`)
2. Replace with actual Podia, Calendly, ConvertKit, or other service URLs
3. Test all CTAs after updating

## 📊 Performance Optimization

### Current Optimizations
- Minimal CSS (single file, no frameworks)
- No JavaScript (except forms if needed)
- Self-hosted fonts with `font-display: swap`
- Lazy loading for images below fold
- Semantic HTML for fast parsing
- Preconnect hints for Google Fonts (Inter fallback)

### To Add (Future)
- Hero video with poster image
- Compressed/optimized images (WebP format)
- Preload critical assets
- Service worker for offline support (optional)

## ♿ Accessibility

- Semantic HTML5 elements
- Proper heading hierarchy (h1 → h2 → h3)
- Focus visible styles for keyboard navigation
- Color contrast ratios meet WCAG AA
- Alt text for all images
- Prefers-reduced-motion support

## 🧪 Testing Checklist

- [ ] All internal links work
- [ ] All external placeholder URLs marked for replacement
- [ ] Responsive on mobile (320px), tablet (768px), desktop (1280px+)
- [ ] All forms submit to correct endpoints
- [ ] Images load with lazy loading
- [ ] Fonts load correctly
- [ ] SEO meta tags present on all pages
- [ ] Sitemap.xml accessible
- [ ] Robots.txt accessible
- [ ] PageSpeed score 90+ on key pages

## 📧 Contact

Questions or updates needed? Email [digitalwellnessdesigner@gmail.com](mailto:digitalwellnessdesigner@gmail.com)

---

**Built with**: HTML, CSS, nature's rhythms, and intention
**Hosted on**: GitHub Pages
**Domain**: www.digitalwellnessdesign.com (staging: digitalwellnessdesign.github.io)
