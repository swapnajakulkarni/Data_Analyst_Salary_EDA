# Project overview
  Business user of Staffing and Recruiting Company in Data Analytics sector intrested to discover <b>"Revenue forecating" .
  Estimate their future income they wants to know the insights ,tends and patterns from available data collected from various sources.</b>

  To do this,As a Data Analyst ,we need to analyze the past data and plan their budget ,resources and strategies for their growth in upcoming year.

## Table of content
-  Project structure
-  Data sources
-  Installation
-  Usage
-  Analysis
-  Result
-  Recommendations
-  Contribution
-  License
-  Limitations

  
## Project Structure
   We aims to achieve the following from this data
    - which job title was in demand from last few years?
    - what category is highly paid last year?
    - which location demand most number of resources?
    - which location/job title gives more revenue?
##  Data Sources
    - Data file/Input sources
        - kaggle Dataset
    -  Tools
        -  Microsoft Excel
        -  Python
        -  Pandas,seaborn,matplotlib Libraries
        -  SQL server
        -  Tableau
##  Data cleaning and Prepration
        -  Data Loading and Inspection
        -  Handling Missing Values
        -  Data Cleaning & Formatting
## Exploratory Data Analysis
        I performed EDA to answer important questions like
        - What is overall profit?
        - Which are top five category openings was in market?
        - What is peak time peroide?
## Data Analysis
  
      code 
      Jobcategory_yearcount = df.groupby('work_year').agg({'job_category':'count'})
      job_categoryTop5count=df['job_category'].value_counts()[:5]
      job_categoryTop5count

      JobTitle_sal=df.groupby('job_title')['salary_in_usd'].mean()
      Top10JobTitle_sal=JobTitle_sal.sort_values(ascending=False)
      key=Top10JobTitle_sal[::10].keys()
      val=Top10JobTitle_sal[::10].values
      Top10JobTitle_sal

      salaryby_loc = df.groupby('company_location')['salary_in_usd'].mean().reset_index()
      salaryby_loc



      Visulations : Matplotlib 
      Top10JobTitle_sal=Top10JobTitle_sal[::10]
      fig=plt.figure(figsize=(8,5))
      sns.barplot(x=key, y=val)
      plt.xticks(rotation=75)
      plt.title("Top 10 highest paid Job Title ")
      fig.show()
## Result /Findings


       

        -
    
