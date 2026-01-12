# HTML Template Structures

This document provides the structural templates for each asset type. Actual generation should follow these structures while applying brand guidelines and inserting user-provided data.

## Email Template Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[ARTICLE_TITLE] - Luxury Communities Market Intelligence</title>
    <style>
        /* Inline CSS for email compatibility */
        body {
            margin: 0;
            padding: 0;
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
            background-color: #ffffff;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
            background-color: #ffffff;
        }
        .header {
            background-color: #1a3e5c;
            padding: 20px;
            text-align: center;
        }
        .hero {
            position: relative;
            width: 100%;
        }
        .hero img {
            width: 100%;
            height: auto;
            display: block;
        }
        .stat-grid {
            display: table;
            width: 100%;
        }
        .stat-card {
            display: table-cell;
            padding: 20px;
            border: 1px solid #e8e8e8;
            text-align: center;
        }
        .cta-button {
            background-color: #00a8e1;
            color: #ffffff;
            padding: 12px 30px;
            text-decoration: none;
            text-transform: uppercase;
            letter-spacing: 0.1em;
            display: inline-block;
        }
        /* More inline styles... */
    </style>
</head>
<body>
    <div class="container">
        
        <!-- HEADER SECTION -->
        <div class="header">
            <div style="color: #ffffff; font-size: 24px; font-weight: 300; letter-spacing: 0.1em;">
                THE EDMUND BOGEN TEAM
            </div>
            <div style="color: #00a8e1; font-size: 12px; text-transform: uppercase; margin-top: 8px;">
                Luxury Communities Market Intelligence
            </div>
            <div style="color: #ffffff; font-size: 14px; margin-top: 4px;">
                Palm Beach County Premium Real Estate Analysis
            </div>
            <div style="color: #999999; font-size: 12px; margin-top: 8px;">
                Market Data as of [DATE]
            </div>
        </div>

        <!-- HERO ARTICLE SECTION -->
        <div class="hero">
            <a href="https://edmundbogen.github.io/[ARTICLE_SLUG]/">
                <img src="https://edmundbogen.github.io/luxury-community-dashboard/[IMAGE_FILENAME]" 
                     alt="[ARTICLE_TITLE]" 
                     style="width: 100%; height: auto;">
            </a>
        </div>
        
        <div style="padding: 30px 20px; background-color: #1a3e5c; color: #ffffff;">
            <h2 style="margin: 0 0 10px 0; font-size: 24px; font-weight: 300; text-transform: uppercase; letter-spacing: 0.05em;">
                [ARTICLE_TITLE]
            </h2>
            <p style="margin: 0 0 20px 0; font-size: 16px; line-height: 1.6;">
                [ARTICLE_SUMMARY]
            </p>
            <a href="https://edmundbogen.github.io/[ARTICLE_SLUG]/" 
               style="background-color: #00a8e1; color: #ffffff; padding: 12px 30px; text-decoration: none; text-transform: uppercase; letter-spacing: 0.1em; display: inline-block;">
                READ THE FULL ANALYSIS
            </a>
        </div>

        <!-- ST. ANDREWS LISTINGS LINK -->
        <div style="padding: 20px; background-color: #f4f4f4; text-align: center;">
            <a href="https://edmundbogen.github.io/luxury-community-dashboard/st-andrews-listings.html" 
               style="color: #1a3e5c; text-decoration: none; font-weight: 600; font-size: 16px;">
                Listings currently at St. Andrews Country Club - click here
            </a>
        </div>

        <!-- EXECUTIVE MARKET SUMMARY -->
        <div style="padding: 30px 20px;">
            <h3 style="font-size: 20px; font-weight: 600; margin: 0 0 20px 0; color: #1a3e5c;">
                Executive Market Summary
            </h3>
            <table style="width: 100%; border-collapse: collapse;">
                <tr>
                    <td style="width: 50%; padding: 15px; border: 1px solid #e8e8e8; vertical-align: top;">
                        <div style="font-size: 12px; color: #666666; text-transform: uppercase; margin-bottom: 8px;">
                            St. Andrews Range
                        </div>
                        <div style="font-size: 20px; font-weight: 300; color: #1a3e5c;">
                            $[LOW]M-$[HIGH]M
                        </div>
                        <div style="font-size: 14px; color: #666666; margin-top: 4px;">
                            [ACTIVE_COUNT] Active
                        </div>
                    </td>
                    <td style="width: 50%; padding: 15px; border: 1px solid #e8e8e8; vertical-align: top;">
                        <div style="font-size: 12px; color: #666666; text-transform: uppercase; margin-bottom: 8px;">
                            Total Active
                        </div>
                        <div style="font-size: 20px; font-weight: 300; color: #1a3e5c;">
                            [TOTAL_ACTIVE]
                        </div>
                        <div style="font-size: 14px; color: #666666; margin-top: 4px;">
                            21 Communities
                        </div>
                    </td>
                </tr>
                <tr>
                    <td style="padding: 15px; border: 1px solid #e8e8e8; vertical-align: top;">
                        <div style="font-size: 12px; color: #666666; text-transform: uppercase; margin-bottom: 8px;">
                            Total Sold YTD
                        </div>
                        <div style="font-size: 20px; font-weight: 300; color: #1a3e5c;">
                            [TOTAL_SOLD]
                        </div>
                        <div style="font-size: 14px; color: #666666; margin-top: 4px;">
                            New Year
                        </div>
                    </td>
                    <td style="padding: 15px; border: 1px solid #e8e8e8; vertical-align: top;">
                        <div style="font-size: 12px; color: #666666; text-transform: uppercase; margin-bottom: 8px;">
                            2026 Status
                        </div>
                        <div style="font-size: 20px; font-weight: 300; color: #1a3e5c;">
                            [STATUS_LABEL]
                        </div>
                        <div style="font-size: 14px; color: #666666; margin-top: 4px;">
                            [DATE]
                        </div>
                    </td>
                </tr>
            </table>
        </div>

        <!-- ALL COMMUNITIES LINK -->
        <div style="padding: 20px; background-color: #f4f4f4; text-align: center;">
            <a href="https://edmundbogen.github.io/luxury-community-dashboard/" 
               style="background-color: #00a8e1; color: #ffffff; padding: 12px 30px; text-decoration: none; text-transform: uppercase; letter-spacing: 0.1em; display: inline-block;">
                ALL 21 LUXURY COMMUNITIES
            </a>
        </div>

        <!-- COMMUNITY STATS GRID -->
        <!-- Repeat for all 21 communities -->
        <div style="padding: 20px;">
            [REPEAT: Community card structure for each of 21 communities]
        </div>

        <!-- FEATURED ST. ANDREWS LISTINGS -->
        <div style="padding: 30px 20px; background-color: #f4f4f4;">
            <h3 style="font-size: 20px; font-weight: 600; margin: 0 0 20px 0; color: #1a3e5c;">
                Featured St. Andrews Listings
            </h3>
            
            [REPEAT: Property card for each of 3 featured listings]
        </div>

        <!-- EDMUND'S MASTERMIND CTA -->
        <div style="padding: 30px 20px; background-color: #1a3e5c; text-align: center;">
            <h3 style="color: #ffffff; font-size: 22px; margin: 0 0 10px 0;">
                Edmund's Mastermind
            </h3>
            <p style="color: #ffffff; font-size: 16px; line-height: 1.6;">
                AI is changing everything - come to my mastermind to make sense of Business, Sales and Life
            </p>
            <a href="https://www.bogen.ai/contact?tab=client" 
               style="background-color: #00a8e1; color: #ffffff; padding: 12px 30px; text-decoration: none; text-transform: uppercase; letter-spacing: 0.1em; display: inline-block; margin-top: 10px;">
                LEARN MORE
            </a>
        </div>

        <!-- DASHBOARD LINK -->
        <div style="padding: 20px; text-align: center;">
            <a href="https://edmundbogen.github.io/luxury-community-dashboard/" 
               style="color: #1a3e5c; font-size: 16px; text-decoration: none; font-weight: 600;">
                📊 View Full Interactive Dashboard
            </a>
        </div>

        <!-- ABOUT AUTHOR BIO -->
        <div style="padding: 30px 20px; background-color: #f4f4f4;">
            <h3 style="font-size: 20px; font-weight: 600; margin: 0 0 20px 0; color: #1a3e5c;">
                About [AUTHOR_NAME]
            </h3>
            <table style="width: 100%;">
                <tr>
                    <td style="width: 100px; vertical-align: top;">
                        <img src="https://edmundbogen.github.io/luxury-community-dashboard/[AUTHOR_PHOTO]" 
                             alt="[AUTHOR_NAME]" 
                             style="width: 80px; height: 80px; border-radius: 50%;">
                    </td>
                    <td style="padding-left: 20px; vertical-align: top;">
                        <p style="font-size: 14px; line-height: 1.6; color: #333333; margin: 0;">
                            [AUTHOR_BIO]
                        </p>
                        <p style="margin-top: 15px;">
                            <a href="tel:+15612357575" style="color: #00a8e1; text-decoration: none;">
                                📞 (561) 235-7575
                            </a><br>
                            <a href="mailto:edmund@bogenhomes.com" style="color: #00a8e1; text-decoration: none;">
                                ✉️ edmund@bogenhomes.com
                            </a>
                        </p>
                    </td>
                </tr>
            </table>
        </div>

        <!-- FOOTER -->
        <div style="padding: 30px 20px; background-color: #1a3e5c; color: #ffffff; text-align: center; font-size: 12px; line-height: 1.6;">
            <p style="margin: 0 0 10px 0; font-weight: 600;">
                Luxury Communities Market Intelligence Dashboard
            </p>
            <p style="margin: 0 0 10px 0;">
                Prepared by <strong>The Edmund Bogen Team</strong> | Douglas Elliman Real Estate
            </p>
            <p style="margin: 0 0 20px 0;">
                Data Sources: MLS, Public Records, Market Analysis 2026
            </p>
            <p style="margin: 0; color: #999999; font-size: 11px;">
                📍 Serving Palm Beach County's Luxury Communities<br>
                1111 LINCOLN RD, MIAMI BEACH, FL 33139. 305.695.6300
            </p>
            <p style="margin: 20px 0 0 0; color: #999999; font-size: 10px; line-height: 1.4;">
                © 2018 DOUGLAS ELLIMAN REAL ESTATE. ALL MATERIAL PRESENTED HEREIN IS INTENDED FOR INFORMATION PURPOSES ONLY. 
                WHILE, THIS INFORMATION IS BELIEVED TO BE CORRECT, IT IS REPRESENTED SUBJECT TO ERRORS, OMISSIONS, CHANGES 
                OR WITHDRAWAL WITHOUT NOTICE. ALL PROPERTY INFORMATION, INCLUDING, BUT NOT LIMITED TO SQUARE FOOTAGE, ROOM COUNT, 
                NUMBER OF BEDROOMS AND THE SCHOOL DISTRICT IN PROPERTY LISTINGS SHOULD BE VERIFIED BY YOUR OWN ATTORNEY, 
                ARCHITECT OR ZONING EXPERT. IF YOUR PROPERTY IS CURRENTLY LISTED WITH ANOTHER REAL ESTATE BROKER, PLEASE 
                DISREGARD THIS OFFER. IT IS NOT OUR INTENTION TO SOLICIT THE OFFERINGS OF OTHER REAL ESTATE BROKERS. 
                WE COOPERATE WITH THEM FULLY. EQUAL HOUSING OPPORTUNITY.
            </p>
        </div>

    </div>
