# GA4 Conversion Tracking Setup Guide
**Sources:** YouTube (Andrew Hubbard), Graphed.com, Sahu Technologies, Google Support, YouTube (ETL Mentor)
**Research Date:** April 2026

---

## Overview

Google Analytics 4 (GA4) tracks form submissions, lead magnet downloads, and other conversion actions as **events**. Setup requires Google Tag Manager (GTM) to avoid hard-coding changes into the website.

---

## Step-by-Step: Setup for Form Submissions & Lead Magnet Downloads

### Step 1 — Set Up GA4 Account & Property
1. Go to analytics.google.com
2. Create an account → Create a property (website name)
3. Set timezone and currency
4. Create a **web data stream**
5. Copy your **Measurement ID** (format: G-XXXXXXXXXX)

### Step 2 — Install Google Tag Manager
1. Go to tagmanager.google.com
2. Create an account and container
3. Copy the **GTM Container ID** (format: GTM-XXXXXXX)
4. Install GTM code snippet in your website's `<head>` tag
   - **WordPress:** Use the "GTM4WP" plugin, paste Container ID, enable
   - **Wix/Squarespace/Clay:** Search "[platform] how to install script in head tag"
5. Verify installation using the **Tag Assistant Chrome extension**

### Step 3 — Create GA4 Base Tag in GTM
1. GTM → Tags → New → Name it "GA4 Base Tag"
2. Tag type: "Google Analytics: GA4 Configuration"
3. Paste your **Measurement ID**
4. Enable "Send a page view event when this configuration loads"
5. Set firing priority to **10** (highest)
6. Trigger: **All Pages**
7. Save & Publish

### Step 4 — Create Conversion Event Tags

**For Form Submissions (lead qualification form):**
1. GTM → Tags → New → Name it "GA4 Event - Generate Lead"
2. Tag type: "Google Analytics: GA4 Event"
3. Select GA4 Base Tag as configuration
4. Event name: `generate_lead`
5. Set trigger → Page View → fires ONLY on thank-you/confirmation page URL
6. Save & Publish

**For Lead Magnet Downloads:**
- Option A (automatic): Enable **Enhanced Measurement** in GA4 → automatically tracks `file_download` events for PDFs
- Option B (custom): Create event when user lands on download confirmation page
  - GA4 Admin → Events → Create Event
  - When `page_view` on URL containing "/download-thank-you" → create `lead_magnet_download`
  - Mark as conversion

### Step 5 — Mark Events as Conversions in GA4
1. GA4 Admin → Data Display → Events
2. Find your events: `generate_lead`, `sign_up`, `file_download`, `lead_magnet_download`
3. Toggle **"Mark as conversion"** on each
4. Data appears in Conversions report within **24–48 hours**

---

## Recommended Event Names (GA4 Standard)

| Event Name | When to Use |
|---|---|
| `generate_lead` | Qualification form submitted |
| `sign_up` | Newsletter, webinar, or membership interest form |
| `file_download` | Lead magnet PDF downloaded |
| `lead_magnet_download` | Custom event for specific gated asset |

---

## Key GA4 Reports for Lead Generation

| Report | Location | What It Shows |
|---|---|---|
| **Traffic Acquisition** | Reports → Acquisition → Traffic acquisition | Conversions by channel (Organic, Email, Social, Direct) |
| **Conversions** | Reports → Engagement → Conversions | Total count of each conversion event |
| **Engagement** | Reports → Engagement | Time on page, scroll depth, pre-conversion behavior |
| **Realtime** | Reports → Realtime | Live verification that tracking is firing |
| **Explorations** | Explore | Custom dashboards combining any metrics |

---

## Key Metrics to Monitor

| Metric | How to Interpret |
|---|---|
| **Conversion count** | Total leads — compare to prior periods |
| **Conversion rate** (calculate: conversions / sessions × 100) | 2–5% typical; 10%+ excellent; <1% needs work |
| **Conversions by channel** | Organic = high-intent; Email = warm leads; Paid = volume |
| **Conversions by landing page** | Identify which pages convert best → invest in more like them |
| **Time to conversion** | How long after first visit do users convert |

---

## Attribution Models

| Model | What It Credits | Best For |
|---|---|---|
| First-click | Channel that first brought user to site | Awareness analysis |
| Last-click | Channel user came from before converting | Direct conversion analysis |
| Data-driven (default in GA4) | ML allocates credit across all touchpoints | Most accurate overall |

---

## Multi-Domain Setup (If Needed)

If the site spans multiple domains (e.g., main site + separate event registration page):
1. GA4 Admin → Data Streams → Your stream → Configure tag settings → Configure your domains
2. Add all domains (subdomains are automatic)
3. Verify: clicking between domains should append `?_gl=` parameter to URLs

---

## Verification Checklist

- [ ] GTM installed on all pages (verify with Tag Assistant)
- [ ] GA4 Base Tag firing on all pages
- [ ] `generate_lead` event fires only on form thank-you page
- [ ] `file_download` or `lead_magnet_download` event fires on PDF access
- [ ] All conversion events toggled ON in GA4 Events list
- [ ] Data showing in GA4 Conversions report within 24–48 hours
- [ ] Realtime report shows live events firing during testing

---

## Notes on Data Delays

- New events can take **up to 24 hours** to appear in GA4 reports
- Always verify in **Realtime** immediately after publishing GTM changes
- Tag Assistant extension shows events firing in real-time for testing

---

## Recommended Additional Tools

| Tool | Purpose |
|---|---|
| Google Tag Manager | Tag management without code changes |
| Tag Assistant (Chrome extension) | Real-time verification of event firing |
| Google Search Console | Organic search performance + keyword data |
| Hotjar | Heatmaps and session recordings for UX optimization |
| Meta Pixel | Track conversions from social media ads (if added later) |
