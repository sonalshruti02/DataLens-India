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


# 📈 Analysis & Insights

# 1️⃣ Most In-Demand Skills for Top Data Roles in India

This analysis identifies the top skills required for the most popular data roles such as:
Data Analyst
Data Scientist
Data Engineer
Key Insights:

SQL is the most frequently requested skill across all data roles.
Python shows strong demand, especially for Data Scientist and Data Engineer roles.
Excel remains highly relevant in Data Analyst positions.
Data Engineer roles demand more specialized tools such as cloud platforms and big data technologies.

📌 Insight:
Core skills like SQL and Python form the foundation of most data roles in India, while advanced tools differentiate senior positions.

# 2️⃣ Skill Demand Trends for Data Analysts in India

Skill trends were analyzed over time to understand how requirements evolve.
Key Insights:
SQL remains consistently in demand across years.
Excel shows renewed importance, particularly in business-focused roles.
Python and visualization tools (Power BI / Tableau) maintain steady demand.
Visualization tools show gradual growth, reflecting the rise of data-driven decision-making.

📌 Insight:
The Indian market values both technical analysis and business reporting skills.

# 3️⃣ Salary Analysis of Data Roles in India

Salary distributions were analyzed across common data job titles.
Key Insights:
Senior roles command significantly higher salaries.
Data Analyst roles show more consistent salary ranges compared to specialized roles.
Higher salaries are closely linked to experience + advanced skill sets.

📌 Insight:
Specialization and seniority play a major role in salary growth in India.

# 4️⃣ Highest-Paid vs Most In-Demand Skills (India)

This section compares:
Most demanded skills
Highest paying skills
Key Insights:
Foundational skills (SQL, Excel) are highly demanded but offer moderate salaries.
Specialized tools and technologies offer higher pay but appear in fewer postings.
There is a clear gap between employability skills and premium skills.

📌 Insight:
Career growth requires a balance between demand-driven and salary-driven skills.

# 5️⃣ Optimal Skills to Learn for Data Analysts in India

Optimal skills were identified based on:
Skill demand percentage
Median salary
Key Insights:
Skills like Python, SQL, Tableau, and Power BI offer strong demand and competitive pay.
Specialized database and programming skills show high salary potential.
Visualization and programming skills together create strong career leverage.

📌 Insight:
Candidates who combine core analytics skills with advanced tools maximize job opportunities.


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
📍 India IN
