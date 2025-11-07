💡 Project Purpose

In today’s data-driven job market, understanding the relationship between skills, salaries, and demand is essential for both job seekers and employers.
This project was designed to analyze real-world job posting data for Data Analyst roles using SQL — transforming raw data into actionable insights about:

Which technical skills command the highest salaries

Which are most in demand across remote opportunities

How skill combinations affect career growth and compensation

The goal is to showcase practical data analysis skills through clean, well-structured SQL queries and analytical reasoning.
It reflects the day-to-day work of a Junior Data Analyst who can extract insight, communicate clearly, and build visual dashboards that drive decision-making.

🧠 Data Analyst Job Market SQL Portfolio
🎯 Overview

This project explores the 2023–2024 Data Analyst job market using real job posting data.
Through SQL-based analysis, it uncovers insights about skill demand, salary trends, and remote work opportunities.
All findings are supported by reproducible SQL scripts and can be visualized in Power BI.

Tech Stack:
PostgreSQL · SQL · Power BI · GitHub

🧩 Data Model
Table	Description
job_postings_fact	Core dataset with job details (title, salary, location, benefits).
company_dim	Company information.
skills_dim	Skill names and categories.
skills_job_dim	Bridge table connecting jobs and skills.
🔍 Key SQL Analyses
1️⃣ Top-Paying Skills for Remote Data Analyst Roles

Objective:
Identify which technical skills yield the highest average salaries among remote Data Analyst roles.

Why It Matters:
This helps analysts prioritize high-value technical skills and guides HR teams when structuring salary benchmarks.

Query Explanation:
Joins job postings with skills, filters remote “Data Analyst” positions, calculates average yearly salary per skill,
and lists the top 25 paying skills.

Sample Insight:
“Advanced data engineering and cloud tools such as Snowflake, AWS, and Python show higher pay ranges compared to reporting skills like Excel or Power BI.”

2️⃣ Most In-Demand Skills for Remote Data Analyst Roles

Objective:
Determine which technical skills appear most frequently in remote Data Analyst job postings.

Why It Matters:
Reveals the core skills consistently required across remote positions,
helping professionals and employers align learning and recruitment priorities.

Query Explanation:
Counts skill occurrences in remote Data Analyst listings, grouping and ordering by demand count.

Sample Insight:
“Top five most requested skills for remote analysts: SQL, Excel, Python, Power BI, Tableau.”

3️⃣ High-Value Skills (Balancing Demand & Salary)

Objective:
Identify skills that balance high demand and high average salary in remote Data Analyst positions.

Why It Matters:
Distinguishes between skills that are simply popular and those that are both popular and lucrative — essential for career ROI planning.

Query Explanation:
Two CTEs measure demand and salary per skill;
the final query filters out low-frequency skills and orders by salary then demand.

Sample Insight:
“Skills like Python, AWS, and Snowflake appear moderately often yet command premium pay, showing strong return on learning investment.”

4️⃣ High-Paying Remote Data Analyst Roles with Key Skills

Objective:
Extract the ten highest-paying remote Data Analyst jobs and identify the technical skills attached to them.

Why It Matters:
Highlights which companies offer top salaries and what skillsets drive those earnings,
helping professionals target premium opportunities.

Query Explanation:
A CTE selects the top ten remote jobs by salary,
then joins skill tables to reveal required technical competencies.

Sample Insight:
“The highest-paid remote roles often come from global tech or analytics firms, combining SQL, Python, and cloud platform expertise with visualization tools like Power BI.”

📈 Power BI Dashboard

Visualizations include:

Salary distribution by country and skill

Skill demand frequency

Relationship between salary and benefits

Top remote employers

💡 Insights Summary

SQL, Python, and Power BI remain the backbone of data analytics hiring.

Cloud and automation skills significantly lift earning potential.

Remote roles offer on average 15–20 % higher salaries.

Companies providing health or remote benefits tend to require more technical versatility.

🚀 How to Use

Clone the repository.

Open SQL scripts from /SQL/ in your SQL environment.

Run queries against your dataset (or demo CSV).

Use Power BI to visualize and extend insights.

👤 Author

[Ehab Abdalsalam Mohammed]
📍 Cairo, Egypt
💼 Junior Data Analyst — SQL | Power BI | Data Visualization
📧 [ehababdalsalam46@gmail.com]
🔗 LinkedIn Profile

⭐ If you find this project valuable, please star the repo and share feedback!
