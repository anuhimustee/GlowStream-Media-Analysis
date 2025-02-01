# GlowStream Media Entertainment Analysis

## Introduction

Truth be told, Netflix is one of the biggest streaming platforms out there and they are really making big waves and massive moves. Not just that, the entertainment industry is constantly growing and the most interesting is that data (unprocessed information)
as I like to call it) plays a crucial role in decision-making. 
In this project, I assumed the role of a Data Analyst at GlowStream Media, a private entertainment company planning to launch a new show by analyzing the trends and performance of blockbuster movies from 2015-2023.
Unlike typical movies review shows, GlowStream wants to avoid subjective opinions and focus on data-driven insights. They aim to explore themes like box office performance, audience demographics, critical receptions, and streaming platform popularity.

> **_Disclaimer:_** All datasets and reports do not represent any company, institution or country, the datasets are part of a capstone project in Data Analysis with TechCruh Africa 
> For this project, some numbers of questions were answered using Excel analysis features like pivot table, conditional formatting, etc

### Project Overview

**GlowStream Media** is a private entertainment company planning to launch a new show **analyzing the trends and performance of blockbuster movies** from 2015 to 2023. Unlike typical movie review shows, GlowStream wants to avoid subjective opinions and focus on **data-driven insights**. They aim to explore themes like **box office performance**, **audience demographics**, **critical reception**, and **streaming platform** popularity.
Here, I assumed the role of a data analyst at GlowStream Media, and my task is to generate meaningful insights using historical movie data.
Since this analysis could influence future content strategies, I am to collaborate with the manager, Mr Emmanuel Ehosa, who has provided a list of questions (which are problem statements also and what they are seeking insights into) to guide my analysis.
My final report or insight will be delivered to GlowStream's Chief Content Officer, Ndidi Chigozie, who values storytelling, clear visuals, and concise insights. 

### Objective
Fundamentally, GlowStream Media aims to launch a unique movie analysis show based purely on data-driven insights rather than subjective reviews. 
Therefore, in this project, my aim is to explore trends in blockbuster movies from 2015 to 2023, providing valuable insights into factors influencing box office success and audience engagement. 
In analyzing any data, the first and the most important aspect is to carefully, strategically & analytically understand the objects and the end goal. 

### About the Dataset:
The dataset used for this project was of a three (3) different table data structure that was used for this analysis. Each of these dataset table structure brief information is outlined below 

Three datasets were used for analysis:

1.	**Movie Box Office Data-:** Contains a total record of 423 (_Before Cleaning/Analysis_) and 8 fields including; movie details, box office revenue, production budget, genre, etc.
Here is a Snapshot of the raw dataset.

<p align="center">
  <img width="624" height="622" src="https://github.com/anuhimustee/GlowStream-Media-Analysis/blob/main/ReadMe%20Images/Dataset%201.png">
</p>
  
