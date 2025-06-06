# Social Media Content Performance Dashboard

### 📊 [Dashboard Link](https://app.powerbi.com/groups/me/reports/384d017e-e935-44dc-9e7d-1626c1a36de1/ReportSection)

## 📌 Problem Statement

This Power BI dashboard tracks and visualizes the performance of social media content across platforms like Instagram, LinkedIn, Facebook, TikTok, YouTube, and X.com. It allows teams to assess what type of content resonates most, how users engage based on geography, time, and platform, and uncover high-performing hashtags, post types, and user behaviors. This insight helps in refining social media strategy and boosting content ROI.

---

Snap of Dashboad Pages (3) ,

![Image](https://github.com/user-attachments/assets/67c615bb-5a72-459e-a9b2-020fbc236b53)

![Image](https://github.com/user-attachments/assets/75b3ca99-3fc7-418e-9ec6-ef3d620a2aff)

![Image](https://github.com/user-attachments/assets/bb21c2a9-6a68-48aa-9b6c-d778de931d81)

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
- **Dynamic Icons & Branding** using company logos

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

```📐 Key Measures:

Totals:
Total Posts = COUNT(Posts[Post_ID])
Total Engagement = SUM(Posts[Engagement])
Total Views = SUM(Posts[Views])
Total Likes = SUM(Posts[Likes])
Total Comments = SUM(Posts[Comments])
Total Shares = SUM(Posts[Shares])
Total Video Views = SUM(Posts[Video_Views])
Total Impressions = SUM(Posts[Impressions])
Total Clicks = SUM(Posts[Clicks])

Other Measures:
Avg Engagement = AVERAGE(Posts[Engagement_Rate])
Click-Through Rate (CTR) = DIVIDE(SUM(Posts[Clicks]), SUM(Posts[Impressions]), 0)
Clicks per view = DIVIDE(SUM('Posts'[Clicks]), [Total Views], 0)
Video View Rate = DIVIDE([Total Video Views], [Total Views], 0)
Live Stream View Rate = DIVIDE(SUM('Posts'[Live_Stream_Views]), [Total Views], 0)
Engagement – Previous Month = CALCULATE([Total Engagement], DATEADD(Dates[Date], -1, MONTH))
Engagement per post = DIVIDE([Total Engagement], [Total Posts], 0)
Engagement MoM % Change =
  DIVIDE(
    [Total Engagement] - [Engagement Previous Month],
    [Engagement Previous Month])
Engagement Rate (%) – ER% = DIVIDE([Total Engagement], [Total Views], 0)
Post Title (Dynamic Labeling) = SELECTEDVALUE('Colour Codes'[Name], "Social Media Marketing Dashboard (All Media)")

```
## Info Button Bookmark. 

![Image](https://github.com/user-attachments/assets/0aa690b7-c024-43ad-9d9e-14b9b9c14ea3)

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
- PowerPoint and Figma for Design
- PBI Helper for documentation

---

Feel free to connect or reach out if you’d like to learn more about this dashboard or build something similar! 😊