</body>
</html>
```

## Article Page Template Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[ARTICLE_TITLE] | The Edmund Bogen Team</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Montserrat', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
            line-height: 1.7;
            color: #333333;
        }
        .nav {
            background-color: #1a3e5c;
            padding: 20px 40px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .hero {
            position: relative;
            height: 60vh;
            background-size: cover;
            background-position: center;
            background-image: linear-gradient(rgba(26, 62, 92, 0.5), rgba(26, 62, 92, 0.7)), 
                              url('[IMAGE_URL]');
        }
        .hero-content {
            position: absolute;
            bottom: 60px;
            left: 40px;
            color: #ffffff;
            max-width: 800px;
        }
        .article-container {
            max-width: 900px;
            margin: 0 auto;
            padding: 60px 40px;
        }
        h1 {
            font-size: 48px;
            font-weight: 300;
            margin-bottom: 20px;
            text-transform: uppercase;
            letter-spacing: 0.05em;
        }
        h2 {
            font-size: 32px;
            font-weight: 500;
            margin: 40px 0 20px 0;
            color: #1a3e5c;
            padding-bottom: 10px;
            border-bottom: 3px solid #00a8e1;
        }
        .stat-callout {
            background-color: #f4f4f4;
            border-left: 4px solid #00a8e1;
            padding: 20px 30px;
            margin: 30px 0;
        }
        .pull-quote {
            border-left: 5px solid #00a8e1;
            padding-left: 30px;
            margin: 40px 0;
            font-size: 20px;
            font-style: italic;
            color: #1a3e5c;
        }
        .author-bio {
            background-color: #f4f4f4;
            padding: 40px;
            margin-top: 60px;
            border-radius: 8px;
        }
        /* More styles... */
    </style>
</head>
<body>

    <!-- NAVIGATION -->
    <nav class="nav">
        <div style="color: #ffffff; font-size: 18px; font-weight: 500;">
            The Edmund Bogen Team at Douglas Elliman
        </div>
        <div>
            <a href="https://www.bogenhomes.com" style="color: #ffffff; text-decoration: none; margin-left: 20px;">Properties</a>
            <a href="https://www.bogenhomes.com/contact" style="color: #ffffff; text-decoration: none; margin-left: 20px;">Contact</a>
        </div>
    </nav>

    <!-- HERO -->
    <div class="hero" style="background-image: linear-gradient(rgba(26, 62, 92, 0.5), rgba(26, 62, 92, 0.7)), 
                                               url('https://edmundbogen.github.io/luxury-community-dashboard/[IMAGE_FILENAME]');">
        <div class="hero-content">
            <div style="font-size: 14px; text-transform: uppercase; letter-spacing: 0.15em; margin-bottom: 15px; color: #00a8e1;">
                Market Commentary
            </div>
            <h1>[ARTICLE_TITLE]</h1>
            <p style="font-size: 20px; font-weight: 400; margin-top: 15px;">
                [ARTICLE_SUBTITLE]
            </p>
            <p style="font-size: 14px; margin-top: 10px; opacity: 0.9;">
                By [AUTHOR_NAME] | [DATE]
            </p>
        </div>
    </div>

    <!-- ARTICLE CONTENT -->
    <div class="article-container">
        
        <!-- Key Stats Callouts -->
        <div style="display: flex; gap: 20px; margin: 40px 0;">
            [STAT_CALLOUTS - typically 3 key metrics]
        </div>

        <!-- Article Body -->
        [FULL_ARTICLE_CONTENT_WITH_FORMATTING]
        
    </div>

    <!-- AUTHOR BIO -->
    <div class="author-bio">
        [AUTHOR_PHOTO + BIO + CONTACT]
    </div>

    <!-- FOOTER -->
    <footer style="background-color: #1a3e5c; color: #ffffff; padding: 40px; text-align: center;">
        [FOOTER_CONTENT]
    </footer>

</body>
</html>
```

