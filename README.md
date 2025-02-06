# Streaming-Trends-Netflix

## Introduction

This project analyzes Netflix data, showcasing my EDA and presentation skills through data cleaning, modeling, and analysis to highlight key insights and KPIs. It includes predictive elements to address performance trends. The interactive dashboard ensures clarity for stakeholders.  
📌 Source: Kaggle | Tools: Excel, Power Query, Power BI

## Dataset Overview 📊  

The dataset consists of the following parameters:  

| Parameter      | Description |
|---------------|------------|
| **show_id**   | Unique identifier for the movie or TV show. |
| **type**      | Specifies whether it is a **Movie** or **TV Show**. |
| **title**     | Name of the program. |
| **director**  | Director responsible for the production (applicable only to movies). |
| **cast**      | Main cast members. |
| **date_added** | Date when the program was added to Netflix. |
| **release_year** | Year the program was released. |
| **rating**    | Age-based content classification. |
| **duration**  | Number of seasons (for TV shows) or runtime in minutes (for movies). |
| **listed_in** | Genre classification of the program. |
| **description** | A brief summary of the program. |

## Objective 🎯  

This project aims to create a **personalized dashboard** for the client, highlighting key **insights** through **exploratory data analysis (EDA), data modeling, and visualization**. The dashboard is designed to be **insightful, interactive, and aligned with the company's color palette** for a seamless experience.  

### Key Objectives:  
- 📌 **Analyze genre distribution** across Netflix content.  
- 🌎 **Identify top content-producing countries** on the platform.  
- 📊 **Determine the most popular content types** produced and consumed globally.  
- 🎭 **Examine movie ratings** and their distribution.  
- 📅 **Track year-wise content addition trends** to understand growth patterns.

## Development ⚙️  

### **1️⃣ Data Import & Profiling**  
- Imported the dataset into the **working environment** for analysis.  
- Ensured data readiness for **cleaning, manipulation, and exploration**.  

### **2️⃣ Data Cleaning & Handling Missing Values**  
- The dataset contained **inconsistent data, blank cells, and duplicates**, requiring **profiling and cleaning**.  
- **Missing director names** were replaced with `"Unknown Director"` to facilitate analysis.  
- **Blank country values** were filled with `"United States"` as it contributes the majority of content.  
- **Date inconsistencies** were resolved by **changing the locale type** for uniform formatting.  

### **3️⃣ Duration Column Standardization**  
- Movies have duration in **minutes**, while TV shows use **seasons**.  
- Created a **conditional column**:  
  - Movies retain duration in minutes.  
  - TV shows have `"null"` for consistency in analysis.  

### **4️⃣ Text Formatting for Better Analysis**  
- Converted **description & director fields** to **lowercase** to improve data processing.  

### **5️⃣ Genre Classification & Filtering**  
- Added a **conditional column** to identify **Murder Mystery** content by detecting keywords like:  
  - *"kill"*, *"death"*, *"assassinate"*.  
- Filtered the dataset to **include only records from the year 2000 onward**, ensuring relevance.  
- Excluded non-essential columns (e.g., **description**) for a **cleaner, optimized dashboard**.  

### **6️⃣ Multi-Genre Handling & Category Mapping**  
- Since each title belongs to **multiple genres**, we created a separate **"Category Mapping 1" query**:  
  - **Split the "listed_in" column** to map genres individually.  
  - Allowed better analysis of **total genre count and distribution**.

 ## Key Findings & Insights 📊  

### **1️⃣ Quick Insights at a Glance**  
- 🎬 **Movies make up 68%** of the content, while **TV shows account for 32%**.  
- 🎭 **Total number of genres:** 42.  
- 📌 **Total number of titles:** 8,278 (since 2000).  
- 📅 **Peak content additions:** 2017-2018.  

### **2️⃣ Key Insights & Trends**  
- 🎞️ **Top 3 genres:** *International, Dramas, and Comedies*, with **International** being a mixed-genre category.  
- 🔞 **Most common ratings:** **TV-MA** (mature audiences) and **TV-14** lead the classification.  
- 🌍 **Top content-producing countries:**  
  - 🇺🇸 **United States** (40% of all content).  
  - 🇮🇳 **India** (~10%) and 🇬🇧 **UK** (~5%).  
- 📺 **Japan & South Korea produce more TV shows** than movies, focusing on **Anime & International TV**.  
- 📈 **Content growth trend:**  
  - **Sharp rise** in TV shows & movies from **2015 to 2018**.  
  - **Sudden decline after 2020**, likely due to the **COVID-19 pandemic**.  
  - **2018 saw the highest number of content releases**.  

## Project Summary

In this project, we’ve uncovered the power of data-driven insights into Netflix's content strategy, audience preferences, and overall platform performance. Using a strong ETL (Extract, Transform, Load) process, we transformed raw data into something clean, structured, and ready to reveal some hidden gems. 🔍✨

The analysis shows that movies reign supreme on Netflix, with 68% of the content being film-related, while TV shows make up 32%. The U.S., India, and the U.K. are the big players in content production, but Japan and South Korea are throwing down some serious TV show content, particularly in the Anime and International TV genres. 🍿 As for audience ratings, Netflix is definitely catering to a mature crowd, with most titles falling under TV-MA and TV-14. Looks like it’s drama o’clock! 🎭

When it comes to trends, we saw a significant increase in production from 2015 to 2018, followed by a notable dip post-2020—likely due to the COVID-19 pandemic and the industry's shifting landscape. But not to worry, Netflix is still pushing forward! And with our data enrichment techniques, like genre-based filtering and keyword classifications (shoutout to the murder mysteries 🕵️‍♂️🔪), we’ve found some cool ways to refine content categorization and improve recommendations.

The final interactive dashboard provides a smooth, dynamic way to explore these insights, allowing stakeholders to dive into key metrics, trends, and parameters at their fingertips. 📊

### LinkedIn post

https://www.linkedin.com/posts/kartik-zingade-90227a1a6_netflix-dataanalytics-powerbi-activity-7292608995377172480-fX_7?utm_source=share&utm_medium=member_desktop



### What's Next?

While we’ve gathered some solid insights, there’s still plenty more to explore. Future analysis could dive deeper into viewer engagement, content recommendation algorithms, and regional performance trends to further enhance Netflix's content optimization. The journey doesn’t stop here! 🚀🍿

 


    

