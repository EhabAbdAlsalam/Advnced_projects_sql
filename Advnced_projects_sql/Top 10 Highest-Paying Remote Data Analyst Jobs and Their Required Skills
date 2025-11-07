WITH HIGH_SALARY AS (
SELECT job_id,
       job_title_short,
       salary_year_avg,
       job_location,
       job_posted_date ::DATE

FROM job_postings_fact 

INNER JOIN company_dim ON job_postings_fact.company_id = company_dim.company_id
WHERE job_title_short = 'Data Analyst'
AND salary_year_avg IS NOT NULL
GROUP BY job_id
ORDER BY salary_year_avg DESC

LIMIT 1000
)

SELECT HIGH_SALARY.* , skills_dim.skills
FROM HIGH_SALARY
INNER JOIN skills_job_dim ON HIGH_SALARY.job_id = skills_job_dim.job_id
INNER JOIN skills_dim ON skills_job_dim.skill_id = skills_dim.skill_id
ORDER BY salary_year_avg DESC 


