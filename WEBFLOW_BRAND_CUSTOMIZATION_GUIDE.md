# Silicon Century Capital - Webflow Brand Customization Guide

**Template**: Foresight (Landing Page 1 selected as Homepage)
**Date**: November 2025
**Status**: In Progress

---

## 🎨 BRAND IDENTITY REFERENCE

### Color Palette:
- **Deep Navy**: `#294c89` - Primary (backgrounds, headers, text)
- **Teal**: `#17b890` - Accent (CTAs, links, hover states)
- **Light Gray**: `#dee5e5` - Backgrounds (alternating sections)
- **Dark Green**: `#082d0f` - Secondary accent (use sparingly)
- **White**: `#FFFFFF` - Text on dark backgrounds, clean sections
- **Dark Text**: `#1a1a1a` or `#2d2d2d` - Body text on light backgrounds

### Typography:
- **Headers (H1-H6)**: **Quixote** (or similar serif - Playfair Display, Lora as fallback)
- **Body Text**: **Nanum Gothic** (Google Font)
- **Weight Hierarchy**:
  - H1: 700 (Bold), 48-64px
  - H2: 700 (Bold), 36-48px
  - H3: 600 (Semibold), 28-36px
  - H4: 600 (Semibold), 24-28px
  - Body: 400 (Regular), 16-18px
  - Small/Caption: 400 (Regular), 14px

### Design Principles:
- **Aesthetic**: "Institutional Industrial" - calm, credible, precise
- **Animation**: Minimal (subtle hover states, smooth scrolling)
- **Spacing**: Generous whitespace
- **Tone**: Professional, modern, NOT flashy

---

## 📋 WEBFLOW CUSTOMIZATION CHECKLIST

### Phase 1: Global Styles (Do This First)
- [ ] Color swatches
- [ ] Typography system
- [ ] Button styles
- [ ] Link styles
- [ ] Form field styles

### Phase 2: Layout & Structure
- [ ] Navigation bar
- [ ] Footer
- [ ] Section backgrounds
- [ ] Container widths
- [ ] Spacing system

### Phase 3: Homepage Customization
- [ ] Hero section
- [ ] Company introduction
- [ ] Four sectors section
- [ ] Experience section
- [ ] Commitment section
- [ ] Final CTA

### Phase 4: Additional Pages
- [ ] About page
- [ ] Investment Focus page
- [ ] Team page
- [ ] Contact page
- [ ] Etc.

---

## 🎯 PHASE 1: GLOBAL STYLES

### Step 1: Set Up Color Swatches

**In Webflow Designer:**

1. **Open Style Panel** → Click on any element → Style tab (paintbrush icon)
2. **Go to Project Settings** → Designer → Color Swatches
3. **Add New Swatches**:

   - **Name**: "SCC Navy" | **Hex**: `#294c89`
   - **Name**: "SCC Teal" | **Hex**: `#17b890`
   - **Name**: "SCC Light Gray" | **Hex**: `#dee5e5`
   - **Name**: "SCC Dark Green" | **Hex**: `#082d0f`
   - **Name**: "SCC White" | **Hex**: `#FFFFFF`
   - **Name**: "SCC Dark Text" | **Hex**: `#2d2d2d`

**Why This Matters**: Color swatches make it easy to update colors globally later and ensure consistency.

---

### Step 2: Update Typography System

**Font Setup:**

#### Option A: Quixote is Available (Check Adobe Fonts or similar)
1. **Add Custom Font**:
   - Project Settings → Fonts → Add Custom Font
   - Upload Quixote font files (.woff, .woff2) if you have them
   - Or use Adobe Fonts integration if available

#### Option B: Quixote Not Available (Use Elegant Serif Fallback)
1. **Use Google Fonts Alternative**:
   - **Playfair Display** (very close to Quixote - elegant, institutional)
   - **Lora** (secondary option)
   - **Cormorant Garamond** (more modern serif)

**Recommendation**: Start with **Playfair Display** as Quixote substitute

2. **Add Nanum Gothic** (Google Font):
   - Project Settings → Fonts → Google Fonts
   - Search "Nanum Gothic"
   - Add weights: 400 (Regular), 600 (Semibold), 700 (Bold)

#### Update Typography Classes:

**In Webflow Designer:**

1. **All Headings** → Style Panel → Typography
   - Font Family: **Playfair Display** (or Quixote if uploaded)
   - Weight: 700 (Bold) for H1-H2, 600 (Semibold) for H3-H4

