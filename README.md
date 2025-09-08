# Data Science Job Market Analysis

## Introduction

As someone preparing to transition into the data field, I’ve always wondered: what jobs pay the most, which skills are really in demand, and when do companies hire the most? This project explores the Data Science job market using real-world job posting data. The goal was to uncover insights into salaries, skills, and hiring trends and to practice building a full analysis pipeline in Excel.

Questions to Analyze

1. What’s the average salary by job title?
2. What are the top 10 in-demand skills?
3. Which skills command the highest pay?
4. When do companies hire the most?

## 🗃️ Data Preparation (ETL with Power Query)

I spent most of the time preparing the dataset in Power Query, following the ETL process:

## Extract:

- Appended multiple monthly job posting files into one dataset.

## Transform:

- Added an Index column for unique job IDs.

- Combined yearly and hourly salaries by converting hourly → yearly (hour_salary * 2080).

- Created a unified salary column with an if statement:

```
if [salary_year_avg] <> null 
   then [salary_year_avg] 
   else [salary_hour_adjusted]
```


- Ensured all data types were formatted correctly.

- Split the skills column into rows, allowing skill frequency analysis.

<img width="2858" height="1336" alt="image" src="https://github.com/user-attachments/assets/85c79268-c841-4fd0-b40c-8313e4d65c88" />

Load:

- Loaded the clean dataset back into Excel for analysis with PivotTables.

<img width="2756" height="1406" alt="image" src="https://github.com/user-attachments/assets/fe33d036-45ed-4bb0-a631-bbb8fbbb78c0" />
loaded the data and hid unecessary columns for efficiency

## 🔧 Excel Tools Used

- 📊 PivotTables

- 📈 PivotCharts

- 🔍 Power Query

- 🎛️ Slicers for interactivity


## 📊 Analysis
### 1️⃣ Salary by Job Title

- Data Scientists and Engineers showed higher average salaries compared to Analysts.

- Highlights pay gaps across roles.

<img width="1514" height="572" alt="image" src="https://github.com/user-attachments/assets/9fc007ea-0554-45b8-bf99-f29e853ffd13" />


## 2️⃣ Top 10 In-Demand Skills

- SQL, Python, and Excel dominate job postings.

- Confirms that core tools are the foundation of most roles.

<img width="1590" height="554" alt="image" src="https://github.com/user-attachments/assets/11365e19-3405-45b6-b12d-f35b3dc5b9e1" />


## 3️⃣ Highest-Paying Skills

- Some niche skills (e.g., Puppet, Solidity) appeared with very high salaries.

- Likely due to fewer postings, but sparks an interesting tradeoff: niche vs. core skills.

<img width="1632" height="644" alt="image" src="https://github.com/user-attachments/assets/2dacdc19-4882-4af9-87f2-0f2263629e0a" />



## 4️⃣ Hiring Trends Over Time

- Hiring peaks in August and January across most countries.

- Likely tied to budget cycles and new project launches.

<img width="1526" height="580" alt="image" src="https://github.com/user-attachments/assets/4ced218e-a9cc-4bf4-b0b4-235e5297a507" />

# Final Presentation

<img width="2220" height="1218" alt="image" src="https://github.com/user-attachments/assets/a40dda14-5a8f-4506-ac03-e5f61886e62f" />



# Conclusion

This project proves that with Excel alone — Power Query, PivotTables, and PivotCharts — you can turn raw job postings into meaningful career insights.

🔑 Key takeaways:

- 💵 Salaries differ widely by job title.

- 🛠️ SQL, Python, and Excel remain must-have skills.

- 💰 Niche skills sometimes bring higher pay, but less demand.

- 📅 Companies hire most in January and August.

Special thanks to Luke Barousse
 for the dataset and inspiration.


