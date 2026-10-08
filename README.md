# TalentCore Workforce Analytics — Power BI Dashboard

An interactive 6-page Power BI dashboard analysing a 1,000-record employee dataset. Built as the capstone project of the Moringa School Data Analytics Programme (2026).

**Author:** Mohamed Mohamud Ahmed — medical student (MBChB), University of Nairobi

## What it answers
- How has headcount grown, and how do hires compare with exits each year?
- Where is attrition highest: by department, office, tenure, age band and performance rating?
- How are performance ratings and training hours distributed across departments?
- How does pay vary by department, role, education and management level, and are there gender pay gaps?

## Data
1,000 employee records (883 active, 117 departed), data as of 30 June 2025. Salaries are monthly gross figures in KES. Employee names in the detail table are anonymised placeholders.

## Selected findings
- Customer Support has the highest attrition (18.3%) and Human Resources the lowest (6.6%), about 2.8× higher.
- Attrition peaks in the 1–3 year tenure window (18.7%), against 3.2% for staff with 5+ years.
- Training hours show no relationship with performance rating (r = 0.03).
- Engineering pays 88% more than Customer Support on average, and management earns a 59% premium over individual contributors.
- Education level shows almost no pay premium (all four levels within about KES 4,400).

## Dashboard pages
| Page | Focus |
|---|---|
| Executive | Headline KPIs, headcount growth, hires vs exits, attrition by tenure and office |
| Workforce | Headcount by department and office, gender split, age, education, management vs individual contributors |
| Ratings | Performance ratings, share of high performers, training hours vs performance, drill-down explorer |
| Attrition | Departure trend, tenure "danger zone", attrition by office, performance, overtime and age band |
| Pay | Salary distribution, mean vs median, pay by department, management and education, gender pay by job role |
| Employee Detail | Record-level table with summary cards (reached by drill-through) |

## Technical approach
- **Power Query:** data cleaning and preparation
- **Data model:** a dedicated date table and a centralised measures table
- **DAX:** 20+ measures, including Attrition Rate, Gender Pay Gap %, High-Performer Attrition Rate, and time-intelligence headcount tracking
- **Design:** insight-led storytelling. Visual titles state the finding (for example, "Attrition Peaks in the 1–3 Year Window") instead of a generic label
- **Interactivity:** Year, Department and Office slicers, a page navigator, a Reset button and drill-down (including a drill-through to Employee Detail)

## Screenshots
![Executive](screenshots/01_executive.png)
![Workforce](screenshots/02_workforce.png)
![Ratings](screenshots/03_ratings.png)
![Attrition](screenshots/04_attrition.png)
![Pay](screenshots/05_pay.png)
![Employee Detail](screenshots/06_employee_detail.png)

## Files
- `TalentCore_Workforce_Analytics_Complete.pbix` — the Power BI report (open in Power BI Desktop)
- `screenshots/` — one image per dashboard page

## Contact
mohamed.m.ahmed946@gmail.com
