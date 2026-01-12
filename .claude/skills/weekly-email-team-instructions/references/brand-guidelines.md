# Brand Guidelines Reference

This document consolidates The Edmund Bogen Team brand standards for use across all generated assets.

## Color Palette

### Primary Colors
- **Navy/Dark Blue:** `#1a3e5c` - Primary brand color (60% usage)
- **Bright Blue/Cyan:** `#00a8e1` - Accent color for CTAs and highlights (10-15% usage)
- **White:** `#ffffff` - Neutral, clean sections (25-30% usage)

### Secondary Colors
- **Black:** `#000000` - Text on white, dramatic headers
- **Light Gray:** `#f4f4f4` to `#e8e8e8` - Background sections

### Semantic Colors (Data Visualization)
- **Green:** `#28a745` - Positive/Strong indicators
- **Amber:** `#ffc107` - Moderate indicators
- **Red:** `#dc3545` - Warning/Weak indicators
- **Gray:** `#666666` - Neutral text

## Typography

### Font Families

**Article Pages (GitHub):**
- Primary: Montserrat (Google Fonts)
- Weights: 300 (light), 400 (regular), 500 (medium), 600 (semi-bold), 700 (bold)

**Email & Dashboard:**
- System font stack: `-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif`

### Type Hierarchy

**Headers:**
- Weight: 300 (light)
- Case: ALL CAPS with wide letter-spacing (0.05-0.15em)
- Size: 36-72px for hero headers, 24-32px for section headers
- Color: White on dark backgrounds, Black on light backgrounds

**Body Text:**
- Weight: 400 (regular)
- Size: 16-18px minimum
- Line-height: 1.6-1.8
- Color: `#333333` on white, `#ffffff` on dark

**CTAs/Buttons:**
- ALL CAPS
- Medium weight (500-600)
- Wide letter-spacing
- Examples: "READ THE FULL ANALYSIS", "VIEW PROPERTIES", "CONTACT US TODAY"

## Layout Principles

### Design Philosophy
- Institutional, data-driven aesthetic
- Investment research meets luxury real estate
- Authority > friendliness
- Precision > decoration

### Structural Elements

**Hero Sections:**
- Full-width background (image or solid color)
- Navy overlay gradient (40-60% opacity)
- Centered content with clear hierarchy
- Image above the fold

**Section Rhythm:**
- Large vertical spacing: 40-60px between sections
- Hard separators: Thick borders, horizontal rules
- Section headers with left border or bottom underline

**Cards & Containers:**
- White background
- Hard edges or subtle radius (4-8px max)
- Left border accent for classification
- Light shadow on hover only

### Specific Component Styles

**Stat Cards:**
- Label (small uppercase)
- Value (large, bold)
- Status badge or change indicator
- Border color indicates category:
  - Green → Waterfront/Positive
  - Red → New construction/Alert
  - Blue → Standard/Neutral

**Property Listing Cards:**
- Address (uppercase, bold)
- Price (large, light weight)
- Structured facts grid (Beds | Baths | SqFt | etc.)
- MLS reference
- CTA button with external link

## CTA Design

**Button Styling:**
- Uppercase text
- Letter-spacing applied
- Bold but restrained
- Rectangular or subtle radius (no pill shapes)

**Color Logic:**
- Cyan (`#00a8e1`) → Primary action
- Navy (`#1a3e5c`) → Contact/secondary action
- Green (`#28a745`) → Positive confirmation

**Hover Behavior:**
- Slight elevation (2-4px shadow)
- Darkening by 10-15%
- No animation gimmicks

## Image Standards

### Hero Images
- High contrast
- Works under dark overlays
- Editorial feel (not promotional)
- Minimum 1920px width
- Same image reused across: Email hero, Article hero, Dashboard featured article

### Property Photography
- Professional real estate photography only
- Golden hour or twilight shots preferred
- Wide-angle interiors, elevated exteriors
- Enhanced blues (pools/sky)

## Email-Specific Rules

- Max width: 600px
- Single column layout
- Inline CSS only (no external stylesheets)
- Mobile-first responsive stacking
- Clear "scan path" hierarchy:
  1. Logo
  2. Market Intelligence header
  3. Weekly article image
  4. Article summary
  5. Community link
  6. Executive summary
  7. Listings
  8. Authority bio

## Consistency Requirements

**ABSOLUTE RULES - These must be enforced:**
1. Same weekly image everywhere (email, article, dashboard)
2. Same article title everywhere
3. Same date everywhere
4. Same community counts everywhere
5. Same color semantics everywhere (blue = inventory, green = strength, red = weakness)

No deviations allowed unless explicitly instructed.

## Data Visualization (Dashboard)

**Chart Library:** Chart.js

**Chart Types Used:**
- Bar charts (vertical)
- Horizontal bar charts
- Bubble charts
- Line charts
- Doughnut charts

**Chart Styling:**
- White container backgrounds
- Understated titles
- Minimal legends
- Interactive but not novelty-driven

**Color Logic:**
- Blue → Inventory
- Green → Sales/Strength
- Red → Weakness/Decline
- Yellow/Amber → Transitional states

## Douglas Elliman Co-Branding

**Requirements:**
- Always include Douglas Elliman logo when space allows
- Maintain Douglas Elliman teal/white colors (never alter)
- Legal footer required on all assets
- Clear separation between EB and Douglas Elliman marks

**Standard Footer Text:**
```
The Edmund Bogen Team | Douglas Elliman Real Estate | (561) 235-7575
1111 LINCOLN RD, MIAMI BEACH, FL 33139. 305.695.6300

© 2018 DOUGLAS ELLIMAN REAL ESTATE. ALL MATERIAL PRESENTED HEREIN IS INTENDED FOR 
INFORMATION PURPOSES ONLY. WHILE, THIS INFORMATION IS BELIEVED TO BE CORRECT, IT IS 
REPRESENTED SUBJECT TO ERRORS, OMISSIONS, CHANGES OR WITHDRAWAL WITHOUT NOTICE. 
[Standard legal disclaimer continues...]
```

## Mobile Responsive Breakpoints

- **Desktop:** 1200px+
- **Tablet:** 768px - 1199px
- **Mobile:** < 768px

All layouts must stack vertically on mobile with appropriate padding adjustments.

## Quality Control Checklist

Before finalizing any asset:
- [ ] Colors match palette (navy #1a3e5c, bright blue #00a8e1)
- [ ] Typography is sans-serif, appropriate weights
- [ ] All-caps used ONLY for headers/CTAs with wide spacing
- [ ] Images are high-quality professional photography
- [ ] EB logo present and unaltered
- [ ] Douglas Elliman co-branding included
- [ ] Generous white space throughout
- [ ] Text readable with proper contrast (WCAG AA: 4.5:1 minimum)
- [ ] Tone is professional yet approachable
- [ ] CTAs are clear and use bright blue
- [ ] All links functional
- [ ] Mobile responsive

---

**Source:** Derived from `/mnt/skills/user/edmund-bogen-brand/SKILL.md` and Brand & Presentation System Specification document.
