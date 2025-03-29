
# DATA SCIENCE JOBS ANALYTICS DASHBOARD




https://github.com/user-attachments/assets/b62e9eac-11e8-4f52-bcae-b9cbfee9dbd7



## Introduction
This data jobs salary dashboard was created to help job seekers investigate salaries for their desired jobs and ensure they are being adequately compensated.

The dataset is from survey which was done back in 2023, which provides a foundation in analyzing data using this powerful tool. The data contains detailed information on job titles, salaries, locations, and essential skills that are presented here.

## Dashboard 
The Dashboard can be used by downloading the Excel file from the link https://github.com/Gitika-26/Data-Science-Job-Insights/blob/main/project_copy.xlsx

## Excel Skill Used
- **📉 Charts**
- **🧮 Formulas and Functions**
- **❎ Data Validation**

## About the Dataset
The dataset used for this project contains real-world data science job information from 2023. The dataset is available via within the hidden workbook of the Excel file, which provides a foundation for analyzing data using Excel. It includes detailed information on:

- **👨‍💼 Job titles**
- **💰 Salaries**
- **📍 Locations**
- **🛠️ Skills**
  
![image](https://github.com/user-attachments/assets/8f85b1d9-ec74-4af6-9f65-9765431f6a44)


## Dashboard Build

### 📊 Data Science Job Salaries - Bar Chart
![Screenshot 2025-03-29 213926](https://github.com/user-attachments/assets/a953d19d-9b1d-4b78-a0a8-8ed0101159b2)

- 🛠️ **Excel Features:** Utilized bar chart feature (with formatted salary values) and optimized layout for clarity.
- 🎨 **Design Choice:** Horizontal bar chart for visual comparison of median salaries.
- 📉 **Data Organization:** Sorted job titles by descending salary for improved readability.
- 💡 **Insights Gained:** This enables quick identification of salary trends, noting that Senior roles and Engineers are higher-paying than Analyst roles.

### 🗺️ Country Median Salaries - Map Chart
![Screenshot 2025-03-29 214130](https://github.com/user-attachments/assets/a085c37a-e9d6-4d0a-b88b-9c6d3e304eea)

- 🛠️ **Excel Features:** Utilized bar chart feature (with formatted salary values) and optimized layout for clarity.
- 🎨 **Design Choice:** Horizontal bar chart for visual comparison of median salaries.
- 📉 **Data Organization:** Sorted job titles by descending salary for improved readability.
- 💡 **Insights Gained:** This enables quick identification of salary trends, noting that Senior roles and Engineers are higher-paying than Analyst roles.

### 🗺️ Salary With Respect to Job Type - Histogram
![Screenshot 2025-03-29 214145](https://github.com/user-attachments/assets/c063ba3e-24f5-4b12-90c1-d839fe13d5a1)

###  🧮 Formulas and Functions
My data science job dashboard uses the following functions to clean the data and present it visually:

COUNTIFS – Used to count jobs with the required conditions (job title, country, and job type).

FILTER – Used to filter the required data for funding platforms.

SEARCH – Used to find job type since a single job title may have different job types offered.

XLOOKUP – Used to find the required data based on ranges.

Example - Finding Median based on the said job title, country and job type

```
=MEDIAN(
IF(
    (jobs[job_title_short]=A2)*
    (jobs[job_country]=country)*
    (ISNUMBER(SEARCH(type,jobs[job_schedule_type])))*
    (jobs[salary_year_avg]<>0),
    jobs[salary_year_avg]
)
)
```

- 🔍 **Multi-Criteria Filtering:** Checks job title, country, schedule type, and excludes blank salaries.
- 📊 **Array Formula:** Utilizes `MEDIAN()` function with nested `IF()` statement to analyze an array.
- 🎯 **Tailored Insights:** Provides specific salary information for job titles, regions, and schedule types.
- **🔢 Formula Purpose:** This formula populates the table below, returning the median salary based on job title, country, and type specified.

## The Background Filtering
All the formulas and data validation used can be found in the Excel sheet by unhiding the hidden data and formula workbooks. They have been hidden for the convinience of stakeholders and to prevent any discrepancies.
![image](https://github.com/user-attachments/assets/316fcded-912f-4992-bd3a-cc136ea57c55)




## Conclusion
I created this dashboard to showcase insights into salary trends across various data-related job titles. Utilizing the dataset, this dashboard allows users to make informed decisions about their career paths. Exploring the functionalities to understand how location and job type influence salaries. 