## Dashboard Template Structure

(Similar structure to article page but with Chart.js integration and interactive elements)

## Community Listings Template Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[COMMUNITY_NAME] - Current Listings | The Edmund Bogen Team</title>
    <style>
        /* Styles similar to dashboard */
    </style>
</head>
<body>

    <!-- Back Navigation -->
    <div style="padding: 20px 40px;">
        <a href="index.html" style="color: #1a3e5c; text-decoration: none; font-weight: 500;">
            ← Back to Market Dashboard
        </a>
    </div>

    <!-- Page Header -->
    <div style="padding: 40px; background-color: #1a3e5c; color: #ffffff;">
        <h1 style="font-size: 36px; font-weight: 300; margin-bottom: 10px;">
            [COMMUNITY_NAME] - Available Listings
        </h1>
        <p style="font-size: 14px; opacity: 0.9;">
            Updated [DATE] | [ACTIVE_COUNT] Active Listings
        </p>
    </div>

    <!-- 4-Stat Summary Grid -->
    <div style="padding: 40px;">
        <div style="display: grid; grid-template-columns: repeat(4, 1fr); gap: 20px;">
            [4 stat cards: Price Range, Active, Sold YTD, Absorption]
        </div>
    </div>

    <!-- Property Listings -->
    <div style="padding: 0 40px 40px 40px;">
        [REPEAT: Property card for each listing in community]
    </div>

    <!-- Contact CTA -->
    <div style="padding: 40px; background-color: #f4f4f4; text-align: center;">
        <h3 style="font-size: 24px; margin-bottom: 20px;">
            Questions about [COMMUNITY_NAME]?
        </h3>
        <a href="https://bogenhomes.com/contact/" 
           style="background-color: #00a8e1; color: #ffffff; padding: 15px 40px; text-decoration: none; text-transform: uppercase; letter-spacing: 0.1em; display: inline-block;">
            CONTACT EDMUND BOGEN
        </a>
    </div>

    <!-- Footer -->
    <footer style="background-color: #1a3e5c; color: #ffffff; padding: 20px; text-align: center;">
        The Edmund Bogen Team | Douglas Elliman Real Estate | (561) 235-7575
    </footer>

</body>
</html>
```

---

## Notes on Template Usage

1. **Variables** are shown in `[BRACKETS]` and should be replaced with actual data
2. **Repeat blocks** are noted with `[REPEAT: ...]` comments
3. **Inline CSS** is used for email, external CSS for web pages
4. **Brand colors** are hardcoded but should match brand guidelines exactly
5. **All images** must use absolute URLs pointing to edmundbogen.github.io
6. **Mobile responsiveness** should be tested across devices
7. **Email compatibility** should be tested in Gmail, Outlook, Apple Mail

These are STRUCTURAL templates - actual generated HTML will be more complete with all styling, content, and validation.
