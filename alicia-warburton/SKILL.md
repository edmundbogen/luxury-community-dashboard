# Alicia Warburton Newsletter Skill

This skill generates Alicia Warburton's market intelligence newsletter package:

1. **Email HTML** (Constant Contact)
2. **Article Page HTML** (GitHub Pages)

## Brand Guidelines

### Color Palette
- **Primary (Deep Blue-Slate):** `#1a2634` - Headers, navigation, authority elements
- **Accent (Warm Champagne Gold):** `#d4a574` - CTAs, highlights, labels
- **Gray:** `#6b7c8a` - Secondary text, subtle elements
- **Light Background:** `#fdfcfb` - Warm white for sections
- **Text:** `#1a1a1a` (primary), `#4a5568` (body)
- **Border:** `#e8e8e8`

### Typography
- **Headlines:** Cormorant Garamond (Google Fonts) - Light/Regular weight, elegant serif
- **Body:** Inter (Google Fonts) - Clean, professional sans-serif
- **Email fallback:** -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Arial, sans-serif

### Voice & Tone
- First-person perspective ("I'm writing this from my perspective...")
- Data-driven but accessible
- Professional yet warm
- References her background: "Having relocated from the New York area myself..."
- Appeals to sophisticated investors and relocating buyers
- No excessive enthusiasm; measured, authoritative

### Visual Style
- Clean, institutional aesthetic (investment research meets luxury real estate)
- Full-width hero images with navy gradient overlay
- Left-border accent on pull quotes (champagne gold)
- Large vertical spacing between sections
- Stat grids with clear hierarchy
- Mobile-first responsive design

## Contact Information

```
Name: Alicia Warburton
Title: Realtor®
Company: Douglas Elliman Real Estate
Address: 100 Beach Drive NE, Suite 102, St. Petersburg, FL 33701
Phone: (727) 313-7035
Email: awarburton@elliman.com
```

## Required Input for Each Newsletter

### Article Details
```
Title: [Full article title]
Date: [Month YYYY format - e.g., January 2026]
Hero Image: [filename.png or filename.jpg - must be uploaded to GitHub first]
Article Slug: [url-friendly-version - e.g., gas-plant-district]
Summary: [2-3 sentence summary for email preview]
Full Article Content: [Complete research/article text]
```

### Key Statistics (3-4 for stats bar)
```
Stat 1: [Number] | [Label]
Stat 2: [Number] | [Label]
Stat 3: [Number] | [Label]
Stat 4: [Number] | [Label]
```

### Pull Quotes (1-2 for emphasis)
```
Quote: "[Quote text]"
Attribution: [Name, Title/Organization]
```

### Call-to-Action Focus
- Primary: Contact Alicia directly (email or phone)
- Secondary: Read full analysis (article page link)

## Asset Specifications

### Email HTML (Constant Contact)

**File naming:** `email-[topic-slug].html`

**Structure:**
1. Header - Alicia Warburton branding with "St. Petersburg Market Intelligence" label
2. Hero Image - Links to full article
3. Article Title Section - Label, headline, summary
4. Key Stats Grid - 3 statistics with left-border accent
5. Quick Insights Box - 4-5 bullet points on dark background
6. Read Full Analysis CTA - Champagne gold button
7. "From My Perspective" Section - Personal commentary (2-3 paragraphs)
8. Contact CTA Box - "Let's Discuss Your Strategy" with contact button
9. About Section - Brief bio on dark background
10. Footer - Address, contact, legal disclaimer

**Technical Requirements:**
- Inline CSS only (no external stylesheets)
- Max width: 600px
- Single column layout
- Mobile-responsive (stacks naturally)
- All images: absolute URLs (edmundbogen.github.io/luxury-community-dashboard/alicia-warburton/)

### Article Page HTML (GitHub Pages)

**File naming:** `[topic-slug].html`

**Structure:**
1. Fixed Navigation - Name, company, phone, contact link
2. Hero Section - Full-width image with gradient overlay, title, date, author
3. Stats Bar - 4 key metrics on dark background
4. Article Content:
   - Intro paragraph (larger text, bordered bottom)
   - H2 sections with body text
   - Pull quotes (left gold border, italic serif)
   - Data tables (dark header, alternating rows)
   - Comparison grids (2-column cards)
   - Callout boxes (labeled insight boxes)
   - Timeline (vertical with gold dots)
5. "My Perspective" Section - Personal analysis
6. Author Section - Dark background with bio and CTA
7. Footer - Company info and legal

**Technical Requirements:**
- Google Fonts: Cormorant Garamond, Inter
- Responsive breakpoints: 768px, 480px
- Mobile-friendly navigation
- Smooth reading experience on iPhone and desktop

## Deployment

### GitHub Pages
1. Upload hero image to `/alicia-warburton/` folder
2. Upload article HTML to `/alicia-warburton/` folder
3. Push to GitHub: `git add . && git commit -m "Add [topic] newsletter" && git push`
4. Live URL: `https://edmundbogen.github.io/luxury-community-dashboard/alicia-warburton/[article-slug].html`

### Constant Contact
1. Copy email HTML content
2. Create new email campaign in Constant Contact
3. Use "Code View" to paste HTML
4. Test in preview mode
5. Schedule or send

## Example Newsletter Topics for Alicia

Given her market focus (St. Petersburg luxury, investor audience, Northeast relocators), ideal topics include:

- **Development Analysis:** Major projects affecting property values (Gas Plant, 400 Central, Waldorf Astoria)
- **Market Intelligence:** Quarterly luxury market updates, migration trends, inventory analysis
- **Neighborhood Deep Dives:** Historic Old Northeast, Snell Isle, Tierra Verde, Venetian Isles
- **Investment Thesis:** Why St. Petersburg for portfolio allocation, rental yields, appreciation forecasts
- **Policy Impact:** Zoning changes, insurance market, tax implications for investors

## Validation Checklist

Before generating assets, verify:

- [ ] Article title matches in email and article page
- [ ] Date is consistent across all assets
- [ ] Hero image exists at specified path (or will be uploaded)
- [ ] All stats have values (no placeholders)
- [ ] Pull quotes have proper attribution
- [ ] Contact information is current
- [ ] Links point to correct destinations
- [ ] Colors match brand palette
- [ ] Mobile responsiveness tested

## Quick Start

**"I need to create a newsletter about [TOPIC]."**

1. Provide: Title, date, summary, full research/article content, hero image filename, 3-4 key stats
2. Claude validates and asks clarifying questions
3. Claude generates email HTML and article page HTML
4. Upload hero image to GitHub folder
5. Push HTML files to GitHub
6. Copy email HTML to Constant Contact
7. Send/schedule

---

## Brand Assets Location

```
/Users/edmundbogen/Desktop/luxury-community-dashboard/alicia-warburton/
├── SKILL.md (this file)
├── gas-plant-hero.png (hero images)
├── gas-plant-district.html (article pages)
├── email-gas-plant.html (email HTML)
└── [future newsletters...]
```

## Future Enhancements (Optional)

- Add Alicia's professional headshot for author section
- Create listings page template for featured properties
- Add social sharing meta tags to article pages
- Create dashboard showing all published articles
