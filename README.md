# Preparing Students
Are schools preparing students for life after high school?  I break down data on if schools are effectively teaching students and preparing them to be successful after graduation.

# Project Overview
The objective of this project is to take a look at how effective schools are in Kentucky and if they are preparing students after graduation.  Important factors in which schools are measured on are the Kentucky State Assessments, Postsecondary Readiness (college readiness benchmarks, career certifications), and Graduation Rate from the 2023-2024 KSA School Report Card Data.

# Project Setup Instructions
In order to run this project:

1. Clone the repository.
2. Save the Folder.
3. Run pip install -r requirements.txt
4. Open Jupyter Notebook from the command line or start menu.
5. Go to the where you saved the notebook.
6. Open 'School_Data.ipynb'
7. Click Run All.


# Data Sources
Data in this project comes from the Kentucky Department of Education
https://kdeschoolreportcard.blob.core.windows.net/datasets/KYRC24_ACCT_Profile.csv

and 

https://kdeschoolreportcard.blob.core.windows.net/datasets/KYRC24_SAFE_Behavior_Events_by_Grade_Level.csv


# Technologies Used
The project was developed using Jupyter Notebooks for a clean and organized presentation of the code.  Pandas was used to narrow down the data set.  I needed to focus on 'All Students' for only the high schools.  I created some functions for us to search for more specific school data and results.  Tables and visualizations were created using numpy, and matplotlib.

# Data Dictionary
Grade 9/10/11/12 - total number of behavior events 

Graduation Status - Percent of students who graduated in 4 years / total number of students in the original cohort

Kentucky State Assessment (KSA) - Given to students in certain content subjects at the end of the year to measure student literacy and numeracy progress towards the academic standards.

Level - Elementary (K-5), Middle (6-8), or High (9-12)

Overall Combined Indicator Rate - Overall school score calculating Reading/Math, Science/Social Studies/Writing, Postsecondary Readiness, Quality of School Climate, and Graduation statuses.  

Postsecondary Status - Percent of students who met either a college readiness benchmark or career readiness benchmark / total number of students in the original cohort.

Reading Math Status - Schools receive points based on how students score on the KSA.  Novice = 0 points, Apprentice = 0.5 points, Proficient = 1.0 points, and Distinguised = 1.5 points.  It is calculated by the number of points scored and total number of students who were elegible to take the test.

Reading Math Status Rating - Based on a five point scale from the Reading Math results in the KSA.

State School ID - Nine digit identifier used for federal reporting

# Data Summary
As expected, we see an even distribution in KSA Reading and Math results with about 67% of schools earning a rating of 3 or higher. Ratings are determined by the percentage of students who are Proficient/Distinguished in the content areas.  

We see a more even distribution of schools earning a rating of 2, 3, or 4 from KSA Science, Social Studies, and Combined Writing Ratings. We should note the Writing Test is scored by a hand, which offers more varying results in scoring.  

I compared the correlation data between the KSA Reading/Math scores with graduation rate across schools. There is a positive correlation in overall school scores and graduation rate.

I also gathered the correlation between post secondary readiness with graduation rate.  Again, there is a positive correlation within the data.  We see a closer 1:1 correlation between this set of data.  

# Project Summary
As stated above, we see an expected bell curve of results in school ratings for the Reading/Math tests.  This is a normal distribution of results.  

While we see a positive correlation in the Reading/Math scores and graduation rate, I am concered on the number of schools that scored in the range of 55 - 65 that also graduated at least 90% of the senior level class.  This is saying that about 60% of students are demonstrating proficiency or higher in Reading and Math but are still earning enough passing credits to graduate.  There are a number of factors to consider why the scores are low (poor test taking, low student input in the tests, lack of instructional expectation, emphasis to move students along).

There was also a positive correlation in the Postsecondary Readiness and Graduation Rate data.  Students are college ready if they meet the expected benchmark score on either English, Math, OR Reading (only needs to meet one of three benchmarks).  Students are career ready if they complete at least two credits in a pathway AND completed a certification test.  It is positive to see that schools are scoring higher in the postsecondary readiness scores.  Although, students who are college bound only need to meet the benchmark in one of three subjects is concerning.

Through the function, I found that only 5 out of 228 high schools scored an overall indicator rating of 90 or higher.  
