# Accenture-Data-Analytics
social buzz data analtics project
## Project Overview  
This project focuses on analyzing the data practices of Social Buzz, a fast-growing technology unicorn, to uncover actionable insights that can enhance user engagement and support the company’s preparation for a successful IPO. Over three months, we conducted an audit of Social Buzz's big data processes, analyzed its vast content database, and provided recommendations for leveraging data-driven strategies.  

## Objectives  
1. Audit Big Data Practices: Evaluate Social Buzz’s existing data management systems and processes.  
2. IPO Readiness: Develop insights and recommendations to ensure data capabilities align with IPO goals.  
3. Content Analysis: Identify the top five most popular content categories to guide future marketing and engagement strategies.  

## Problem Statement  
Social Buzz generates over 100,000 posts daily, resulting in an overwhelming 36.5 million pieces of content per year. This massive data volume poses challenges in identifying key trends and capitalizing on them effectively. The objective was to determine how Social Buzz can utilize its data for real-time decision-making and increased user engagement.  

## Analytics Team  
- Andrew Fleming: Chief Technical Architect  
- Marcus Rompton: Senior Principal  
- Yogesh: Data Analyst  

## Project Workflow  
The project was executed in five key steps:  
### 1. Data Understanding: Gaining a comprehensive view of the data structure and scope.
the first step is to use this data model to identify which datasets will be required to answer your business question - which is to to figure out the top 5 categories with the largest popularity.
#### Definitions of different data types:

- String - Sequence of characters, digits, or symbols—always treated as text,
- UUID - Universally Unique Identifiers,
- Array - List with a number of elements in a specific order—typically of the same type,
- Integer - Numeric data type for numbers without fractions,
- Timestamp - Number of seconds that have elapsed since midnight (00:00:00 UTC), 1st January 1970 (Unix time),
### 2. Data Cleaning: Ensuring data accuracy and consistency for meaningful analysis.
- removing rows that have values which are missing,
- changing the data type of some values within a column, and
- removing columns which are not relevant to this task
- CLICK THIS LINK FOR :![DATA MODEL.PDF](https://github.com/yogeshwaran03/Accenture-Data-Analytics/blob/4b92f1a3ebe215d6878f8c72c93ab0d912a940d6/Data%20model/Data%20model.pdf)
### 3. Data Modeling: Building models to identify patterns and trends.
1. Merge the Data: We start by merging the three provided data sets using the Reaction table as the base and joining the relevant columns from the Content and Reaction Types tables.
-  To perform the merge:
   You can use a VLOOKUP formula in Excel or an equivalent operation in your chosen data processing tool to combine the tables based on a common key (such as Reaction ID or Content ID). Eg: =VLOOKUP(Reaction_ID, Content, 2, FALSE)
3. Calculate Total Scores: Next, we aggregate the scores for each category using the SUMIF formula to calculate the total score for each category. Eg: =SUMIF(Category_Range, Category_ID, Score_Range) 
4. Identify the Top 5 Categories: Finally, we identify the top 5 categories based on the total scores.
The result of this process is a cleaned dataset containing the merged data and the top 5 categories with the highest scores.
### 4. Data Analysis: Performing in-depth analysis to uncover insights.  
### 5. Insights Extraction: Delivering actionable insights and recommendations.  

## Insights and Findings  
1. Unique Categories: We identified 16 distinct categories of content.  
2. Peak Activity Month: January recorded the highest volume of posts.  
3. Engagement Trends: Content related to animals garnered significant reactions.  
4. Top Categories by Popularity:  
   - Healthy Eating emerged as the most popular category, indicating a strong interest in health-related content among users.  
5. Actionable Insight: These findings suggest an opportunity for Social Buzz to collaborate with health-focused brands to create targeted campaigns and boost engagement.  

## Recommendations  
- Real-Time Analytics: Transition the current ad-hoc analysis to a large-scale, production-ready system for continuous, real-time insights.  
- Strategic Campaigns: Leverage insights to design campaigns around popular themes, such as healthy eating, to align with audience interests.  

## Next Steps  
To implement the recommendations, Social Buzz can adopt advanced analytics tools and real-time data pipelines, enabling faster decision-making and deeper engagement strategies.  

## Conclusion  
This project demonstrates the potential of leveraging big data to drive business success. By scaling the insights into real-time systems, Social Buzz can position itself as a leader in data-driven engagement, achieving its business goals while preparing for its IPO.  