2. **All Paragraphs** → Style Panel → Typography
   - Font Family: **Nanum Gothic**
   - Weight: 400 (Regular)
   - Size: 18px (desktop), 16px (mobile)
   - Line Height: 1.6-1.8 (generous for readability)
   - Color: `#2d2d2d` (SCC Dark Text)

3. **All Body (Default)** → Style Panel → Typography
   - Font Family: **Nanum Gothic**
   - Weight: 400
   - Color: `#2d2d2d`

**Specific Typography Styles to Update:**

Navigate to: **Style Panel → Typography tab** (Click the "All" dropdown)

Update these classes:

- **H1 Heading**:
  - Font: Playfair Display, 700
  - Size: 56px (desktop) → 40px (tablet) → 32px (mobile)
  - Line Height: 1.2
  - Color: `#294c89` (SCC Navy) for dark sections, `#FFFFFF` for light sections

- **H2 Heading**:
  - Font: Playfair Display, 700
  - Size: 44px (desktop) → 36px (tablet) → 28px (mobile)
  - Line Height: 1.3
  - Color: `#294c89` or `#FFFFFF`

- **H3 Heading**:
  - Font: Playfair Display, 600
  - Size: 32px (desktop) → 28px (tablet) → 24px (mobile)
  - Line Height: 1.4
  - Color: `#294c89` or `#FFFFFF`

- **Paragraph**:
  - Font: Nanum Gothic, 400
  - Size: 18px (desktop) → 16px (mobile)
  - Line Height: 1.7
  - Color: `#2d2d2d` (on light backgrounds) or `#FFFFFF` (on dark backgrounds)

---

### Step 3: Update Button Styles

**Primary Button (Main CTAs):**

1. Select any primary button in the template
2. **Style Panel** → Look for button class (e.g., `.button-primary`, `.btn`, etc.)
3. Update styles:

   **Background**: `#17b890` (SCC Teal)
   **Text Color**: `#FFFFFF` (White)
   **Border**: None (or 2px solid `#17b890` if you want border)
   **Border Radius**: 4px (subtle) or 8px (more rounded) - George wants not flashy, so keep subtle
   **Padding**: 16px 32px (comfortable click area)
   **Font**: Nanum Gothic, 600 (Semibold), 16px
   **Letter Spacing**: 0.5px (slightly spaced for clarity)
   **Text Transform**: None (keep as-is, or Uppercase if template uses it)

