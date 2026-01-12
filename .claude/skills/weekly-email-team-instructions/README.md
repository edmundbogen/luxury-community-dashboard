# Weekly Email Team Instructions - Installation & Usage Guide

## Overview

This skill generates The Edmund Bogen Team's complete weekly market intelligence package:
- Email HTML (Constant Contact)
- Article Page HTML (GitHub Pages)
- Dashboard HTML (GitHub Pages)
- Community Listings Pages HTML (GitHub Pages)

**Designed for:** Edmund, Nicole, Dina, Samantha

## Installation

### Option 1: Install via Terminal (Recommended)

1. **Download the skill zip file** to your computer

2. **Open Terminal** (Mac/Linux) or Command Prompt (Windows)

3. **Navigate to your downloads folder:**
   ```bash
   cd ~/Downloads
   ```

4. **Unzip the skill:**
   ```bash
   unzip weekly-email-team-instructions.zip
   ```

5. **Move to Claude skills directory:**
   
   **On Mac/Linux:**
   ```bash
   mv weekly-email-team-instructions ~/.claude/skills/
   ```
   
   **On Windows:**
   ```bash
   move weekly-email-team-instructions %USERPROFILE%\.claude\skills\
   ```

6. **Verify installation:**
   ```bash
   ls ~/.claude/skills/weekly-email-team-instructions
   ```
   
   You should see:
   - SKILL.md
   - team-workflow-template.md
   - references/ (folder)
   - README.md

7. **Restart Claude** if it's currently running

### Option 2: Manual Installation

1. Download and unzip the skill folder
2. Manually copy `weekly-email-team-instructions/` folder to:
   - **Mac:** `/Users/[YOUR_USERNAME]/.claude/skills/`
   - **Windows:** `C:\Users\[YOUR_USERNAME]\.claude\skills\`
   - **Linux:** `/home/[YOUR_USERNAME]/.claude/skills/`
3. Restart Claude

## Quick Start

### For Team Members Using This Skill

**Every Monday morning (or whenever weekly email is due):**

1. **Open the template:** `team-workflow-template.md` (keep this file handy)

2. **Fill in all sections:**
   - Article details (title, author, date, image, content)
   - Market data (Nicole provides community stats)
   - Featured St. Andrews listings (top 3 properties)
   - Which communities need full listings pages

3. **Copy the completed template**

4. **Open Claude and say:**
   ```
   "Generate this week's market intelligence package using the weekly-email-team-instructions skill"
   ```

5. **Paste your filled template**

6. **Answer Claude's validation questions** (if any)

7. **Receive all HTML files** ready for deployment

8. **Deploy following Claude's checklist**

## Typical Weekly Workflow

### Monday Morning (Nicole)
- [ ] Pull latest MLS data for all 21 communities
- [ ] Export community stats (Active | Sold YTD | Absorption)
- [ ] Export full listing data for St. Andrews (always) + any other communities requested
- [ ] Send data to team member generating the email

### Monday Afternoon (Edmund/Samantha/Dina)
- [ ] Write weekly article (or finalize draft)
- [ ] Select hero image
- [ ] Choose article author/attribution
- [ ] Open `team-workflow-template.md`
- [ ] Fill in all sections with article + Nicole's data
- [ ] Paste into Claude with skill activated
- [ ] Answer validation questions
- [ ] Review generated HTML files

### Monday Late Afternoon (Team Member)
- [ ] Upload email.html to Constant Contact
- [ ] Push article HTML to GitHub (edmundbogen.github.io/[article-slug]/)
- [ ] Push dashboard updates to GitHub (edmundbogen.github.io/luxury-community-dashboard/)
- [ ] Push community listings to GitHub (edmundbogen.github.io/luxury-community-dashboard/[community]-listings.html)
- [ ] Send email preview to: edmund@, nicole@, dina@, samantha@
- [ ] Schedule or send email campaign

**Total Time:** ~20-30 minutes from data collection to deployment

## What Gets Generated

### 1. email.html
- **Destination:** Upload to Constant Contact
- **Format:** Single-column, inline CSS, 600px max width
- **Contains:** Hero article, executive summary, all 21 community stats, 3 featured St. Andrews listings, author bio
- **Email to:** edmund@bogenhomes.com, dina@, nicole@, samantha@

### 2. [article-slug].html
- **Destination:** GitHub Pages at `edmundbogen.github.io/[article-slug]/`
- **Format:** Full-width responsive, Montserrat font, long-form article
- **Contains:** Hero image, article content, author bio, footer
- **Example:** `nyc-tenant-czar-article.html`

### 3. index.html (Dashboard Update)
- **Destination:** GitHub Pages at `edmundbogen.github.io/luxury-community-dashboard/`
- **Format:** Interactive dashboard with Chart.js
- **Contains:** Featured article section, executive summary, all 21 community cards, charts
- **Note:** This UPDATES the existing dashboard, doesn't replace it entirely

### 4. [community-name]-listings.html (Multiple Files)
- **Destination:** GitHub Pages at `edmundbogen.github.io/luxury-community-dashboard/[community]-listings.html`
- **Format:** Property listing pages
- **Contains:** Community stats, all active listings with details
- **Example:** `st-andrews-listings.html`, `polo-club-listings.html`

## Troubleshooting

### "Skill not found"
- Verify skill is in correct directory: `~/.claude/skills/weekly-email-team-instructions/`
- Check that `SKILL.md` exists in the folder
- Restart Claude application

### "Missing required data"
Claude will flag any missing fields. Common issues:
- Article title not provided → Add title
- Community stats incomplete → Verify all 21 communities present
- Featured listings missing MLS# → Add MLS numbers
- Dates don't match → Confirm article date = market data date

### "Image not found"
- Images must be uploaded to `edmundbogen.github.io` BEFORE generating assets
- Use exact filename (case-sensitive)
- Supported formats: .png, .jpg, .jpeg

### "Property links broken"
- Use links from bogenhomes.com (NOT direct MLS links)
- Format: `https://bogenhomes.com/homes-for-sale-details/[ADDRESS]/[MLS]/[ID]/`
- Copy directly from the website listing