Click [here](https://github.com/anuhimustee/GlowStream-Media-Analysis/blob/main/ReadMe%20Images/movie_box_office_data.csv) to access to the dataset

   
2. **Audience Demographics Data–:** Contains a total record of 501(_Before Cleaning/Analysis_) and has 6 fields namely audience age, gender, ratings, and preferred viewing platforms.

<p align="center">
  <img width="612" height="864" src="https://github.com/anuhimustee/GlowStream-Media-Analysis/blob/main/ReadMe%20Images/Dataset%202.png">
</p>
  
Click [here](https://github.com/anuhimustee/GlowStream-Media-Analysis/blob/main/ReadMe%20Images/audience_demographics_data.csv) to access to the dataset

3. **Critical Reviews Data –:** This dataset contains a total record of 401(___Before Cleaning/Analysis___) and has 6 fields which comprise of critic ratings, sources, review scores, etc.

<p align="center">
  <img width="624" height="717" src="https://github.com/anuhimustee/GlowStream-Media-Analysis/blob/main/ReadMe%20Images/Dataset%203.png">
</p>

Click [here](https://github.com/anuhimustee/GlowStream-Media-Analysis/blob/main/ReadMe%20Images/critical_reviews_data.csv)  to access to the dataset

Each dataset required cleaning due to issues like _missing values_, _inconsistent formatting_, _duplicate entries_, and _typos_.


## Problem Statement
Mr Emmanel Ehosa who is the manager at GlowStream Media has provided me with key questions to answer for my analysis. The answers to these questions are given birth of the problem statement and prospect that GlowStream intend to embark on which launch a new show. The answers to these questions will unlock a comprehensive insight into **trends and performance of blockbuster movies** from 2015-2023 based on the datasets provided. 

1.	What are the top 5 highest-grossing movies between 2015 and 2023? 
2.	Which genres have the highest average box office revenue? 
3.	What is the relationship between production budget and box office gross? 
4.	Which movies had the highest audience ratings on streaming platforms? 
5.	What age group gave the highest average ratings for each genre? 
6.	Are there any trends in box office performance over the years? 
7.	Which movies received the highest critical review scores? 
8.	What are the most popular viewing platforms for different genres? 
9.	How does audience gender distribution vary by genre? 
10.	Which directors have the highest average box office revenue?

## Concepts/Skills Demonstrated
The following Data Analysis Skill plus Excel features were incorporated during the run down of this project.
•	Data Importation: Importing multiple data into Excel
•	Data Cleaning (handling missing values, duplicates, formatting inconsistencies)
•	Data Transformation (restructuring datasets for better analysis)
•	Exploratory Data Analysis (EDA) (identifying trends, patterns, and anomalies)
•	Data Visualization (charts and graphs for insights presentation)
•	 Excel Pivot Table for Analysis
•	 Excel Interactive Dashboard Design

## Data Transformation/Cleaning
The raw dataset that was used for this analysis project was extremely dirty in the sense that  it affects the data integrity and accuracy altogether. These datasets contain high level of inconsistencies, duplicates, missing values and formatting issues that has to be cleaned before processing.

For the **First Dataset** which **Movie Box Office Data** (Check the __**image below**__ for a snapshot of the unclean dataset)
The **Underlying Issues** are: 
•	Inconsistent currency formatting. 
•	Typos in data entries (e.g., "20a7"). 
•	Missing values for some fields. 
•	Duplicate movie entries. 
•	Blank spaces in names. 



For the **Second Dataset** which is **Audience Demographic Data** (Check the **_image below_** for a snapshot of the unclean dataset)
The **Underlying Issues** are:
•	Inconsistent gender labels (e.g., "M", "Male"). 
•	Invalid Movie ID entries. 
•	Missing values for age and rating. 
•	Typos in Rating values. 
•	Inconsistent viewing of platform names. 


For the **Third Dataset Critical Reviews Data** (Check the **_image below_** for a snapshot of the unclean dataset)
The Underlying Issues are:
•	Inconsistent date formats. 
•	Missing critic names. 
•	Invalid dates (e.g., "2017-13-05"). 
•	Missing or incorrect review scores. 


## Data Cleaning Approach: 
The dirty data with its inaccuracies CANNOT be used for analysis just like that. It has to undergo some level of cleaning for it to be fit for analysis.
One of such approach to do this is using the Power Query Features in Excel. 

Through Power Query, Key issues with each dataset was addressed:
•	Standardized currency formatting in box office data
•	Fixed incorrect data entries (e.g., ‘20a7’ → ‘2017’ in release year)

**IMAGE!!!**

•	Handled missing values with appropriate imputation methods-( One of such method I used was to replace missing numeric values with the mean/average of the column).
For the categorical variables, for example, the missing values in **Gender**, **Directors** & **Lead Actor** were replaced with words like **“Others”**, **“Unknown”** respectively.

**IMAGE!!!**

•	Removed duplicate entries
•	Standardized audience demographics labels (‘M’, ‘Male’ → ‘Male’)

**IMAGE!!!**

•	Formatted inconsistent date formats

---

## Data Modelling

Fundamentally, as a data analyst, a comprehensive understanding of each dataset shows that there is or should be a relationship between the three datasets.
The datasets were structured in a relational format:
•	Movie Box Office Data (Primary Key: Movie ID)
•	Audience Demographics Data (Foreign Key: Movie ID)
•	Critical Reviews Data (Foreign Key: Movie ID)
The presence of these key columns as Primary and Foreign Key suggests a relationship and hence this was done through Power Pivot as shown in the image below.

|                                              Original Model                                        |                                         After Modelling                                              |
|----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------- |
| ![](https://github.com/anuhimustee/BSCo-Excel-Data-Analysis-Project/blob/main/Initial%20Model.png) | ![](https://github.com/anuhimustee/BSCo-Excel-Data-Analysis-Project/blob/main/ModellingComplete.png) |



## Data Analysis Insights
**1. Top 5 Highest-Grossing Movies**
The data reveals that **“Agree Wide Easy”** and **“Total Maybe May”** are the highest-grossing movies, generating box office revenues of **$1,990,610,982** and **$1,989,062,668**, respectively. These two films individually contribute the most to overall revenue. The chart below provides a visual representation of the top five highest-grossing movies.

**See the image below:**

**2. Highest Average Box Office Revenue by Genre:**
The genres with the highest average box office revenue are **Drama**, **Horror**, **Sci-Fi**, and **Romance**, in that order. This suggests that these genres attract larger audiences and generate higher ticket sales.

**See the image below:**

**3. Relationship Between Production Budgets and Box Office Revenue Over the Years**
Over the years, most movies, regardless of genre, have shown potential for box office growth. This trend is evident in the graph below.
•	The **blue curvy line** with white markers represents production budgets from 2015 to 2023.
•	The **top curvy line** indicates box office revenue, showing a fluctuating increase over time.
•	**2022 recorded the highest box office revenue growth**, reaching **$57 Billion**, making it the peak year in the observed period.

_This suggests that as production budgets increase, box office earnings tend to rise, highlighting the financial impact of investment in filmmaking._

**4. Movies with Highest Audience Ratings**


|               Military point           |   Top Ratings  | 
|----------------------------------------|----------------|
|           Risk specific treat          |       10       |
|           Page Establish               |       10       |
|           Article book company         |       10       |
|           Art heart provide as         |       10       |
|           Attorney south state         |       10       |
|           Nor second                   |       10       |
|           Church herself push house    |       10       |
|           Point strong account         |       10       |
|           Clearly court return         |       10       |
|           Wish here                    |       10       |
|           Customer pattern message     |       10       |
|           Fill edge                    |       10       |

## 5. Box office performance trends over the years? 
Over the years, most movies, regardless of genre, have shown potential for box office growth. This trend is evident in the graph below.
2022 recorded the highest box office revenue growth, reaching $57 billion, making it the peak year in the observed period.


## 6.	Popular View Platforms for Different Genres
•	Romance is predominantly watched in cinemas, significantly more than other genres.
•	Thrillers and Sci-Fi have high engagement on streaming platforms.
•	Comedy and Action are frequently downloaded, with Action also having notable DVD viewership.
•	Drama and Horror show a balanced distribution across all platforms.

This suggests that audience preferences vary by genre, influencing distribution strategies GlowStream Media

## 7.	Gender's Distribution by Genre?
**Men** predominantly watches movies through the services of Glowstream than Woman. However,**Men** predominantly **Action,** **Drama**, and **Comedy**, while **Women** mostly prefer **Romance**, **Thrillers**, and Comedy. This indicates that Comedy appeals to both genders, whereas Action and Romance have more distinct audience preferences. Interestingly, both genders have an equal viewing count for the Horror genre.

## 8.	Directors Box Office Average
The directors influence on revenue showed the top-grossing films can be linked to how well-known the directors were with their established reputations

---

## Recommendations

Based on the insights I will recommend the following to Glowstream Media;

**1.	Content Strategy:** 
- Gl
- owStream should prioritize **Drama**, **Romance**, **Comedy**, & **Horror** as they generate the highest revenue and audience engagement
- For each of these genre, Glowstream can target respective genders that shows a signifacent inclination toward their services. **Men** predominantly watch **Action**, **Drama**, and **Comedy**, while **"Women"** mostly prefer **Romance**, **Thrillers**, and **Comedy**. This indicates that Comedy appeals to both genders, whereas Action and Romance have more distinct audience preferences.
  
**2.	Marketing Focus:**
- Use data-driven marketing to target younger demographics on streaming platforms.
- Promote cinema releases more heavily to older audiences who prefer the theatrical experience.

**3.	Data-Driven Decision-Making:**
- Regularly track box office trends and audience preferences to refine content selection.
- Leverage audience insights to create customized promotions and improve engagement.

---

### Conclusion
This project has provided a solid foundation for GlowStream Media by leveraging effective data cleaning, modeling, and visualization.
The insights gained will support data-driven content strategies, ensuring that shows resonate with the target audience and enhance overall content performance.

<h2 style="text-align:center;">THANK YOU!🤝🤝🤝</h2>
