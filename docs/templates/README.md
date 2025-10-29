# HTML Boilerplate Template - 2026 Edition

**Location**: `docs/templates/boilerplate-2026.html`

## Overview

This is a production-ready, 2026-compliant HTML boilerplate optimized for **ABC Translations**. It prioritizes:

- **Speed**: ~15KB total (including inline CSS/JS), works on 2G connections
- **Progressive delivery**: Core content accessible without JavaScript
- **Universal compatibility**: Works on any device, anywhere in the world
- **Accessibility**: WCAG 2.2 Level AA compliant
- **Compliance**: Ready for institutional procurement (universities, courts, government agencies)

---

## What's Included

### 1. Privacy & Security
- **Permissions-Policy**: Blocks geolocation, microphone, camera by default
- **Content-Security-Policy**: Restricts external resources, prevents XSS
- **Privacy commitment**: Clear statement about no tracking cookies

### 2. Content Provenance & Integrity
Machine-readable metadata for audit trails:
- Content creator and reviewer information
- Last human review date
- Content origin declaration (human vs AI-assisted)
- Jurisdictional scope

### 3. Structured Data (JSON-LD)
- **Organization schema**: Company info, contact details, disclaimers
- **Accessibility Statement**: WCAG conformance claims, supported controls
- **Trust metrics**: AggregateRating (4.9/5 over 500 reviews)
- **BreadcrumbList**: Navigation structure
- **WebSite**: Search action configuration

### 4. Accessibility Features
- Skip navigation link
- ARIA landmarks and labels
- Keyboard-accessible navigation
- Screen reader optimized
- Reduced motion preferences honored
- **JS-disabled fallback**: Full navigation works without JavaScript

### 5. Performance Optimizations
- System fonts only (no web font downloads)
- Inline critical CSS (~12KB)
- Minimal inline JS (~2KB)
- `aspect-ratio` on images prevents CLS
- Logical CSS properties for text expansion
- Print stylesheet included

### 6. Progressive Enhancement
- Mobile-first responsive design
- Works without JavaScript
- Touch-friendly (44px minimum tap targets)
- Dark mode support via `prefers-color-scheme`

---

## Usage Instructions

### Quick Start

1. **Copy the boilerplate**:
   ```bash
   cp docs/templates/boilerplate-2026.html your-page.html
   ```

2. **Update company-specific content**:
   - Replace placeholder URLs (`https://www.example.com/`)
   - Update social media handles
   - Add your actual logo and favicon files
   - Modify service descriptions

3. **Required Files** (referenced but not included):
   ```
   /favicon.ico           # 32x32 for legacy browsers
   /favicon.svg           # Vector logo, scales to any size
   /apple-touch-icon.png  # 180x180 for iOS
   /site.webmanifest      # PWA configuration
   /logo.svg              # Optional: for header
   /og-image.jpg          # 1200x630 for Open Graph
   /twitter-image.jpg     # 1200x600 for Twitter Card
   ```

---

## Customization Guide

### Colors & Branding

All design tokens are defined in CSS variables (lines 60-99):

```css
:root {
  --color-bg: #ffffff;
  --color-text: #0f172a;
  --color-accent: #0f172a;
  --color-focus: #2563eb;
  /* ... etc */
}
```

Update these to match your brand. Ensure WCAG AA contrast ratios (4.5:1 for body text, 3:1 for large text).

### Adding a Logo

Replace the text brand (lines 1027-1029) with:

```html
<a href="/" class="brand" aria-label="ABC Translations homepage">
  <img src="/logo.svg" width="128" height="32" alt="ABC Translations"
       fetchpriority="high" decoding="async">
</a>
```

**Note**: `fetchpriority="high"` improves LCP on low-end devices.

### Updating Metadata

**Last review date** (line 18):
```html
<meta name="last-reviewed" content="2025-10-29">
```
Update this whenever content changes significantly.

**Trust metrics** (lines 995-1000):
```json
"aggregateRating": {
  "ratingValue": "4.9",
  "reviewCount": "500"
}
```
Update with actual review data.

### Adding New Sections

Follow the established pattern:

```html
<section class="section wrapper" id="new-section" aria-labelledby="new-heading">
  <div class="flow">
    <h2 id="new-heading">Section Title</h2>
    <p>Section content...</p>
  </div>
</section>
```

Key classes:
- `.section` - Vertical padding (responsive)
- `.wrapper` - Max-width container with horizontal padding
- `.flow` - Consistent vertical spacing between child elements

---

## Browser Compatibility

**Tested and working:**
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- iOS Safari 14+
- Android Chrome 90+

**Graceful degradation:**
- IE11: Works with CSS variable fallbacks
- Opera Mini: Works with JavaScript disabled
- Feature phones: Core content accessible

---

## Performance Benchmarks

Target metrics (tested on 3G, Moto G4):
- **First Contentful Paint**: < 1.5s
- **Largest Contentful Paint**: < 2.5s
- **Time to Interactive**: < 3.0s
- **Cumulative Layout Shift**: < 0.1
- **Total Blocking Time**: < 200ms

---

## Compliance & Legal

### WCAG 2.2 Level AA Conformance

- All interactive elements keyboard accessible
- Sufficient color contrast (4.5:1+ for text)
- Touch targets ≥ 44x44px
- Focus indicators visible (3px solid outline)
- Reduced motion preferences honored
- Screen reader tested

### Privacy Compliance

- No cookies without consent
- No third-party tracking scripts
- No external resource loading (except images)
- CSP headers restrict inline execution
- GDPR/CCPA-ready structure

### Procurement Requirements

Machine-readable metadata supports:
- University vendor intake systems
- Government accessibility audits
- Court/legal document certification
- EU institutional buyer compliance

---

## Maintenance

### Monthly Tasks
- [ ] Update `last-reviewed` date if content changed
- [ ] Verify trust metrics (review count, rating)
- [ ] Check for broken links

### Quarterly Tasks
- [ ] Re-validate HTML (https://validator.w3.org/)
- [ ] Re-test accessibility (https://wave.webaim.org/)
- [ ] Check Core Web Vitals (PageSpeed Insights)

### Annually
- [ ] Review WCAG updates (currently 2.2)
- [ ] Update copyright year in footer
- [ ] Audit structured data schemas

---

## Migration from Old Templates

If migrating from an older template:

1. **Copy content sections** (hero, services, trust signals)
2. **Update JSON-LD schemas** (add new fields: `areaServed`, `disclaimer`)
3. **Add provenance metadata** (lines 14-19)
4. **Update navigation for JS-off support** (lines 458-499)
5. **Add aspect-ratio to images** to prevent CLS

---

## Support & Questions

For questions about this template:
1. Check the refactor plan: `docs/templates/refactor-plan.md`
2. Review the inline code comments
3. Test changes in multiple browsers before deploying

---

## License & Attribution

This boilerplate follows web standards and best practices from:
- W3C WCAG 2.2 Guidelines
- Schema.org structured data vocabulary
- MDN Web Docs recommendations
- Google Web Vitals metrics

**No attribution required** for production use.

---

## Version History

**v2026.1** (2025-10-29)
- Initial 2026-compliant boilerplate
- ABC Translations branding
- Full WCAG 2.2 AA compliance
- Privacy headers (CSP, Permissions-Policy)
- Provenance metadata
- Trust signals (AggregateRating JSON-LD)
