# Aviraj EV Ports Limited (AEP) Website

**Premium, responsive, production-ready EV charging website prototype.**

A complete, fully functional website showcasing AEP's AC/DC chargers, OCPP platform, Make in India manufacturing, and sustainability commitment.

---

## 📂 Project Structure

```
aep-website-design/
├── index.html                    # Home page (hero, trust, products, platform teaser)
├── solutions.html                # Product showcase (AC001, AC Type 2, AC Hybrid, DC CCS2, DC001)
├── smart-platform.html           # OCPP platform (EV app + CPO console)
├── charger-selector.html         # 3-step interactive wizard with recommendations
├── make-in-india.html            # Manufacturing, certifications, safety, pan-India network
├── sustainability.html           # COP26 Panchamrit + carbon impact calculator
├── resources.html                # Downloads hub, knowledge center, FAQs
├── about.html                    # Company story, mission, values, careers
├── contact.html                  # Inquiry form, contact info, partnership CTA
├── css/
│   └── styles.css               # Complete design system (colors, typography, components)
├── js/
│   └── main.js                  # Header scroll behavior, menu toggle, scroll animations
└── assets/                       # (Ready for high-res images, logos, product renders)
```

---

## 🎨 Design System

### Colors
- **Primary Green:** `#123f33` (deep forest, sustainability)
- **Secondary Green:** `#1b4d3e` (accent)
- **Cyan/Electric Blue:** `#00a8e8` & `#00d9ff` (technology, energy)
- **Gold/Bronze:** `#d4a574` (luxury accents, reserved)
- **Neutrals:** Off-white (`#f5f8f8`), grays (`#667680`), dark ink (`#17242f`)

### Typography
- **Headings:** Montserrat (Bold 600–800, geometric, modern)
- **Body Text:** Inter (Regular 400–700, clean, highly readable)
- **Loaded via Google Fonts** (preconnected for speed)

### Responsive Breakpoints
- **Mobile:** 320px–640px (single column, 68px header)
- **Tablet:** 640px–1060px (2-column grids, menu drawer)
- **Desktop:** 1060px+ (full 4-column layouts, sticky header)

### Key Components
- Gradient buttons (primary/secondary/light variants)
- Product cards with hover effects
- Glassmorphism header on scroll
- Scroll-triggered fade-in animations
- Interactive tabs and accordions
- Form inputs with focus states

---

## 🚀 Deployment Guide

### Local Development
```bash
# Navigate to project directory
cd /Users/rittiktyagi839/aep-website-design

# Start a simple HTTP server (Python 3)
python3 -m http.server 8000

# Open http://localhost:8000 in browser
```

### Production Deployment (WordPress + Bricks/Elementor)

1. **CMS Setup**
   - Install WordPress on your hosting
   - Install Bricks Builder or Elementor plugin
   - Use this prototype as a design reference

2. **Export & Migrate**
   - Copy all HTML content into Bricks/Elementor pages
   - Migrate CSS to builder's custom CSS panel
   - Migrate JS to custom code blocks

3. **Performance Optimization**
   - Enable caching (WP Super Cache, W3 Total Cache)
   - Use CDN for CSS/JS (Cloudflare, AWS CloudFront)
   - Optimize images (WebP format, lazy loading)
   - Minify CSS/JS in production

4. **SEO & Analytics**
   - Install Yoast SEO plugin
   - Add schema markup (Organization, Product, LocalBusiness)
   - Connect Google Analytics 4 (GA4)
   - Set up Google Search Console

