# Google AdSense Setup Guide

## Overview
Google Ads have been added to your website in 3 strategic locations:
1. **Header Banner** - Below the navigation/header section
2. **Middle Rectangle** - Between tools grid and info boxes
3. **Footer Banner** - Before the footer section

## Setup Instructions

### Step 1: Sign Up for Google AdSense
1. Go to [Google AdSense](https://www.google.com/adsense/start/)
2. Sign in with your Google account
3. Add your website URL: `https://yashwantbuilds.github.io/your-companion/`
4. Follow Google's verification process
5. Once approved, you'll get your **Publisher ID** (format: `ca-pub-xxxxxxxxxxxxxxxx`)

### Step 2: Get Your Ad Unit IDs
1. In AdSense dashboard, go to **Ads** > **Ad units**
2. Create new ad units with these specifications:

#### Ad Unit 1: Header Banner
- Name: `Header Banner`
- Type: `Display ads` (Responsive)
- Copy the **Ad Unit ID** (format: `xxxxxxxx`)

#### Ad Unit 2: Middle Rectangle
- Name: `Middle Rectangle`
- Type: `Display ads` (Responsive)
- Copy the **Ad Unit ID**

#### Ad Unit 3: Footer Banner
- Name: `Footer Banner`
- Type: `Display ads` (Responsive)
- Copy the **Ad Unit ID**

### Step 3: Update Your Files

Replace `ca-pub-xxxxxxxxxxxxxxxx` with your **Publisher ID** and `xxxxxxxx` with your respective **Ad Unit IDs** in both:
- `/index.html`
- `/root/index.html`

#### Example:
```html
<!-- BEFORE -->
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-xxxxxxxxxxxxxxxx"
 crossorigin="anonymous"></script>

<!-- AFTER -->
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-1234567890123456"
 crossorigin="anonymous"></script>
```

Similarly for ad unit IDs:
```html
<!-- BEFORE -->
<ins class="adsbygoogle"
     data-ad-client="ca-pub-xxxxxxxxxxxxxxxx"
     data-ad-slot="xxxxxxxx"
     ...></ins>

<!-- AFTER -->
<ins class="adsbygoogle"
     data-ad-client="ca-pub-1234567890123456"
     data-ad-slot="1234567890"
     ...></ins>
```

### Step 4: Commit and Deploy
Once you've updated the Publisher ID and Ad Unit IDs:

```bash
git add -A
git commit -m "Add Google AdSense integration with 3 ad placements"
git push origin main
```

### Step 5: Verify and Monitor
1. Wait 5-10 minutes for GitHub Pages to rebuild
2. Visit `https://yashwantbuilds.github.io/your-companion/`
3. Check if ads are displaying
4. Monitor performance in Google AdSense dashboard

## Ad Placements

### 1. Header Banner (Horizontal)
- **Location**: Below header, above feature badges
- **Dimensions**: Responsive (728x90 on desktop, mobile-optimized)
- **Purpose**: Captures immediate attention

### 2. Middle Rectangle (Vertical)
- **Location**: Between tools grid and info boxes
- **Dimensions**: Responsive (300x250 on desktop, mobile-optimized)
- **Purpose**: Natural scroll point in user journey

### 3. Footer Banner (Horizontal)
- **Location**: Before footer section
- **Dimensions**: Responsive (728x90 on desktop, mobile-optimized)
- **Purpose**: Last impression before leaving

## CSS Classes Available

- `.ad-container` - For vertical/rectangle ads (300x250)
- `.ad-container-horizontal` - For horizontal banner ads (728x90)
- `.ad-container-sidebar` - For sidebar ads (300x600) - *available for future use*
- `.ad-label` - Gray text label showing "Advertisement"

## Important Notes

⚠️ **AdSense Policies:**
- Do NOT click your own ads
- Do NOT ask visitors to click ads
- Do NOT place ads too close together
- Do NOT use deceptive ad placements
- Ensure content is valuable (which your tools are!)

✅ **Best Practices:**
- Ads should blend naturally with page design
- Maintain good user experience
- Monitor ad performance regularly
- Keep content quality high for better ad rates
- Test responsive design on mobile

## Troubleshooting

### Ads Not Showing
1. Check if your site is approved in AdSense
2. Verify Publisher ID is correct
3. Check browser console for errors
4. Allow 24 hours for ads to appear after approval
5. Disable ad blockers in your browser for testing

### Low Revenue
1. Increase site traffic
2. Optimize for high-value keywords (developer tools get good CPM)
3. Test different ad sizes
4. Ensure content is high-quality
5. Use multiple ad formats

### Invalid Traffic Warning
- Never click your own ads
- Don't use click-baiting headlines
- Ensure genuine traffic only
- Report any suspicious activity to Google

## File Locations
- Main home page: `/index.html`
- Backup copy: `/root/index.html`
- This guide: `/GOOGLE_ADS_SETUP.md`

## Next Steps
1. Get your Publisher ID and Ad Unit IDs from Google AdSense
2. Update the placeholder values in index.html files
3. Deploy to GitHub Pages
4. Monitor performance in AdSense dashboard
5. Optimize ad placements based on performance data

For more information, visit [Google AdSense Help](https://support.google.com/adsense/)
