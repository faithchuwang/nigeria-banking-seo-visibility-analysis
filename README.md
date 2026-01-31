# Nigeria-Banking-SEO-Visibility-Analysis
SEO visibility and search performance analysis of selected Nigerian consumer banks using keyword rankings, visibility scores, and revenue comparison.

## Project Background

The Nigerian consumer banking sector is highly competitive, with major banks competing for visibility across digital channels, particularly search engines. As customers increasingly rely on online search to compare banking services, SEO performance has become a key driver of brand visibility and customer acquisition.

This project analyzes search visibility and keyword performance for a selected group of 10 major Nigerian banks, using a curated dataset of 50 consumer banking–related keywords. The goal is to understand how banks perform in organic search, how visibility is distributed across competitors, and whether stronger SEO presence aligns with higher revenue levels.

Insights and recommendations are provided in the following key areas:

- **SEO Visibility Performance**: Evaluation of total visibility scores and ranking strength across banks to identify market leaders and laggards.
- **Keyword Coverage & Ranking Depth:** Analysis of how many keywords each bank ranks for and their relative positioning in search results.
- **Search Demand Analysis:** Identification of the highest-volume banking keywords driving consumer interest.
- **SEO Visibility vs Revenue:** Exploratory assessment of the relationship between search visibility and reported bank revenue.

An interactive Power BI dashboard used to explore SEO visibility, keyword rankings, and search performance across selected Nigerian consumer banks can be found here [link].

## **Data Structure & Initial Checks**

The project dataset is structured into **two main tables**, designed to support keyword-level SEO analysis and bank-level comparison. The combined dataset represents **50 consumer banking keywords** analyzed across **10 Nigerian consumer banks**.

A brief description of each table is provided below.

### **SEO_Table (Keyword Performance Table)**

This table contains keyword-level SEO and ranking information and forms the core of the analysis.

**Key fields include:**

* `Keyword` – Consumer banking search query
* `Search Volume` – Estimated monthly search volume
* `SEO Difficulty` – Organic ranking difficulty score
* `Paid Difficulty` – Paid competition indicator
* `Keyword Intent` – Classified as informational, transactional, navigational, or opportunity
* `Bank` – Name of the Nigerian bank appearing in search results
* `Rank` – Bank’s position in organic search results (1–10; 0 if not ranked)

Each row represents a **bank–keyword combination**, allowing direct comparison of SEO performance across banks.

### **Banks Table**

This table contains contextual information used for aggregation and correlation analysis.

**Key fields include:**

* `Bank` – Bank name
* `Revenue` – Reported or estimated annual revenue used for comparative analysis

This table is joined to the SEO_Table using the **Bank** field.

### **Initial Data Checks**

Before analysis, the following checks were performed:

* Verified consistency of bank naming across both tables
* Converted numeric fields stored as text into appropriate numeric formats
* Replaced missing rank values with zero to represent non-ranking keywords
* Confirmed keyword count consistency (50 unique keywords)
* Validated relationships between tables in Power BI’s data model

### **Data Model**

The data model follows a **one-to-many relationship**, where:

* One bank in the **Banks** table relates to multiple records in the **SEO_Table**

## Executive Summary

The analysis shows that SEO visibility in Nigerian consumer banking is highly concentrated, with a small number of banks consistently dominating organic search results while several others have limited or inconsistent visibility. Consumer search demand is heavily skewed toward branded digital banking queries, particularly internet banking and transfer-related terms, indicating that search behavior is largely navigational rather than exploratory. Additionally, SEO visibility does not scale directly with revenue, suggesting that targeted SEO strategy and keyword focus can create competitive advantages independent of bank size.

<img width="1198" height="673" alt="Screenshot 2026-01-30 at 20 52 23" src="https://github.com/user-attachments/assets/d877f2e4-c607-484e-b5ef-7b184ef7c924" />

## Insights Deep Dive

#### Search Demand Concentration & High-Volume Keywords:

- Search demand is heavily concentrated around branded online banking queries, with “UBA internet banking” recording the highest search volume at ~1.35M searches, significantly outperforming all other keywords.
- The second highest keyword, “Zenith Bank internet banking”, records ~740K searches, indicating that online banking access remains a dominant consumer search behavior.
- Non-branded but functional keywords such as “bank transfer code” appear multiple times across different banks, suggesting strong demand for transactional and USSD-related banking services.
- Lower-ranked keywords show a sharp drop-off in volume (≤0.08M), highlighting a long-tail distribution where only a few keywords drive the majority of search traffic.


#### Visualization: Top 10 Keywords by Search Volume

Keyword Coverage by Bank
Access Bank and First Bank lead keyword coverage, each ranking for 29 out of 50 tracked keywords, indicating broader SEO footprint compared to peers.


Stanbic Bank follows closely with 24 ranked keywords, positioning it as a strong mid-tier competitor in organic visibility.


GTBank and UBA rank for 18 and 17 keywords respectively, suggesting moderate coverage but room for expansion.


Polaris Bank ranks for only 2 keywords, reflecting extremely limited search visibility within the selected keyword set.


Visualization: Keywords Ranked by Bank

SEO Visibility Performance by Bank
First Bank holds the highest total visibility score (15.1), narrowly ahead of UBA (14.7), indicating strong overall ranking positions across tracked keywords.


Stanbic Bank (12.8) and Access Bank (12.2) form a competitive middle tier with comparable visibility performance.


GTBank records a visibility score of 10.9, lower than expected given brand strength, suggesting underperformance in organic rankings.


Polaris Bank’s visibility score of 0.5 confirms minimal SEO presence within this keyword set.


Visualization: Total Visibility Score by Bank

Relationship Between SEO Visibility and Revenue
Banks with higher visibility scores generally align with higher reported revenues, suggesting a positive relationship between organic search visibility and financial scale.


First Bank combines the highest visibility score (15.1) with strong revenue (~₦1.4T), reinforcing its leadership position.


Access Bank and UBA show high revenue figures (~₦2.6T and ~₦2.1T respectively) alongside solid visibility scores, indicating effective digital presence supporting business scale.


Lower-visibility banks (Sterling, Ecobank, Polaris) cluster at the lower end of the revenue axis, highlighting potential missed opportunities in search-driven customer acquisition.


Visualization: SEO Visibility vs Revenue (Scatter Plot)
