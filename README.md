# Comprehensive Analysis of EdTech Start-Ups in India

A Power BI dashboard project analyzing online course data to uncover learner engagement patterns, content performance, and strategic growth opportunities for an EdTech startup.

## Author

**Manish Lal Gupta**
- RTU Roll No: 23EACCS176
- Email: manishgupta1458149@gmail.com


## Project Overview

This project analyzes a dataset of online courses (Coursera-style platform data) to help an EdTech startup make data-driven decisions about content strategy, instructor partnerships, language localization, and category expansion. The dashboard answers 10 key business questions using Power BI, transforming raw course data into actionable insights.

## Dataset

- **File:** `data_Online_Courses.csv`
- Contains course-level data including title, category, sub-category, course type, language, subtitles, instructors, ratings, number of viewers, and duration.
- ~3,000 courses after data cleaning.

## Business Questions Answered

| # | Question |
|---|----------|
| Q1 | Total number of courses (after cleaning) |
| Q2 | Average rating across all courses |
| Q3 | Overall registrations & average registrations per course |
| Q4 | Distribution of course types across categories (and sub-categories) |
| Q5 | Average number of views by category, sub-category, and language |
| Q6 | Distribution of languages used across courses |
| Q7 | Language preferences for the top 5 categories by viewer demand |
| Q8 | Relationship between subtitle availability and number of views |
| Q9 | Top 3 instructors per category/sub-category based on ratings |
| Q10 | Relationship between course duration and number of views, by category/sub-category |

## Process

The project followed a standard data analysis workflow, from raw data to a polished, decision-ready dashboard:

1. **Data Collection**
   - Sourced a raw CSV export of online course listings (Coursera-style platform data) containing 8,800+ rows with details on title, category, instructors, ratings, viewers, duration, and more.

2. **Data Cleaning**
   - Removed duplicate, irrelevant, and blank columns left over from multiple merged source exports.
   - Standardized inconsistent text fields (e.g., rating values like `"4.9stars"`, viewer counts with commas like `"10,438"`).
   - Filtered out incomplete or corrupted rows, reducing the dataset to a clean ~3K usable courses.
   - Split multi-value fields (e.g., instructors, subtitle languages) where needed for accurate counting and analysis.

3. **Data Modeling**
   - Loaded the cleaned dataset into Power BI and defined data types (numeric, text, category) correctly for each field.
   - Created calculated columns/measures using DAX, including:
     - Average Rating, Total Registrations, Average Registration per Course
     - Average Number of Viewers by Category/Sub-Category/Language
     - Rank-based measures to identify Top 3 instructors per category

4. **Dashboard Design**
   - Built one visual page per business question (Q1–Q10) for clarity and ease of navigation.
   - Used KPI cards for single-number metrics (totals, averages).
   - Used bar charts, line charts, pie charts, and matrix tables depending on what best represented each relationship (distribution, trend, ranking).
   - Added interactive **category slicers** so the client can filter visuals (e.g., Q4, Q5) by category on demand.

5. **Analysis & Insight Generation**
   - Interpreted each visual to extract a clear, actionable insight (e.g., subtitle availability strongly correlates with higher engagement).
   - Synthesized all 10 answers into an overall **Project Conclusion** and a set of **Business Recommendations** for the EdTech client.

6. **Documentation**
   - Exported key dashboard views as images and compiled them with the dataset and findings into this repository for sharing and portfolio purposes.

## Key Findings