### HTML renders incorrectly
- Email: Test in Gmail, Outlook, Apple Mail before sending
- Web pages: Check mobile responsive at 768px, 1024px breakpoints
- Colors: Verify #1a3e5c (navy), #00a8e1 (cyan), #ffffff (white)

## Team Responsibilities

### Edmund
- Write/approve weekly articles
- Select article images
- Final review of all assets
- Approve deployment

### Nicole
- Compile all 21 community stats weekly
- Export MLS listing data
- Verify property details accuracy
- Provide data by Monday 9am

### Dina / Samantha
- Alternate article writing
- Fill out workflow template
- Generate assets via Claude
- Deploy to Constant Contact + GitHub
- Send team preview

## File Locations Reference

### Source Files (Team Maintains)
- Article content: [Google Docs or wherever articles are drafted]
- Community data: [Nicole's MLS export location]
- Images: `edmundbogen.github.io/luxury-community-dashboard/[images]/`

### Generated Files (Output)
- `email.html` → Constant Contact
- `[article-slug].html` → `edmundbogen.github.io/[article-slug]/index.html`
- `index.html` → `edmundbogen.github.io/luxury-community-dashboard/index.html`
- `[community]-listings.html` → `edmundbogen.github.io/luxury-community-dashboard/[community]-listings.html`

## Support

**Questions about the skill?**
- Check this README first
- Review `team-workflow-template.md` for data format examples
- Ask Claude: "How do I use the weekly-email-team-instructions skill?"

**Questions about deployment?**
- Constant Contact: [Your Constant Contact account manager]
- GitHub Pages: [Your GitHub repository admin]

**Questions about data/content?**
- Community stats: Nicole
- Article content: Edmund
- Brand guidelines: See `/references/brand-guidelines.md`

## Version History

**v1.0** - January 2026
- Initial release
- Supports all 4 asset types
- Interactive validation
- Brand guidelines integration
- 21 community template system

---

**Skill Author:** Edmund Bogen  
**Last Updated:** January 2026  
**Skill Name:** `weekly-email-team-instructions`