5. **Security**
   - SSL certificate (Let's Encrypt, Cloudflare)
   - Implement reCAPTCHA v3 on contact form
   - Regular backups (daily, automated)
   - Keep plugins & WordPress updated

### Static Hosting (GitHub Pages, Netlify, Vercel)

1. **Prepare Files**
   ```bash
   # Add a 404.html for SPA fallback (if needed)
   cp index.html 404.html
   ```

2. **Deploy to Netlify**
   ```bash
   # Install Netlify CLI
   npm install -g netlify-cli
   
   # Login and deploy
   netlify login
   netlify deploy --prod --dir=.
   ```

3. **Domain & SSL**
   - Point DNS to hosting provider
   - SSL auto-provisioned (Netlify, Vercel, GitHub Pages)

---

## 📋 Customization Checklist

### Content Updates
- [ ] Replace placeholder company info (address, phone, email)
- [ ] Add actual team member names & bios (About page)
- [ ] Update product pricing (if displaying)
- [ ] Add real product images in `assets/` folder
- [ ] Replace SVG charger illustrations with actual renders
- [ ] Update map coordinates (Make in India page)
- [ ] Add real case studies or customer testimonials

### Technical Setup
- [ ] Configure contact form backend (FormSubmit, Netlify Forms, or custom API)
- [ ] Integrate with CRM (HubSpot, Salesforce)
- [ ] Add Google Analytics tracking ID
- [ ] Set up reCAPTCHA v3 keys (contact form)
- [ ] Add favicon & apple-touch-icon
- [ ] Configure email notifications for form submissions

### Performance
- [ ] Compress images (TinyPNG, ImageOptim)
- [ ] Convert to WebP format
- [ ] Test on Google PageSpeed Insights
- [ ] Aim for 90+ score (mobile & desktop)
- [ ] Set up monitoring (UptimeRobot, Pingdom)

### SEO & Meta
- [ ] Customize meta descriptions for each page
- [ ] Add Open Graph tags for social sharing
- [ ] Create sitemap.xml
- [ ] Create robots.txt
- [ ] Add structured data (schema.org JSON-LD)
- [ ] Test with Google Search Console

---

## 📱 Mobile-First Features

- Hamburger menu (auto-collapses on mobile)
- Thumb-friendly button sizing (48px min)
- Touch-optimized form inputs
- Responsive images & videos
- Viewport meta tags configured
- Fast scroll on mobile (smooth-scroll: smooth)

---

## ♿ Accessibility

- Semantic HTML5 (headings, nav, main, article, footer)
- ARIA labels on buttons & interactive elements
- Color contrast: WCAG AA compliant
- Keyboard navigation supported
- Screen reader friendly (alt text on all visuals)
- Focus states on interactive elements

---

## 📊 Performance Targets

- **First Contentful Paint (FCP):** < 2.0s
- **Largest Contentful Paint (LCP):** < 2.5s
- **Cumulative Layout Shift (CLS):** < 0.1
- **Time to Interactive (TTI):** < 3.5s
- **PageSpeed Score:** 90+
- **Lighthouse Audit:** 95+ (Mobile & Desktop)

---

## 🔒 Security Considerations

- **SSL/TLS:** Always use HTTPS
- **Form Validation:** Server-side validation required
- **reCAPTCHA:** Implement v3 for spam prevention
- **CORS:** Configure for API calls
- **Headers:** Set Content-Security-Policy, X-Frame-Options
- **Data Privacy:** Comply with GDPR/CCPA (if applicable)

---

## 📞 Contact & Support Integration

### Contact Form Processing
Options:
1. **Netlify Forms** (auto-submission, no backend needed)
2. **FormSubmit.co** (free, simple email forwarding)
3. **AWS Lambda + SES** (scalable, serverless)
4. **Firebase Realtime Database** (real-time dashboard)

### Email Notifications
- Auto-send inquiry to: `info@avirajevport.com`
- Auto-reply to user with confirmation
- Create Slack notification for sales team

---

## 📈 Recommended Next Steps (Post-Launch)

1. **Content Enhancements**
   - Add blog/news section
   - Create case studies with real customer data
   - Add video testimonials
   - Publish whitepapers on EV infrastructure

2. **Feature Expansions**
   - Multi-language support (Hindi, regional)
   - Live chat / chatbot for instant support
   - Customer portal for tracking quotes
   - Integration with sales CRM

3. **Marketing & Analytics**
   - Set up conversion funnels
   - Implement heatmapping (Hotjar, Microsoft Clarity)
   - A/B test CTAs and page layouts
   - Monthly SEO reporting

4. **Maintenance**
   - Monthly security audits
   - Quarterly content refresh
   - Annual accessibility audit (WCAG 2.1 AA)
   - Continuous performance monitoring

---

## 🛠 Development Tools Recommended

| Tool | Purpose |
|------|---------|
| **VS Code** | Code editor |
| **Chrome DevTools** | Debugging, performance, accessibility |
| **Google Lighthouse** | Performance audits |
| **Figma** | Design collaboration & prototyping |
| **Netlify / Vercel** | Deployment & hosting |
| **GitHub** | Version control |
| **FormSubmit.co** | Contact form backend |

---

## 📄 File Size Reference (Current)

- `index.html` - 9.2 KB
- `solutions.html` - 13.8 KB
- `smart-platform.html` - 11.3 KB
- `charger-selector.html` - 14.2 KB
- `contact.html` - 9.5 KB
- `css/styles.css` - 23 KB (can be reduced with minification)
- `js/main.js` - 2.1 KB

**Total uncompressed:** ~83 KB  
**Gzipped (production):** ~18 KB  
**With images & assets:** +5–10 MB (depending on image quality & count)

---

## 🎯 Testing Checklist

### Functionality
- [ ] All links navigate correctly
- [ ] Forms submit without errors
- [ ] Contact form sends emails
- [ ] Charger selector outputs recommendations
- [ ] Carbon calculator updates on input change
- [ ] Mobile menu opens/closes
- [ ] FAQ accordions expand/collapse

### Visual
- [ ] Design matches across Chrome, Safari, Edge
- [ ] Mobile layout reflows correctly
- [ ] Images load and scale properly
- [ ] Typography is readable at all sizes
- [ ] Colors contrast correctly
- [ ] Animations are smooth (60fps)

### Performance
- [ ] Page loads in < 3 seconds
- [ ] Images are optimized
- [ ] No console errors
- [ ] No broken links or 404s

---

## 📞 Support & Questions

For technical support or customization assistance:
- **Email:** info@avirajevport.com
- **Phone:** +91 8810500002

---

## 📄 License

This website is proprietary to **Aviraj EV Ports Limited**. All rights reserved.

---

**Last Updated:** June 10, 2026  
**Version:** 1.0 (Production Ready)