- **3K** total courses analyzed after cleaning, with an **average rating of 4.70**.
- **8M** overall registrations, averaging **3.22K registrations per course**.
- **Courses** (vs. Specializations) drive far higher total viewership (200K vs 44K), though Specializations have a higher average number of viewers per offering (2.4K vs 2.0K).
- **Data Science** has the highest average viewers per category (6.3K), followed by Information Technology (4.6K) and Computer Science (4.4K).
- **English dominates** the platform, accounting for 97.11% of content; Spanish is a distant second at 2.19%.
- Among the top 5 categories, **Data Science has the highest average registration per course (6,340.59)**, while Language Learning has the lowest (2,844.29).
- Courses with **more available subtitle languages correlate with significantly higher average registrations** — courses with 26 subtitle languages average ~86K registrations vs. near 0 for courses with very few subtitles.
- **Business** category instructors have the highest cumulative ratings among top-ranked instructors (5,580.70), followed by Data Science (2,614.20).
- Course duration's effect on viewership varies by category — some categories perform best with short, focused content while others support longer formats.

## Business Recommendations

1. Prioritize investment in the highest-performing categories based on viewership and learner demand.
2. Launch course types that align with successful category-specific trends identified in the analysis.
3. Expand multilingual content offerings and subtitle support to improve accessibility and audience reach.
4. Partner with top-rated instructors to create premium learning content and strengthen brand credibility.
5. Optimize course duration based on category-specific engagement patterns rather than a uniform content length.
6. Continuously monitor ratings, views, and language preferences to adapt content strategy to evolving learner needs.

## Tools Used

- **Power BI** — dashboard design, DAX measures, interactive visuals
- **Excel/CSV** — data source and cleaning

## Repository Structure

```
edtech-project/
├── README.md
├── data_Online_Courses.csv          # Raw dataset
└── images/                          # Dashboard screenshots
    ├── 01_title_page.png
    ├── 02_q1_total_courses.png
    ├── 03_q2_average_rating.png
    ├── 04_q3_overall_registered.png
    ├── 05_q4_course_type_distribution.png
    ├── 06_q5_avg_views_by_category.png
    ├── 07_q6_language_distribution.png
    ├── 08_q7_language_pref_top5_categories.png
    ├── 09_q8_subtitles_vs_views.png
    ├── 10_q9_top_instructors.png
    ├── 11_q10_duration_vs_views.png
    ├── 12_project_conclusion.png
    ├── 13_business_recommendations.png
    └── 14_final_outcome.png
```

> **Note:** The original `.pbix` Power BI file is not included in this repository. Only the dataset and dashboard screenshots are provided. If you'd like to reproduce the dashboard, open `data_Online_Courses.csv` in Power BI Desktop and recreate the visuals shown in `images/`.

## Dashboard Preview


### Q1 — Total Number of Courses (After Cleaning)
![Q1](images/02_q1_total_courses.png)

### Q2 — Average Ratings
![Q2](images/03_q2_average_rating.png)

### Q3 — Overall Registered & Average Registration per Course
![Q3](images/04_q3_overall_registered.png)

### Q4 — Course Type Distribution Across Categories
![Q4](images/05_q4_course_type_distribution.png)

### Q5 — Average Number of Views by Category, Sub-Category & Language
![Q5](images/06_q5_avg_views_by_category.png)

### Q6 — Distribution of Languages Across Courses
![Q6](images/07_q6_language_distribution.png)

### Q7 — Language Preferences for Top 5 Categories
![Q7](images/08_q7_language_pref_top5_categories.png)

### Q8 — Subtitle Availability vs. Number of Views
![Q8](images/09_q8_subtitles_vs_views.png)

### Q9 — Top 3 Instructors by Category & Sub-Category
![Q9](images/10_q9_top_instructors.png)

### Q10 — Course Duration vs. Number of Views
![Q10](images/11_q10_duration_vs_views.png)

### Project Conclusion
![Project Conclusion](images/12_project_conclusion.png)

### Business Recommendations
![Business Recommendations](images/13_business_recommendations.png)

### Final Outcome
![Final Outcome](images/14_final_outcome.png)

## Final Outcome

The dashboard transforms raw course data into actionable business intelligence, enabling the EdTech startup to make data-driven decisions regarding content creation, instructor partnerships, language localization, accessibility improvements, and category expansion — ultimately improving learner engagement and driving strategic growth.
