# 21 Luxury Communities Reference

Complete list of Palm Beach County luxury communities tracked in The Edmund Bogen Team's weekly market intelligence package.

## All Communities (Alphabetical)

1. Addison Reserve
2. Boca Bridges
3. Boca Grove
4. Boca West Country Club
5. Bocaire Country Club
6. Broken Sound
7. Delaire Country Club
8. Le Lac
9. Long Lake Estates
10. Lotus
11. Mizner Country Club
12. Polo Club
13. Royal Palm Yacht Club
14. Seasons
15. Seven Bridges
16. St. Andrews Country Club
17. Stonebridge
18. The Bridges
19. The Oaks
20. The Sanctuary
21. Woodfield

## Community URL Slugs

For generating listings pages, use these URL-friendly slugs:

- St. Andrews Country Club → `st-andrews-listings.html`
- Delaire Country Club → `delaire-listings.html`
- Boca West Country Club → `boca-west-listings.html`
- Polo Club → `polo-club-listings.html`
- Broken Sound → `broken-sound-listings.html`
- The Bridges → `the-bridges-listings.html`
- The Oaks → `the-oaks-listings.html`
- Mizner Country Club → `mizner-listings.html`
- Addison Reserve → `addison-reserve-listings.html`
- Lotus → `lotus-listings.html`
- Seven Bridges → `seven-bridges-listings.html`
- Boca Grove → `boca-grove-listings.html`
- Seasons → `seasons-listings.html`
- Stonebridge → `stonebridge-listings.html`
- Bocaire Country Club → `bocaire-listings.html`
- Royal Palm Yacht Club → `royal-palm-listings.html`
- The Sanctuary → `the-sanctuary-listings.html`
- Long Lake Estates → `long-lake-listings.html`
- Le Lac → `le-lac-listings.html`
- Boca Bridges → `boca-bridges-listings.html`
- Woodfield → `woodfield-listings.html`

## Community Data Structure

Each community requires the following data points for weekly reporting:

### Summary Stats (for email & dashboard)
- Active Listings (count)
- Sold YTD (count)
- Absorption Rate (percentage or "N/A")

### Full Listings Page Stats
- Price Range (Low - High in millions)
- Active Listings (count)
- Sold YTD (count)
- Absorption Rate (percentage or "N/A")

### Individual Property Data
For each active listing in a community:
- Address (street address)
- Price ($X,XXX,XXX)
- Bedrooms (count)
- Bathrooms (count with decimal for half-baths)
- Living Square Feet (formatted with commas)
- Year Built (YYYY)
- Lot Square Feet (formatted with commas)
- MLS Number (format: RX-XXXXXXXX or FXXXXXXXXX)
- Days on Market (count)
- Feature Badge (optional: "New Construction 2026", "Waterfront", "Golf & Lake Views", "Price Reduced")
- Property URL (link to bogenhomes.com listing page)

## Special Considerations

### St. Andrews Country Club
- Featured prominently in every email (3 top listings highlighted)
- Edmund is a member, so this community gets priority placement
- Always shown at top of community stats grid

### Featured Communities
Some communities consistently have higher volume and may need full listings pages more frequently:
- Boca West Country Club (typically 35-45 active)
- Broken Sound (typically 30-40 active)
- Royal Palm Yacht Club (typically 35-45 active)

### Smaller Communities
These typically have fewer than 10 active listings:
- Le Lac (often 1-5 active)
- Long Lake Estates (typically 5-8 active)
- Delaire Country Club (typically 4-8 active)

## Data Source

All community data is provided by Nicole Hudson, compiled from MLS (Multiple Listing Service) via the team's access at bogenhomes.com.

**Nicole's Responsibility:**
- Pull weekly stats for all 21 communities
- Export current active listings for any communities needing full pages
- Verify MLS numbers and property URLs
- Calculate or note Days on Market

**Format Nicole Should Use:**
```
Community Name | Active | Sold YTD | Absorption Rate
St. Andrews Country Club | 13 | 0 | N/A
Delaire Country Club | 4 | 0 | N/A
[etc.]
```

## Validation Rules

When processing community data:
1. All 21 communities MUST be present (even if some have 0 active listings)
2. Active count must be a positive integer or zero
3. Sold YTD must be a positive integer or zero
4. Absorption Rate must be a percentage (e.g., "73%") or "N/A"
5. If generating a full listings page, ALL active listings must be provided (not just featured ones)

## Historical Context

These 21 communities represent Palm Beach County's most prestigious luxury residential developments. Price points generally range from $1M to $20M+, with St. Andrews and Boca West being among the highest-value markets.

The weekly tracking demonstrates The Edmund Bogen Team's market expertise and provides high-net-worth clients with institutional-grade data intelligence.

---

**Last Updated:** January 2026
