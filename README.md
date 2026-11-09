# Data Science Salary Analysis for Competitive Hiring

What should a fast-growing small company pay its first data scientist? This project analyzes data scientist salaries to recommend a competitive pay range, and compares hiring in the United States with hiring offshore.

**Tools:** R · dplyr · ggplot2 · readr · stringr · scales

## The scenario
A CEO wants to hire a full-time data scientist who could later lead a team. Salaries vary widely around the world and the market is competitive, so the CEO asked for a salary range that will attract top talent, and for the difference between a US-based and an offshore hire. The final product is a presentation for a non-technical audience.

## Data
`r project data.csv`: 607 data-science salary records from 2020–2022. Each record has work year, experience level (entry, mid, senior, executive), employment type, job title, salary in USD, employee residence, remote ratio, company location and company size (small, medium, large).

## Approach
1. Filtered the records to data scientist roles.
2. Grouped employee residence into **United States** vs. **offshore**.
3. Split the data by company size (small, medium, large) and calculated the **average, minimum and maximum salary** by year, experience level and residence.
4. Visualized the results with ggplot2: average-salary charts faceted by experience level for each company size, plus a line chart of how average salaries changed over the years.
5. Turned the findings into a slide deck with salary-range tables for the CEO.

## Results
The presentation (`Comparing Data Scientist Salaries.pptx`) shows:
- Average data scientist salaries for small, medium and large companies, broken down by experience level and US vs. offshore residence
- Salary-range tables (minimum to maximum) by year and residence, which give the CEO a concrete range to offer
- How average salaries moved from 2020 to 2022

## Files
| File | What it is |
|---|---|
| `ertugrulturkseven_project_1.Rmd` | Analysis code (R Markdown) |
| `ertugrulturkseven_project_1.pdf` | Knitted report |
| `Comparing Data Scientist Salaries.pptx` | Presentation for the CEO |
| `Project Description-1.pdf` | Original project brief |
| `r project data.csv` | Dataset |

## How to run
Open `ertugrulturkseven_project_1.Rmd` in RStudio, point the data path to `r project data.csv`, and click **Knit**.

---
*Created by Ertugrul Turkseven, M.S. in Data Science, Merrimack College.*
