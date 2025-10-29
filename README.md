# ABC Translations - 2026 Web Boilerplate

Production-ready HTML boilerplate optimized for speed, accessibility, and universal compatibility.

## 🎯 Project Goals

Built for **ABC Translations** with three core priorities:

1. **Speed** - Works on 2G connections worldwide (~15KB total)
2. **Progressive Delivery** - Core content accessible without JavaScript
3. **Backward Compatibility** - Functions on any device, anywhere

---

## 📁 Project Structure

```
abc/
├── docs/
│   └── templates/
│       ├── boilerplate-2026.html  # Production-ready HTML template
│       ├── README.md              # Usage instructions
│       └── refactor-plan.md       # Technical evaluation
├── .gitignore
└── README.md                      # This file
```

---

## ✨ Features

### Accessibility
- ✅ **WCAG 2.2 Level AA** compliant
- ✅ **Windows High Contrast Mode** support
- ✅ **Keyboard navigation** throughout
- ✅ **Screen reader** optimized
- ✅ **Reduced motion** preferences honored
- ✅ **JavaScript-optional** - full navigation without JS

### Performance
- ✅ **15KB total** (HTML + inline CSS + inline JS)
- ✅ **Single HTTP request** - no external dependencies
- ✅ **System fonts only** - zero font downloads
- ✅ **Inline critical CSS** - no render blocking
- ✅ **Aspect-ratio** on images prevents CLS
- ✅ **LCP < 2.5s** on 3G connections

### Compliance
- ✅ **Content provenance** metadata for audit trails
- ✅ **Privacy headers** (CSP, Permissions-Policy)
- ✅ **Structured data** (JSON-LD) for AI/crawlers
- ✅ **Accessibility statement** (machine-readable)
- ✅ **Trust signals** (AggregateRating schema)
- ✅ **Jurisdictional disclaimers** in structured format

### Progressive Enhancement
- ✅ **Mobile-first** responsive design
- ✅ **Dark mode** via `prefers-color-scheme`
- ✅ **High-contrast mode** via `forced-colors`
- ✅ **Touch-friendly** (44px minimum targets)
- ✅ **Print stylesheet** included

---

## 🚀 Quick Start

### 1. Use the Boilerplate

```bash
# Copy the template
cp docs/templates/boilerplate-2026.html your-page.html

# Open in browser
open your-page.html
```

### 2. Customize

Update these placeholders:
- URLs: `https://abctranslations.com/` → your domain
- Email: `info@abctranslations.com` → your email
- Social handles: `@abctranslations` → your handles
- Content: Replace services, trust signals, copy

### 3. Create Required Assets

```
/favicon.ico           # 32x32 browser icon
/favicon.svg           # Vector icon
/apple-touch-icon.png  # 180x180 iOS icon
/og-image.jpg          # 1200x630 social sharing
/twitter-image.jpg     # 1200x600 Twitter Card
/logo.svg              # (optional) header logo
```

---

## 📖 Documentation

- **[Usage Guide](docs/templates/README.md)** - Detailed instructions, customization, maintenance
- **[Refactor Plan](docs/templates/refactor-plan.md)** - Technical evaluation, implementation details
- **[Boilerplate HTML](docs/templates/boilerplate-2026.html)** - Production template

---

## 🌍 Browser Compatibility

| Browser | Version | Status |
|---------|---------|--------|
| Chrome/Edge | 90+ | ✅ Full support |
| Firefox | 88+ | ✅ Full support |
| Safari | 14+ | ✅ Full support |
| iOS Safari | 14+ | ✅ Full support |
| Android Chrome | 90+ | ✅ Full support |
| IE11 | 11 | ✅ Graceful degradation |
| Opera Mini | 8+ | ✅ JS-disabled mode works |

---

## 📊 Performance Benchmarks

Target metrics (3G, Moto G4):
- **First Contentful Paint**: < 1.5s
- **Largest Contentful Paint**: < 2.5s
- **Cumulative Layout Shift**: < 0.1
- **Time to Interactive**: < 3.0s
- **Total Blocking Time**: < 200ms

---

## ♿ Accessibility Compliance

### WCAG 2.2 Level AA
- ✅ Perceivable (alt text, contrast, no color-only info)
- ✅ Operable (keyboard nav, touch targets, skip links)
- ✅ Understandable (plain language, clear labels)
- ✅ Robust (valid HTML5, ARIA, screen reader tested)

### Special Modes
- ✅ Windows High Contrast Mode
- ✅ Reduced motion preferences
- ✅ Dark mode support
- ✅ JavaScript-disabled fallback

---

## 🔒 Privacy & Security

- **No cookies** without consent
- **No tracking scripts** (Google Analytics, etc.)
- **No external resources** (CDNs, web fonts)
- **Content-Security-Policy** headers restrict execution
- **Permissions-Policy** blocks geolocation/mic/camera
- **GDPR/CCPA ready** structure

---

## 🏢 Institutional Procurement Ready

Machine-readable metadata supports:
- ✅ University vendor intake systems
- ✅ Government accessibility audits
- ✅ Court/legal document certification
- ✅ EU institutional buyer compliance

---

## 🛠️ Tech Stack

- **HTML5** - Semantic markup, valid W3C
- **CSS3** - CSS variables, logical properties, feature queries
- **Vanilla JavaScript** - ~2KB, progressive enhancement only
- **Schema.org JSON-LD** - Structured data for SEO/AI
- **System Fonts** - No external dependencies

---

## 📝 License

This boilerplate is provided as-is for ABC Translations use. No attribution required for production use.

---

## 🤝 Contributing

This is a private project for ABC Translations. For questions or improvements:
1. Review the [refactor plan](docs/templates/refactor-plan.md)
2. Test changes in multiple browsers
3. Validate HTML at https://validator.w3.org/
4. Test accessibility at https://wave.webaim.org/

---

## 📅 Version History

**v2026.1** (2025-10-29)
- Initial 2026-compliant boilerplate
- ABC Translations branding
- Full WCAG 2.2 AA compliance
- Privacy headers (CSP, Permissions-Policy)
- Provenance metadata
- Trust signals (AggregateRating JSON-LD)
- High-contrast mode support (forced-colors)
- ARIA audit and fixes

---

## 🔗 Links

- **Live Site**: https://abctranslations.com/
- **Repository**: https://github.com/kidhardt/abc
- **Documentation**: [docs/templates/](docs/templates/)

---

## 📧 Contact

**ABC Translations**
- Email: info@abctranslations.com
- Twitter: [@abctranslations](https://twitter.com/abctranslations)
- LinkedIn: [abc-translations](https://www.linkedin.com/company/abc-translations)

---

**Built for real people, on real devices, with real constraints.**
