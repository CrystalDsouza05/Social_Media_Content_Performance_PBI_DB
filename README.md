# Social Media Content Performance Dashboard

### 📊 [Dashboard Link](https://app.powerbi.com/groups/me/reports/384d017e-e935-44dc-9e7d-1626c1a36de1/ReportSection)

## 📌 Problem Statement

This Power BI dashboard tracks and visualizes the performance of social media content across platforms like Instagram, LinkedIn, Facebook, TikTok, YouTube, and X.com. It allows teams to assess what type of content resonates most, how users engage based on geography, time, and platform, and uncover high-performing hashtags, post types, and user behaviors. This insight helps in refining social media strategy and boosting content ROI.

---

## 📁 File Details

- **File Name:** `Crystal_Social_Media_Content_DB.pbix`
- **File Path:** `G:/My Drive/Personal/Github/Power BI/Social Media Content/`

---

## 📄 Pages Included

| Page No. | Page Name                  |
|----------|----------------------------|
| 1        | Executive Summary          |
| 2        | Platform & Content Deep Dive |
| 3        | Temporal & Geo Performance |

---

## 🧩 Key Visuals and Features

### ✅ Executive Summary
- **KPI Cards** for total posts, engagement, views, likes, comments, and shares  
- **Donut Chart** for post type & content share breakdown  
- **Bar Chart** for engagement by region  
- **Timeline Chart** for daily engagement & MoM %  
- **Advanced Slicers** for content type, engagement level, and platform  
- **Dynamic Icons & Branding** using company logos and color palettes  

### ✅ Platform & Content Deep Dive
- Engagement metrics: CTR, ER%, clicks per view  
- **Top Performing Posts Table**  
- **Top Hashtags & Clicks by Hashtags**  
- Engagement rate matrix by platform & content category  

### ✅ Temporal & Geo Performance
- **Map visual** for geographic engagement  
- **Time of Day vs Engagement Pivot Table**  
- **Post frequency by region**  
- **Slicers** for granular date/time analysis  

---

## ⚙️ DAX Measures & Expressions

Some of the DAX measures used in the dashboard include:

```DAX
Click - Through Rate = [Total Clicks] / [Total Views]
ER% = ([Total Engagement] / [Total Posts])

```

---

## 📊 Tables & Relationships

- **Main Tables Used:**
  - `Posts` (Post data, platforms, content)
  - `Key Measures` (aggregated KPIs)
  - `Dates` (calendar for time analysis)
  - `Location` (region and geo info)
  - `Icons` and `Colour Codes` (branding visuals)

- **Relationships:**
  - Dates linked to post published date  
  - Region in `Posts` linked to `Location`  
  - Platform linked to icons and color codes  

---


## 🔍 Insights Uncovered

- **Instagram** leads in engagement and reach  
- **Reels** & **Carousels** outperform single-image posts  
- **Mid-week posts** perform best (Wednesday & Thursday)  
- **Top hashtags** drive higher clicks and engagement  
- **Business-related posts** show higher CTR on LinkedIn  

---

## 🚀 Tech Stack

- Power BI Desktop & Power BI Service  
- DAX  
- Power Query  
- ZoomCharts Visuals  
- PBI Helper for documentation

---

Feel free to connect or reach out if you’d like to learn more about this dashboard or build something similar! 😊

