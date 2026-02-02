# Digital Wellness Design - Deployment Guide

## Clean URL Structure

This site now uses clean URLs without `.html` extensions for better SEO and user experience.

### URL Structure

All pages use folder-based routing with clean URLs:

- `/about.html` → `/about`
- `/practitioners.html` → `/for-businesses`
- `/services.html` → `/services`
- `/contact.html` → `/contact`
- `/iphone-ritual-reset.html` → `/iphone-ritual-reset`
- `/iphone-sanctuary-session.html` → `/iphone-sanctuary-session`
- `/iphone-seasonal-syncs.html` → `/iphone-seasonal-syncs`
- `/sunset-sunrise-sync.html` → `/sunset-sunrise-sync`
- `/privacy.html` → `/privacy`
- `/terms.html` → `/terms`

### Folder Structure

Each page is in its own directory with an `index.html` file:

```
/
├── index.html (homepage)
├── about/
│   └── index.html
├── for-businesses/
│   └── index.html
├── services/
│   └── index.html
├── contact/
│   └── index.html
├── iphone-ritual-reset/
│   └── index.html
└── ...
```

## Deployment

### Netlify

1. Connect your Git repository to Netlify
2. Build settings are configured in `netlify.toml`
3. The `_redirects` file handles old URLs automatically with 301 redirects
4. Deploy command: `npm run build` (no actual build needed for static site)
5. Publish directory: `.` (root)

### Cloudflare Pages

1. Connect your Git repository to Cloudflare Pages
2. Build command: `npm run build`
3. Build output directory: `.` (root)
4. The `_redirects` file will handle old URLs automatically

### Other Static Hosts

Most modern static hosting providers support folder-based routing automatically. If your host doesn't:

1. Ensure your host serves `index.html` files when accessing directories
2. Configure 301 redirects from old `.html` URLs to new clean URLs using the `_redirects` file

## Performance Optimizations

The site now includes:

### Mobile-First Design
- ✅ Responsive breakpoints at 480px, 768px, and 1024px
- ✅ Touch-friendly targets (44px minimum for buttons and links)
- ✅ Optimized typography scaling for small screens
- ✅ Mobile-optimized navigation and spacing

### Performance Enhancements
- ✅ DNS prefetching for Google Fonts
- ✅ Progressive web app meta tags
- ✅ iOS home screen app support
- ✅ Optimized viewport settings with `viewport-fit=cover`
- ✅ Theme color for browser UI
- ✅ Long-term caching for static assets (CSS, JS, fonts, images)
- ✅ Security headers (X-Frame-Options, X-Content-Type-Options, etc.)
- ✅ Hardware acceleration hints for animations
- ✅ Reduced motion support for accessibility

### Asset Optimization
- ✅ Font display swap for faster text rendering
- ✅ Optimized image loading with lazy loading hints
- ✅ Content visibility optimization for off-screen content

## Testing Locally

```bash
npm run dev
```

This will serve the site locally at `http://localhost:3000`. Most local servers handle folder-based routing automatically.

## SEO Considerations

- ✅ `sitemap.xml` updated with clean URLs
- ✅ All canonical URLs updated in HTML files
- ✅ All Open Graph URLs updated for social sharing
- ✅ 301 redirects configured for old URLs to preserve SEO
- ✅ Updated lastmod dates in sitemap to 2026-02-02

## Performance Targets

Site is optimized for 90+ PageSpeed scores:

- **Mobile**: Optimized touch targets, responsive images, efficient caching
- **Desktop**: Fast rendering, optimized fonts, minimal layout shifts
- **Core Web Vitals**: Improved LCP, FID, and CLS scores

## Domain

The site remains on: `www.digitalwellnessdesign.com`

No domain changes required.

## Notes

- All marketing copy and visual styling preserved
- No design changes or color scheme modifications
- Structural update only for better URLs and mobile experience
- Ready for deployment to any modern static hosting platform
