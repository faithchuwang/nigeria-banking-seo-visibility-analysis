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

Got it — this is a **GitHub README–style “Data Structure & Initial Checks” section**, short and factual, adapted **exactly to your project** (Power BI + SEO, not a company SQL database).

Here is the **clean, correct version** you should use 👇

---

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

---

### **Data Model**

The data model follows a **one-to-many relationship**, where:

* One bank in the **Banks** table relates to multiple records in the **SEO_Table**