4. **Hover State**:
   - Background: Darker Teal `#149c7d` (slightly darker than #17b890)
   - OR: `#294c89` (SCC Navy) - creates nice color transition
   - Transition: All 300ms ease (smooth)
   - Transform: translateY(-2px) (subtle lift - optional, minimal)
   - Box Shadow: 0 4px 12px rgba(23, 184, 144, 0.3) (subtle glow - optional)

**Secondary Button (Outline/Ghost):**

1. Select secondary button
2. Update styles:

   **Background**: Transparent
   **Text Color**: `#294c89` (SCC Navy) on light backgrounds, `#FFFFFF` on dark
   **Border**: 2px solid `#294c89` (or `#FFFFFF` on dark backgrounds)
   **Border Radius**: 4px
   **Padding**: 16px 32px
   **Font**: Nanum Gothic, 600, 16px

3. **Hover State**:
   - Background: `#294c89` (SCC Navy)
   - Text Color: `#FFFFFF`
   - Border: 2px solid `#294c89`
   - Transition: All 300ms ease

**Button Placement Notes** (from George's copy):
- Most sections have **two CTAs** side-by-side
- Primary CTA = Teal solid button
- Secondary CTA = Navy outline button

---

### Step 4: Update Link Styles

**Body Links (in paragraph text):**

1. **Default State**:
   - Color: `#17b890` (SCC Teal)
   - Text Decoration: Underline (subtle, 1px)
   - Font Weight: 600 (Semibold)

2. **Hover State**:
   - Color: `#294c89` (SCC Navy)
   - Text Decoration: Underline
   - Transition: Color 200ms ease

**Navigation Links:**

1. **Default State**:
   - Color: `#294c89` (SCC Navy) on light nav, `#FFFFFF` on dark nav
   - Font: Nanum Gothic, 600, 16px
   - Text Decoration: None

2. **Hover State**:
   - Color: `#17b890` (SCC Teal)
   - OR: Underline with teal color
   - Transition: Color 200ms ease

3. **Active/Current Page**:
   - Color: `#17b890` (SCC Teal)
   - OR: Border-bottom 2px solid `#17b890`

---

### Step 5: Update Form Field Styles

**Input Fields (text, email, etc.):**

1. **Default State**:
   - Background: `#FFFFFF` (White)
   - Border: 2px solid `#dee5e5` (SCC Light Gray)
   - Border Radius: 4px
   - Padding: 14px 16px
   - Font: Nanum Gothic, 400, 16px
   - Color: `#2d2d2d` (SCC Dark Text)
   - Placeholder Color: `#999999` (gray, subtle)

2. **Focus State**:
   - Border: 2px solid `#17b890` (SCC Teal)
   - Box Shadow: 0 0 0 3px rgba(23, 184, 144, 0.1) (subtle glow)
   - Outline: None (remove browser default)

3. **Error State** (if needed):
   - Border: 2px solid `#e74c3c` (red)
   - Background: `#fef5f5` (light red tint)

**Textarea:**
- Same styles as input fields
- Min-height: 120px

**Select Dropdown:**
- Same styles as input fields
- Add dropdown arrow icon (teal color)

**Form Labels:**
- Font: Nanum Gothic, 600, 14px
- Color: `#2d2d2d`
- Margin-bottom: 8px

**Form Submit Button:**
- Use Primary Button style (Teal background)

---

## 🏗️ PHASE 2: LAYOUT & STRUCTURE

### Step 6: Update Navigation Bar

**Current Foresight Nav** (Landing Page 1 has minimal nav)

**Navigation Structure** (from George's copy):
- Logo (left)
- Links (center or right):
  - Home
  - About
  - Investment Focus
  - Team
  - Partners
  - Insights
  - Portfolio
  - Contact
  - **Investor Login** (button style, right-aligned)

**Styling:**

1. **Nav Container**:
   - Background: `#FFFFFF` (white) - clean, professional
   - OR: `#dee5e5` (Light Gray) - subtle
   - Border-bottom: 1px solid `#dee5e5` (subtle separation)
   - Padding: 20px 0 (vertical)
   - Position: Fixed top (sticky navigation)
   - Z-index: 1000

2. **Logo**:
   - Update with SCC logo (when George sends brand assets)
   - For now: Text logo "Silicon Century Capital" in Playfair Display, 700, 22px, color `#294c89`

3. **Nav Links**:
   - Font: Nanum Gothic, 600, 16px
   - Color: `#294c89` (Navy)
   - Spacing: 32px between links
   - Hover: Color changes to `#17b890` (Teal)

4. **"Investor Login" Button**:
   - Style as Secondary Button (Navy outline)
   - OR: Primary Button (Teal solid) if you want it to stand out
   - Position: Right-aligned

**Mobile Navigation:**
- Hamburger menu icon: `#294c89` (Navy)
- Mobile menu background: `#FFFFFF` or `#294c89`
- Links stack vertically, same hover states

---

### Step 7: Update Footer

**Footer Structure** (standard for institutional sites):

**3 or 4 Columns:**

1. **Column 1: About**
   - Logo + tagline: "Private Investment for the New Industrial Core"
   - Brief 1-2 sentence description

2. **Column 2: Quick Links**
   - About
   - Investment Focus
   - Team
   - Contact

3. **Column 3: Resources**
   - Insights
   - Portfolio
   - Careers
   - Investor Login

4. **Column 4: Contact**
   - Office: Dallas–Fort Worth Metroplex, Texas
   - Email: ContactUs@siliconcenturycapital.com
   - LinkedIn icon (if desired)

**Bottom Footer:**
- Copyright: © 2025 Silicon Century Capital. All rights reserved.
- Links: Privacy Policy | Terms of Use | Legal

**Styling:**

1. **Footer Background**: `#294c89` (SCC Navy) - strong, institutional
2. **Text Color**: `#FFFFFF` (White)
3. **Links Color**: `#FFFFFF`, hover to `#17b890` (Teal)
4. **Padding**: 60px 0 (generous vertical spacing)
5. **Border-top**: None (or 4px solid `#17b890` for accent - subtle)
6. **Font**: Nanum Gothic, 400, 14px

**Bottom Bar:**
- Background: `#1f3a6b` (slightly darker navy)
- Text: `#FFFFFF`, 14px
- Padding: 20px 0

---

### Step 8: Section Background Colors

**Alternating Pattern** (creates visual rhythm):

Landing Page 1 structure typically has multiple sections. Alternate backgrounds:

**Pattern**:
1. **Hero**: `#294c89` (Navy) with video overlay OR high-quality image
2. **Section 1 (Intro)**: `#FFFFFF` (White)
3. **Section 2 (Four Sectors)**: `#dee5e5` (Light Gray)
4. **Section 3 (Experience)**: `#FFFFFF` (White)
5. **Section 4 (Network)**: `#dee5e5` (Light Gray)
6. **Section 5 (Commitment)**: `#FFFFFF` (White)
7. **Final CTA**: `#294c89` (Navy) OR `#17b890` (Teal - for impact)

**Implementation**:
- Select each section wrapper
- Update background color using color swatches
- Adjust text colors accordingly (dark text on light backgrounds, white text on dark backgrounds)

---

### Step 9: Container Widths & Spacing

**Max-Width for Content:**
- **Standard Container**: 1200px (comfortable reading width)
- **Narrow Container** (for text-heavy sections like About): 900px
- **Wide Container** (for grids/galleries): 1400px

**Vertical Spacing (Section Padding):**
- **Large sections**: 100px top/bottom (desktop) → 60px (tablet) → 40px (mobile)
- **Medium sections**: 80px top/bottom (desktop) → 50px (tablet) → 30px (mobile)
- **Small sections**: 60px top/bottom (desktop) → 40px (tablet) → 24px (mobile)

**Horizontal Padding:**
- Container: 40px left/right (desktop) → 24px (tablet) → 16px (mobile)

**Element Spacing:**
- Heading → Paragraph: 24px margin-bottom
- Paragraph → Paragraph: 16px margin-bottom
- Section Heading → Body: 40px margin-bottom
- CTA Buttons: 16px gap between them (if side-by-side)

---

## 🏠 PHASE 3: HOMEPAGE CUSTOMIZATION (Landing Page 1)

### Step 10: Hero Section

**Current Foresight Hero** (Landing Page 1 has clean, minimal hero)

**What George Wants**:
- **Headline**: "Private Investment for the New Industrial Core"
- **Subheadline**: "We invest in proven and emerging industrial technologies — semiconductors, robotics, AI, and advanced manufacturing platforms — that strengthen performance, resilience, and global competitiveness."
- **Two CTAs**: "Learn More About Our Strategy" + "Connect With Us"
- **Background**: Video (semiconductors/robotics) OR high-quality industrial image

**Customization Steps**:

1. **Background**:
   - If using video: Add video element, set to autoplay, loop, muted
   - Overlay: Dark overlay (Navy `#294c89` at 70% opacity) to ensure text readability
   - If using image: High-resolution semiconductor/robotics image, same overlay

2. **Headline**:
   - Text: "Private Investment for the New Industrial Core"
   - Font: Playfair Display, 700, 56px (desktop) → 40px (tablet) → 32px (mobile)
   - Color: `#FFFFFF` (White)
   - Line Height: 1.2
   - Max-width: 800px (centered)
   - Margin-bottom: 24px

3. **Subheadline**:
   - Text: George's copy (see above)
   - Font: Nanum Gothic, 400, 20px (desktop) → 18px (mobile)
   - Color: `#FFFFFF` (White) or `#dee5e5` (Light Gray - slightly muted)
   - Line Height: 1.6
   - Max-width: 700px (centered)
   - Margin-bottom: 40px

4. **CTA Buttons** (side-by-side):
   - **Button 1**: "Learn More About Our Strategy" (Primary - Teal)
   - **Button 2**: "Connect With Us" (Secondary - White outline)
   - Gap: 16px between buttons
   - Mobile: Stack vertically, full-width

5. **Hero Height**:
   - Min-height: 80vh (80% of viewport height)
   - Flexbox: Center content vertically and horizontally
   - Padding: 120px 0 (to account for fixed navigation)

6. **Animation** (subtle):
   - Headline: Fade in from bottom, 0.8s delay
   - Subheadline: Fade in from bottom, 1.0s delay
   - Buttons: Fade in from bottom, 1.2s delay
   - Keep animations subtle (George wants minimal animation)

**Optional: Scrolling Indicator**:
- Small downward arrow at bottom of hero
- Color: `#FFFFFF` or `#17b890`
- Animation: Subtle bounce
- Links to next section (smooth scroll)

---

### Step 11: Company Introduction Section

**Content** (from George's copy):
- **Headline**: "Advancing the Engines of Industrial Innovation"
- **Body**: "Silicon Century Capital is a U.S.-based independent sponsor investing across the semiconductor and advanced manufacturing value chain..."

**Layout**:
- Background: `#FFFFFF` (White)
- Max-width: 900px (narrow for readability)
- Text-align: Center (or left, depending on preference)
- Padding: 100px 0

**Styling**:
1. **Headline**:
   - Font: Playfair Display, 700, 44px
   - Color: `#294c89` (Navy)
   - Margin-bottom: 32px

2. **Body Paragraphs**:
   - Font: Nanum Gothic, 400, 18px
   - Color: `#2d2d2d` (Dark Text)
   - Line Height: 1.7
   - Margin-bottom: 16px between paragraphs

3. **Key Phrases** (bold in copy):
   - "semiconductors, robotics, AI, and intelligent manufacturing systems" → Bold (700)
   - "unlock value through corporate carve-outs and strategic partnerships" → Bold

**Optional Visual**:
- Background image or subtle pattern (faded semiconductor diagram, abstract industrial lines)
- Opacity: 3-5% (very subtle, doesn't interfere with readability)

---

### Step 12: Four Sectors Section

**Content** (from George's copy):
- **Headline**: "Investing Across the Connected Industrial Ecosystem"
- **Intro**: "We invest in four interconnected sectors..."
- **Four Cards**:
  1. Semiconductors
  2. Advanced Manufacturing
  3. Robotics & Automation
  4. AI & Intelligent Systems
- **Each card has**: Title, description, hover insight

**Layout**:
- Background: `#dee5e5` (Light Gray)
- Padding: 100px 0
- Grid: 2x2 (desktop) → 1x4 (mobile)
- Gap: 32px between cards

**Card Styling**:
1. **Card Container**:
   - Background: `#FFFFFF` (White)
   - Border: None OR 1px solid `#dee5e5` (subtle)
   - Border Radius: 8px (subtle rounded corners)
   - Padding: 40px
   - Box Shadow: 0 2px 8px rgba(0,0,0,0.06) (very subtle)
   - Transition: All 300ms ease

2. **Card Hover State**:
   - Transform: translateY(-4px) (subtle lift)
   - Box Shadow: 0 8px 24px rgba(41, 76, 137, 0.12) (navy-tinted shadow)
   - Border: 2px solid `#17b890` (Teal accent - optional)

3. **Icon/Visual** (top of card):
   - Option A: Icon (semiconductor chip, gear, robot arm, brain/AI)
   - Option B: Small image (128x128px)
   - Color: `#17b890` (Teal) for icons
   - Size: 48px x 48px
   - Margin-bottom: 24px

4. **Card Title**:
   - Font: Playfair Display, 700, 24px
   - Color: `#294c89` (Navy)
   - Margin-bottom: 16px

5. **Card Description**:
   - Font: Nanum Gothic, 400, 16px
   - Color: `#2d2d2d`
   - Line Height: 1.6
   - Margin-bottom: 16px

6. **Hover Insight** (appears on hover):
   - Background: `#17b890` (Teal) - OR overlay on card
   - Text Color: `#FFFFFF`
   - Font: Nanum Gothic, 600, 14px
   - Padding: 12px 16px
   - Border-radius: 4px
   - Position: Absolute bottom of card OR tooltip
   - Transition: Opacity 300ms ease

**Implementation Note**:
- Hover insights can be:
  - **Option A**: Tooltip that appears on hover (cleaner)
  - **Option B**: Entire card flips to show insight on back (more flashy - avoid)
  - **Option C**: Small panel slides up from bottom of card (moderate)
- Recommend **Option A** (tooltip) or **Option C** (slide up panel) to maintain "not flashy" aesthetic

---

### Step 13: Experience Section

**Content** (from George's copy):
- **Headline**: "Experience, Insight, and Industrial Depth"
- **Body**: Team capabilities, carve-out expertise, partnerships

**Layout**:
- Background: `#FFFFFF` (White)
- Max-width: 1000px
- Two-column layout (desktop) → Single column (mobile)
- Padding: 100px 0

**Styling**:

**Option A: Text + Image Layout**
- Left: Text content (60% width)
- Right: Image or abstract visual (40% width)

**Option B: Full-width Text with Background Image**
- Text overlaid on faded industrial background image
- Dark overlay for readability

**Text Styling**:
1. **Headline**:
   - Font: Playfair Display, 700, 44px
   - Color: `#294c89`
   - Margin-bottom: 32px

2. **Body Paragraphs**:
   - Font: Nanum Gothic, 400, 18px
   - Color: `#2d2d2d`
   - Line Height: 1.7

3. **Key Phrases** (bold):
   - "family offices, corporates, institutional investors, and sovereign wealth funds"
   - "code as on capital"

**Optional Enhancements**:
- Pull quote: "Industrial performance today depends as much on code as on capital"
  - Font: Playfair Display, 600, 28px
  - Color: `#17b890` (Teal)
  - Border-left: 4px solid `#17b890`
  - Padding-left: 24px
  - Margin: 40px 0

---

### Step 14: Trusted Network Section

**Content**:
- **Headline**: "Trusted Experience Across the Global Industrial Ecosystem"
- **Body**: Network of executives, engineers, investors

**Layout**:
- Background: `#dee5e5` (Light Gray)
- Padding: 100px 0

**Special Element**: **Semiconductor Company Logos Banner**

George mentioned scrolling logos of semiconductor companies for credibility.

**Logo Banner Implementation**:

1. **Container**:
   - Background: `#FFFFFF` (White section within Light Gray background)
   - Padding: 60px 0
   - Border-top: 1px solid `#dee5e5`
   - Border-bottom: 1px solid `#dee5e5`

2. **Layout**:
   - **Option A**: Static grid (4-6 logos, fixed)
   - **Option B**: Scrolling marquee (8-12 logos, infinite scroll)

3. **Logo Styling**:
   - Grayscale filter (makes logos look more cohesive)
   - Opacity: 60%
   - Hover: Remove grayscale, opacity 100%
   - Max-height: 60px (consistent sizing)
   - Padding: 0 40px (spacing between logos)

4. **Animation** (if scrolling):
   - Smooth horizontal scroll
   - Speed: Slow (30-40 seconds for full loop)
   - Seamless loop

**Text Content** (above or below logos):
- Headline: "Trusted Experience Across the Global Industrial Ecosystem"
- Font: Playfair Display, 600, 36px
- Color: `#294c89`
- Text-align: Center
- Margin-bottom: 48px

---

### Step 15: Commitment Beyond Capital Section

**Content** (from George's copy):
- **Headline**: "Commitment Beyond Capital"
- **Body**: "A portion of Silicon Century Capital's profits support organizations..."
- **Two Foundations**:
  1. Tunnel to Towers Foundation
  2. mikeroweWORKS Foundation
- **Values**: "discipline, purpose, and a belief in the value of building things that last"

**Layout**:
- Background: `#FFFFFF` (White)
- Max-width: 900px
- Text-align: Center
- Padding: 100px 0

**Styling**:

1. **Headline**:
   - Font: Playfair Display, 700, 44px
   - Color: `#294c89`
   - Margin-bottom: 24px

2. **Intro Paragraph**:
   - Font: Nanum Gothic, 400, 18px
   - Color: `#2d2d2d`
   - Margin-bottom: 40px

3. **Foundation Logos + Descriptions**:
   - Layout: Two columns (desktop) → Stack (mobile)
   - Each foundation:
     - Logo (centered, max-width 200px)
     - Name (Nanum Gothic, 700, 18px, `#294c89`)
     - Description (Nanum Gothic, 400, 16px, `#2d2d2d`)
   - Spacing: 32px gap between foundations

4. **Closing Statement**:
   - Font: Playfair Display, 600, 20px (slightly larger, italicized)
   - Color: `#294c89`
   - Margin-top: 40px
   - Text: "These causes reflect the same principles that guide our work — discipline, purpose, and a belief in the value of building things that last."

**Optional Visual**:
- Subtle icon or graphic representing service/craftsmanship (American flag, hard hat, etc.)
- Keep minimal and tasteful

---

### Step 16: Final CTA Section

**Content**:
- **Headline**: "Ready to Build the Next Century of Industry?"
- **Body**: "We welcome conversations with investors, management teams, and partners..."
- **Two CTAs**: "Connect With Us" + "Learn More About Our Strategy"

**Layout**:
- Background: `#294c89` (Navy) OR `#17b890` (Teal - for impact)
- Full-width section
- Padding: 80px 0
- Text-align: Center

**Styling**:

1. **Headline**:
   - Font: Playfair Display, 700, 48px
   - Color: `#FFFFFF`
   - Margin-bottom: 24px

2. **Body**:
   - Font: Nanum Gothic, 400, 18px
   - Color: `#FFFFFF` or `#dee5e5` (slightly muted)
   - Max-width: 700px (centered)
   - Margin-bottom: 40px

3. **CTA Buttons**:
   - If Navy background:
     - Button 1: Teal solid (`#17b890`)
     - Button 2: White outline
   - If Teal background:
     - Button 1: White solid (`#FFFFFF`, text `#17b890`)
     - Button 2: White outline
   - Layout: Side-by-side (desktop) → Stacked (mobile)

---

## ✅ QUICK WINS (Do These First for Maximum Impact)

### Priority 1: Colors
1. Update section backgrounds (alternating White → Light Gray → White)
2. Update hero background to Navy with video/image
3. Update footer background to Navy

### Priority 2: Typography
1. Change all headings to Playfair Display (or Quixote)
2. Change all body text to Nanum Gothic
3. Update heading colors to Navy (`#294c89`)

### Priority 3: Buttons
1. Primary button: Teal background (`#17b890`)
2. Secondary button: Navy outline (`#294c89`)
3. Add hover states

### Priority 4: Navigation
1. Update nav links to Navy color
2. Add "Investor Login" button (right-aligned)
3. Make navigation sticky (fixed position)

**After these 4, the site will already feel like Silicon Century Capital's brand!**

---

## 📱 RESPONSIVE DESIGN CHECKLIST

### Mobile (< 768px):
- [ ] Navigation: Hamburger menu working
- [ ] Hero: Headline readable (32px), buttons stack vertically
- [ ] Four sectors: Cards stack vertically (1 column)
- [ ] All text: Readable sizes (16px minimum)
- [ ] Buttons: Full-width or comfortable tap targets (44px height minimum)
- [ ] Images: Scale properly, don't overflow
- [ ] Forms: Input fields full-width, comfortable spacing

### Tablet (768px - 1024px):
- [ ] Four sectors: 2x2 grid OR 1x4 column (depending on preference)
- [ ] Typography: Slightly smaller than desktop but still readable
- [ ] Spacing: Reduce section padding (60px vs 100px)
- [ ] Navigation: May still be full horizontal nav or switch to hamburger

### Desktop (> 1024px):
- [ ] All content within max-width containers (1200px)
- [ ] Comfortable spacing and whitespace
- [ ] Hover states working on buttons, cards, links
- [ ] Two-column layouts displaying properly

**Test Breakpoints in Webflow**:
- Base (desktop): 1440px+
- Tablet: 991px
- Mobile Landscape: 767px
- Mobile Portrait: 479px

---

## 🎬 ANIMATION GUIDELINES (Keep Minimal)

George specifically requested: **"Minimal animation, maintain gravitas"**

**Allowed Animations**:
1. **Button hovers**: Color change, subtle lift (2-4px), smooth transition (300ms)
2. **Card hovers**: Subtle lift (4-8px), shadow increase, border accent
3. **Link hovers**: Color change (200ms)
4. **Scroll animations**: Fade in from bottom (subtle, 0.8s), only on first viewport
5. **Page transitions**: Smooth scroll between sections

**Avoid**:
- ❌ Flashy parallax effects
- ❌ Bounce animations
- ❌ Spinning/rotating elements
- ❌ Excessive fade/slide combinations
- ❌ Animated backgrounds (beyond subtle video)

**Easing Functions**:
- Use `ease`, `ease-out`, or `ease-in-out`
- Avoid `cubic-bezier` with dramatic curves

---

## 🚀 NEXT STEPS AFTER BRAND CUSTOMIZATION

Once brand is applied to Landing Page 1 (Homepage):

1. **Duplicate structure for other pages**:
   - About/Strategy
   - Investment Focus
   - Team
   - Partners
   - Contact
   - Etc.

2. **Set up CMS collections**:
   - Team members
   - Portfolio companies
   - Blog posts (Insights)
   - Advisory board

3. **Implement forms**:
   - Contact form (dual version)
   - Investor access request form
   - Newsletter signup

4. **Add content from George's PDF**:
   - Copy/paste all copy
   - Replace placeholder text
   - Adjust layouts as needed

5. **Source and add imagery**:
   - Hero video
   - Stock photos
   - Icons
   - Foundation logos
   - Semiconductor company logos

6. **Test everything**:
   - Forms submit correctly
   - Links work
   - Mobile responsive
   - Browser compatibility
   - Performance (page load speed)

---

## 📝 NOTES & TIPS

### Webflow Best Practices:

1. **Use Classes, Not IDs**:
   - Create reusable classes: `.section`, `.container`, `.heading-navy`, `.button-primary`
   - Use combo classes for variations: `.button-primary.button-large`

2. **Organize Your Classes**:
   - Prefix global styles: `.global-`, `.layout-`, `.component-`
   - Keep naming consistent and descriptive

3. **Use Symbols for Repeating Elements**:
   - Navigation bar → Symbol (appears on all pages)
   - Footer → Symbol
   - Buttons → Component (if Webflow supports it)

4. **Backup Your Work**:
   - Webflow auto-saves, but duplicate your project before major changes
   - Export code periodically (if on CMS plan)

5. **Preview Often**:
   - Click Preview button frequently to see changes in real browser
   - Test responsiveness at each breakpoint

### Common Webflow Gotchas:

- **Z-index**: Fixed navigation needs z-index 1000+ to stay above content
- **Overflow**: Hidden overflow on body can break fixed positioning
- **Max-width**: Use max-width on containers, not width: 100%
- **Line-height**: Unitless line-height (1.6) is better than px values
- **Hover states**: Only work on desktop, not touch devices (don't rely on them for critical interactions on mobile)

---

## ✅ BRAND CUSTOMIZATION CHECKLIST

### Colors:
- [ ] Color swatches created (Navy, Teal, Light Gray, Dark Green, White, Dark Text)
- [ ] Section backgrounds updated (alternating White → Light Gray)
- [ ] Hero background: Navy with video/image overlay
- [ ] Footer background: Navy
- [ ] Text colors: Navy for headings, Dark Text for body

### Typography:
- [ ] Headings: Playfair Display (or Quixote) applied
- [ ] Body text: Nanum Gothic applied
- [ ] Font sizes responsive (desktop → tablet → mobile)
- [ ] Line heights comfortable (1.6-1.8 for body)
- [ ] Font weights correct (700 for H1-H2, 600 for H3-H4, 400 for body)

### Buttons:
- [ ] Primary button: Teal background, white text
- [ ] Primary button hover: Darker teal or Navy
- [ ] Secondary button: Navy outline, transparent background
- [ ] Secondary button hover: Navy fill, white text
- [ ] Button padding comfortable (16px 32px)
- [ ] Transitions smooth (300ms)

### Navigation:
- [ ] Nav background: White or Light Gray
- [ ] Nav links: Navy color, Teal on hover
- [ ] "Investor Login" button added (right-aligned)
- [ ] Mobile: Hamburger menu working
- [ ] Position: Fixed/sticky

### Footer:
- [ ] Background: Navy
- [ ] Text: White
- [ ] Links: White, hover to Teal
- [ ] Copyright and legal links included
- [ ] 3-4 column layout (desktop) → Stack (mobile)

### Forms:
- [ ] Input fields: White background, Light Gray border, Teal focus border
- [ ] Labels: Semibold, readable
- [ ] Submit button: Primary button style (Teal)
- [ ] Placeholders: Subtle gray color

### Homepage Sections:
- [ ] Hero: Navy background, white text, two CTAs, video/image
- [ ] Company intro: White background, centered text
- [ ] Four sectors: Light Gray background, card grid with hover states
- [ ] Experience: White background, two-column or full-width
- [ ] Trusted network: Light Gray, logo banner (when logos available)
- [ ] Commitment: White background, foundation logos
- [ ] Final CTA: Navy or Teal background, white text, two CTAs

### Responsive:
- [ ] Mobile: All sections stack vertically, readable text
- [ ] Tablet: Hybrid layouts, comfortable spacing
- [ ] Desktop: Full layouts, generous whitespace

### Animations:
- [ ] Button hovers: Smooth transitions
- [ ] Card hovers: Subtle lift and shadow
- [ ] Scroll animations: Fade in (subtle, first viewport only)
- [ ] No flashy or excessive animations

---

## 🎯 ESTIMATED TIME

**Phase 1 (Global Styles)**: 2-3 hours
- Colors: 30 min
- Typography: 1 hour
- Buttons, links, forms: 1-1.5 hours

**Phase 2 (Layout & Structure)**: 2-3 hours
- Navigation: 1 hour
- Footer: 1 hour
- Section backgrounds, spacing: 1 hour

**Phase 3 (Homepage Customization)**: 4-6 hours
- Hero section: 1 hour
- Company intro: 30 min
- Four sectors: 1.5 hours
- Experience, network, commitment, final CTA: 2-3 hours

**Total**: 8-12 hours for complete brand customization of Landing Page 1 (Homepage)

---

## 📧 READY TO SHOW GEORGE?

After completing brand customization:

1. **Take screenshots** of key sections (Hero, Four Sectors, etc.)
2. **Send staging link** to George with context:
   - "Homepage 50% complete with SCC brand applied"
   - "Placeholder images for now (sourcing hero video this week)"
   - "Ready for your feedback on colors, typography, and layout"

3. **Ask specific questions**:
   - "Does the Navy + Teal color scheme feel right for 'Institutional Industrial'?"
   - "Is the typography readable and professional?"
   - "Any sections you'd like adjusted before I build out the remaining pages?"

---

*Document Created: November 2025*
*Status: Ready to implement*
*Next: Apply to Webflow staging site*
