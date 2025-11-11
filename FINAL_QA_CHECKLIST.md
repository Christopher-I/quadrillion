# Silicon Century Capital - Final QA Checklist

**Before Launch - Quality Assurance**

---

## 🎨 Design & Brand Consistency

### Visual Design
- [ ] All pages use consistent dark navy (#0d1f3c) background for hero sections
- [ ] All pages use consistent bronze (#b8956a) for accent colors
- [ ] All pages use light grey (#dee5e5) for section backgrounds
- [ ] Logo appears correctly on all pages (white version on dark navy, dark version on light backgrounds)
- [ ] Bronze tagline "Private Investment for the New Industrial Core" appears in footer on all pages
- [ ] All custom icons (Core Principles, Investment Characteristics) are properly displayed
- [ ] All images are high quality and properly sized (no pixelation or stretching)

### Typography
- [ ] All headlines use Playfair Display, 600 weight
- [ ] All body copy uses Nanum Gothic, 400 weight
- [ ] Line height is 1.7 for all body text
- [ ] Font sizes are consistent across similar elements (headlines, subheadlines, body)
- [ ] No typography inconsistencies or random font changes

### Spacing & Layout
- [ ] Consistent padding/margins across all sections
- [ ] Proper spacing between sections (visual breathing room)
- [ ] No overlapping elements or broken layouts
- [ ] Grid layouts align properly (4-column sections, 2-column sections)

---

## 📱 Responsive Design

### Desktop (1920px+)
- [ ] Home page displays correctly
- [ ] About/Strategy page displays correctly
- [ ] Investment Focus/Sectors page displays correctly
- [ ] Contact page displays correctly
- [ ] Portfolio page displays correctly
- [ ] Privacy Policy page displays correctly
- [ ] Terms of Use page displays correctly
- [ ] Footer displays in 4-column layout

### Tablet (768px - 1024px)
- [ ] All pages display correctly
- [ ] Navigation collapses appropriately
- [ ] Footer stacks to 2-column layout
- [ ] Images resize appropriately
- [ ] No horizontal scrolling issues
- [ ] Touch targets are appropriately sized

### Mobile (320px - 767px)
- [ ] All pages display correctly
- [ ] Navigation becomes hamburger menu (if applicable)
- [ ] Footer stacks to single column
- [ ] Images scale down appropriately
- [ ] Text is readable (not too small)
- [ ] Forms are easy to fill out on mobile
- [ ] No horizontal scrolling issues
- [ ] Touch targets are minimum 44px × 44px

---

## 🔗 Navigation & Links

### Header Navigation
- [ ] Logo links to homepage
- [ ] All navigation links work correctly
- [ ] Active page state is indicated (if applicable)
- [ ] Navigation is consistent across all pages
- [ ] "Connect With Us" CTA button works (links to Contact page)

### Footer Navigation
- [ ] All footer links work correctly (About, Investment Focus, Contact, etc.)
- [ ] Privacy Policy link works
- [ ] Terms of Use link works
- [ ] Legal Disclosure link works (if added)
- [ ] No broken links or 404 errors

### Internal Links
- [ ] All internal page links work correctly
- [ ] Anchor links work (if any, e.g., "Jump to section")
- [ ] Email links open email client correctly:
  - investors@siliconcenturycapital.com
  - deals@siliconcenturycapital.com
  - privacy@siliconcenturycapital.com (Privacy Policy page)
  - legal@siliconcenturycapital.com (Terms of Use page)
  - contact@siliconcenturycapital.com (general)

### External Links
- [ ] Tunnel to Towers foundation link works (if applicable)
- [ ] mikeroweWORKS foundation link works (if applicable)
- [ ] All external links open in new tab (target="_blank")
- [ ] All external links have rel="noopener noreferrer" for security

---

## 📝 Content & Copy

### Proofreading
- [ ] All content has been proofread for typos and grammatical errors
- [ ] Company name "Silicon Century Capital" is spelled correctly everywhere
- [ ] George's name and title are correct on About page
- [ ] No placeholder text (Lorem ipsum, [Insert text here], etc.)
- [ ] No overly verbose copy (trimmed per George's direction)
- [ ] Consistent voice and tone across all pages

### Factual Accuracy
- [ ] "$400M+ EBITDA improvement" stat is correct (Investment Focus page)
- [ ] "30+ Years experience" stat is correct (Investment Focus page)
- [ ] All sector descriptions are accurate
- [ ] All transaction types are accurate
- [ ] George's bio and background are accurate
- [ ] Contact information is correct (location: Dallas-Fort Worth Metroplex, Texas)

### Legal & Compliance
- [ ] Privacy Policy has correct effective date
- [ ] Terms of Use has correct effective date
- [ ] "No offer to sell securities" disclaimer appears on Terms of Use page
- [ ] Accredited investor language is present and correct
- [ ] SEC compliance disclaimers are present (no general solicitation)
- [ ] All confidentiality notices are present

---

## 🖼️ Images & Media

### Image Quality
- [ ] All images are high resolution (no pixelation)
- [ ] All images load correctly (no broken images)
- [ ] All images have appropriate alt text for accessibility
- [ ] Images are optimized for web (file size < 500KB ideally)
- [ ] No copyright issues (all images are licensed or owned)

### Specific Images to Check
- [ ] Semiconductor wafer background (Home page hero)
- [ ] Semiconductor clean room image (About page, Investment Focus page)
- [ ] Carousel images for 4 sectors (Home page)
- [ ] Robotics image (replaced with better quality version)
- [ ] George's photo (About page - Meet Our Founder section)
- [ ] Tunnel to Towers logo (if applicable)
- [ ] mikeroweWORKS logo (if applicable)
- [ ] All 4 Core Principles icons (About page)
- [ ] All 4 Investment Characteristics icons (Investment Focus page)
- [ ] Portfolio page placeholder images (if any)

### Animations
- [ ] Home page hero animation works: "Capital ━━━━━ Capability"
- [ ] Carousel on Home page works smoothly
- [ ] No jarring or broken animations
- [ ] Animations don't cause performance issues

---

## 📧 Forms & Functionality

### Contact Form
- [ ] Name field works correctly
- [ ] Email field works correctly (validates email format)
- [ ] Message field works correctly
- [ ] Submit button works
- [ ] Form submissions are sent to correct email address
- [ ] Thank you message appears after submission
- [ ] Form validation works (required fields, email format)
- [ ] No spam submissions (consider adding reCAPTCHA if needed)

### Email Links
- [ ] investors@siliconcenturycapital.com is set up and working
- [ ] deals@siliconcenturycapital.com is set up and working
- [ ] All email links open email client correctly (mailto: links)

---

## 🔍 SEO & Technical

### Page Titles
- [ ] Home: "Silicon Century Capital | Private Investment for Industrial Innovation"
- [ ] About: "About & Strategy | Silicon Century Capital"
- [ ] Investment Focus: "Investment Focus & Sectors | Silicon Century Capital"
- [ ] Contact: "Contact Us | Silicon Century Capital"
- [ ] Portfolio: "Portfolio | Silicon Century Capital"
- [ ] Privacy Policy: "Privacy Policy | Silicon Century Capital"
- [ ] Terms of Use: "Terms of Use | Silicon Century Capital"
- [ ] All titles are ≤ 60 characters

### Meta Descriptions
- [ ] All pages have unique, compelling meta descriptions
- [ ] All meta descriptions are 150-155 characters
- [ ] Meta descriptions include relevant keywords (semiconductors, PE, industrial, etc.)

### URL Structure
- [ ] Homepage: / or /home
- [ ] About: /about or /strategy
- [ ] Investment Focus: /investment-focus or /sectors
- [ ] Contact: /contact
- [ ] Portfolio: /portfolio
- [ ] Privacy Policy: /privacy-policy
- [ ] Terms of Use: /terms-of-use
- [ ] All URLs are clean (no special characters, lowercase, hyphen-separated)

### Technical SEO
- [ ] Favicon is set up and displays correctly
- [ ] Robots.txt file exists (if needed)
- [ ] Sitemap.xml is generated and submitted to Google Search Console
- [ ] Google Analytics is set up (if applicable)
- [ ] Page load speed is acceptable (< 3 seconds on desktop, < 5 seconds on mobile)
- [ ] No broken links (use broken link checker)
- [ ] HTTPS is enabled (SSL certificate installed)
- [ ] Schema markup is implemented (Organization schema)

---

## ♿ Accessibility

### Color Contrast
- [ ] Text has sufficient contrast against backgrounds (WCAG AA minimum)
- [ ] Dark navy (#0d1f3c) text on white background is readable
- [ ] White text on dark navy (#0d1f3c) background is readable
- [ ] Bronze (#b8956a) text has sufficient contrast

### Keyboard Navigation
- [ ] All interactive elements are keyboard accessible (Tab key navigation)
- [ ] Focus states are visible (outline on focused elements)
- [ ] Forms can be filled out using keyboard only
- [ ] Navigation menu can be accessed via keyboard

### Screen Readers
- [ ] All images have descriptive alt text
- [ ] Form fields have proper labels
- [ ] Heading hierarchy is logical (H1, H2, H3, etc.)
- [ ] Links have descriptive text (not just "Click here")

---

## 🚀 Performance

### Load Times
- [ ] Home page loads in < 3 seconds
- [ ] All other pages load in < 3 seconds
- [ ] Images are lazy-loaded (if applicable)
- [ ] No render-blocking resources

### File Sizes
- [ ] All images are compressed and optimized
- [ ] No unnecessarily large files (> 1MB)
- [ ] CSS and JavaScript are minified (Webflow handles this automatically)

---

## 🧪 Browser Testing

### Desktop Browsers
- [ ] Google Chrome (latest version)
- [ ] Safari (latest version)
- [ ] Firefox (latest version)
- [ ] Microsoft Edge (latest version)

### Mobile Browsers
- [ ] Safari (iOS)
- [ ] Chrome (Android)
- [ ] Samsung Internet (Android)

### Check for
- [ ] Layout consistency across browsers
- [ ] Font rendering consistency
- [ ] Animation/interaction consistency
- [ ] No browser-specific bugs

---

## 📊 Portfolio Page Specific

### CMS Setup (Webflow)
- [ ] "Portfolio Companies" CMS collection is created
- [ ] Fields are properly configured:
  - Company Name (Plain text)
  - Company Logo (Image)
  - Industry Sector (Option field with 4 sectors)
  - Short Description (Plain text, 150 characters)
  - Investment Date (Date)
  - Company Website (Link)
  - Featured Image (Image)
- [ ] CMS collection is hidden until George adds companies
- [ ] Test adding a dummy portfolio company to verify layout works

---

## 🔒 Security

### SSL Certificate
- [ ] HTTPS is enabled
- [ ] SSL certificate is valid
- [ ] No mixed content warnings (all resources loaded via HTTPS)

### Forms
- [ ] Contact form has basic spam protection
- [ ] No sensitive data is transmitted insecurely
- [ ] Privacy Policy link is visible on form

---

## 📱 Pre-Launch Actions

### Client Review
- [ ] George has reviewed and approved all pages
- [ ] All requested changes from George have been implemented
- [ ] Client is satisfied with overall design and content

### Email Setup
- [ ] investors@siliconcenturycapital.com is set up
- [ ] deals@siliconcenturycapital.com is set up
- [ ] privacy@siliconcenturycapital.com is set up (optional)
- [ ] legal@siliconcenturycapital.com is set up (optional)
- [ ] contact@siliconcenturycapital.com is set up
- [ ] All email addresses are tested and working

### Domain & Hosting
- [ ] Domain is registered (siliconcenturycapital.com)
- [ ] DNS is properly configured
- [ ] Domain is connected to Webflow
- [ ] www and non-www versions both work
- [ ] Email is set up with domain registrar or email provider

### Analytics & Tracking
- [ ] Google Analytics is set up (if applicable)
- [ ] Google Search Console is set up
- [ ] Conversion tracking is set up (form submissions)

---

## 🎯 Final Checks Before Launch

- [ ] All items on this checklist are completed
- [ ] Client has given final approval
- [ ] Backup of entire site is created
- [ ] Launch date is confirmed with client
- [ ] Plan for post-launch monitoring (analytics, errors, etc.)

---

## 🚨 Post-Launch Monitoring (First 48 Hours)

- [ ] Check Google Analytics for traffic
- [ ] Check for 404 errors or broken links
- [ ] Monitor form submissions (are they working?)
- [ ] Check mobile performance
- [ ] Monitor page load speeds
- [ ] Check for any user-reported issues

---

**Prepared by:** Chris
**Date:** November 10, 2025
**Launch Target:** November 17, 2025 (End of Week 3)
