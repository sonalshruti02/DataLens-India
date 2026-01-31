# DataLens-India
Welcome to DataLens India , focusing on data analyst roles. This project was created out of a desire to navigate and understand the job market more effectively. It delves into the top-paying and in-demand skills to help find optimal job opportunities for data analysts.  The data sourced is from Luke Barousse's Python Course .


# Overview
Welcome to my analysis of the data job market, focusing on data analyst roles. This project was created out of a desire to navigate and understand the job market more effectively. It delves into the top-paying and in-demand skills to help find optimal job opportunities for data analysts.

The data sourced from Luke Barousse's Python Course which provides a foundation for my analysis, containing detailed information on job titles, salaries, locations, and essential skills. Through a series of Python scripts, I explore key questions such as the most demanded skills, salary trends, and the intersection of demand and salary in data analytics.


# The Questions
Below are the questions I want to answer in my project:

# 1 What are the skills most in demand for the top 3 most popular data roles?
# 2 How are in-demand skills trending for Data Analysts?
# 3 How well do jobs and skills pay for Data Analysts?
# 4 What are the optimal skills for data analysts to learn? (High Demand AND High Paying)


# Objectives

Analyze job availability trends across years
Identify top hiring locations in India
Discover most in-demand skills in the data domain
Understand role distribution (Data Analyst, Data Scientist, etc.)
Highlight top companies hiring for data roles
Study salary patterns and experience demand


# Tools I Used
For my deep dive into the data analyst job market, I harnessed the power of several key tools.
Python: The backbone of my analysis, allowing me to analyze the data and find critical insights.I also used the following Python libraries:
Pandas Library: This was used to analyze the data.
Matplotlib Library: I visualized the data.
Seaborn Library: Helped me create more advanced visuals.
Jupyter Notebooks: The tool I used to run my Python scripts which let me easily include my notes and analysis.
Visual Studio Code: My go-to for executing my Python scripts.
Git & GitHub: Essential for version control and sharing my Python code and analysis, ensuring collaboration and project tracking.


# Data Preparation and Cleanup
This section outlines the steps taken to prepare the data for analysis, ensuring accuracy and usability.

# Import & Clean Up Data
I started by importing necessary libraries and loading the dataset, followed by initial data cleaning tasks to ensure data quality.

# Importing Libraries
import ast
import pandas as pd
import seaborn as sns
from datasets import load_dataset
import matplotlib.pyplot as plt  

# Loading Data
dataset = load_dataset('lukebarousse/data_jobs')
df = dataset['train'].to_pandas()

# Data Cleanup
df['job_posted_date'] = pd.to_datetime(df['job_posted_date'])
df['job_skills'] = df['job_skills'].apply(lambda x: ast.literal_eval(x) if pd.notna(x) else x)
Filter US Jobs
To focus my analysis on the U.S. job market, I apply filters to the dataset, narrowing down to roles based in the United States.

df_India = df[df['job_country'] == 'India']
The Analysis
Each Jupyter notebook for this project aimed at investigating specific aspects of the data job market. Here’s how I approached each question:

# 📈 Key Insights from Data Analysis

# 1️⃣ Job Trends Over the Years (2019–2023)

Job postings declined during 2020, indicating the impact of COVID-19.
A strong recovery is observed from 2021 onwards.
2022–2023 show the highest demand, reflecting rapid digital transformation and data adoption.
📌 Insight: The data domain has become recession-resilient in recent years.

# 2️⃣ Top Hiring Locations in India

Bangalore leads as the largest hub for data jobs.
Hyderabad, Pune, Mumbai, and Delhi NCR follow closely.
Tier-2 cities are gradually emerging but still contribute a smaller share.
📌 Insight: Metro cities dominate due to strong IT ecosystems and startup presence.

# 3️⃣ Most In-Demand Data Skills

SQL and Python appear in the majority of job postings.
Excel remains essential despite advanced tools.
Machine Learning, Power BI, Tableau, and Statistics are highly valued.
Cloud and big-data skills show increasing demand.
📌 Insight: Strong fundamentals + visualization tools = maximum employability.

# 4️⃣ Role Distribution in the Data Domain
Data Analyst roles form the largest share.
Data Scientist and Business Analyst roles follow.
Specialized roles like ML Engineer have fewer openings but higher skill requirements.
📌 Insight: Entry-level opportunities are highest in Data Analyst roles.

# 5️⃣ Top Hiring Companies
IT giants and MNCs dominate hiring.
Product-based companies and startups are increasingly hiring data professionals.
Consulting and analytics firms show consistent demand.
📌 Insight: Data roles are no longer limited to tech companies—every industry needs data.

# 6️⃣ Experience vs Job Demand

Majority of jobs require 0–3 years of experience.
Mid-level roles (3–5 years) are the second largest segment.
Senior roles have fewer but more specialized openings.
📌 Insight: The market is highly favorable for freshers and early-career professionals.

# 7️⃣ Salary Insights (If Analyzed)

Entry-level salaries show steady growth over the years.
Higher salaries are strongly linked to advanced skills and experience.
Metro cities offer better compensation on average.
📌 Insight: Upskilling directly impacts earning potential.


# What I Learned

Throughout this project, I deepened my understanding of the data analyst job market and enhanced my technical skills in Python, especially in data manipulation and visualization. Here are a few specific things I learned:

Advanced Python Usage: Utilizing libraries such as Pandas for data manipulation, Seaborn and Matplotlib for data visualization, and other libraries helped me perform complex data analysis tasks more efficiently.
Data Cleaning Importance: I learned that thorough data cleaning and preparation are crucial before any analysis can be conducted, ensuring the accuracy of insights derived from the data.
Strategic Skill Analysis: The project emphasized the importance of aligning one's skills with market demand. Understanding the relationship between skill demand, salary, and job availability allows for more strategic career planning in the tech industry.

# Insights

This project provided several general insights into the data job market for analysts:

1 The Indian data job market is growing rapidly and shows long-term stability.
2 Mastering SQL, Python, Excel, and visualization tools is crucial.
3 Location still plays a key role, but remote and hybrid opportunities are rising.
4 This analysis can guide career planning, skill selection, and placement preparation.

# Challenges I Faced


This project was not without its challenges, but it provided good learning opportunities:

Data Inconsistencies: Handling missing or inconsistent data entries requires careful consideration and thorough data-cleaning techniques to ensure the integrity of the analysis.
Complex Data Visualization: Designing effective visual representations of complex datasets was challenging but critical for conveying insights clearly and compellingly.
Balancing Breadth and Depth: Deciding how deeply to dive into each analysis while maintaining a broad overview of the data landscape required constant balancing to ensure comprehensive coverage without getting lost in details.


# Conclusion

This exploration into the data analyst job market has been incredibly informative, highlighting the critical skills and trends that shape this evolving field. The insights I got enhance my understanding and provide actionable guidance for anyone looking to advance their career in data analytics. As the market continues to change, ongoing analysis will be essential to stay ahead in data analytics. This project is a good foundation for future explorations and underscores the importance of continuous learning and adaptation in the data field.


# 👩‍💻 Author

Sonal Shruti
B.Tech | Data Analytics Enthusiast
📍 Noida , India
