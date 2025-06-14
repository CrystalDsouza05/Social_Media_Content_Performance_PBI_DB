# Social Media Content Performance Dashboard

### 📊 [Dashboard Link](https://app.powerbi.com/view?r=eyJrIjoiMWRiMTQzOTUtZGEzYy00NjY1LWEwNzgtNzAyODY0MDU1YmY5IiwidCI6IjQ2NTRiNmYxLTBlNDctNDU3OS1hOGExLTAyZmU5ZDk0M2M3YiIsImMiOjl9)

## 📌 Problem Statement

This Power BI dashboard tracks and visualizes the performance of social media content across platforms like Instagram, LinkedIn, Facebook, TikTok, YouTube, and X.com. It allows teams to assess what type of content resonates most, how users engage based on geography, time, and platform, and uncover high-performing hashtags, post types, and user behaviors. This insight helps in refining social media strategy and boosting content ROI.

---

Snap of Dashboad Pages (3) ,

![image](https://github.com/user-attachments/assets/9e95d0bf-f0a0-4086-96c7-e8be349d8515)

![image](https://github.com/user-attachments/assets/16c7674c-c13e-4ea8-878e-d063fe04cee9)

![image](https://github.com/user-attachments/assets/3cd28538-01f0-4726-abec-a1f84e990429)

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

`Totals:`
Total Posts = COUNT(Posts[Post_ID])
Total Engagement = SUM(Posts[Engagement])
Total Views = SUM(Posts[Views])
Total Likes = SUM(Posts[Likes])
Total Comments = SUM(Posts[Comments])
Total Shares = SUM(Posts[Shares])
Total Video Views = SUM(Posts[Video_Views])
Total Impressions = SUM(Posts[Impressions])
Total Clicks = SUM(Posts[Clicks])

`Other Measures:`
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

![image](https://github.com/user-attachments/assets/b3f09e00-4776-4b70-9c2c-0906f7763be5)

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

- **Data Model:**
![Image](https://github.com/user-attachments/assets/5d229f3c-fe12-48ae-8e38-94052984276a)
---

## 🔍 Insights Uncovered

- **Youtube** leads in engagement and reach  
- **Videos** & **Images** outperform other posts type by Shares
- **Mid-week posts** perform best (Wednesday & Thursday) in the mornings and afternoons 
- **Top hashtags** drive higher clicks and engagement  
- **#CustomerStory** is the Top Hashtag that drives higher clicks and engagement  
---

## 🚀 Tech Stack

- Power BI Desktop & Power BI Service
- MS Excel for Data Source 
- DAX  
- Power Query  
- ZoomCharts Visuals
- PowerPoint and Figma for Design
- PBI Helper for documentation

---

Feel free to connect or reach out if you’d like to learn more about this dashboard or build something similar! 😊

