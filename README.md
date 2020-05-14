# SAT & ACT 2017/2018 Analysis #

## Problem Statement

For this project we seek to examine SAT and ACT score for both 2017 and 2018. We plan to identify trends and compare those trends against other states.

## Executive Summary

For the first time in 2017 Illinois provided free SAT test to 11th graders.
Average scores of schools ranged from 740 to 1300 in some schools. This shows the wide disparities that exist between the schools in the state of Illinois.

According to the Chicago Tribune, data supports the correlation between students taking the test in high-poverty neighborhoods and low scores and wealthy suburbs and higher scores.
Source: https://www.chicagotribune.com/news/breaking/ct-met-illinois-school-report-card-20171030-story.html


## Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|State|object|ACT/SAT|Every State including D.C.|
|act_participation_18|float|ACT|Percentage of students who took the ACT in 2018| 
|Composite_18|float|ACT|Composite score for the ACT in 2018| 
|sat_participation_18|float|SAT|Percentage of students of took the SAT in 2018| 
|sat_rw_18|int|SAT|SAT Reading and Writing score for 2018| 
|sat_math_18|int|SAT|SAT Math score for 2018| 
|sat_total_18|int|SAT|SAT total score for 2018| 
|act_participation_2017|float|ACT|% of students of took the ACT in 2017| 
|act_eng_2017|float|ACT|ACT English score in 2017|
|act_math_2017|float|ACT|ACT Math score in 2017| 
|act_reading_2017|float|ACT|ACT Reading score in 2017|
|act_sci_2017|float|ACT|ACT Science score in 2017| 
|Composite_2017|float|ACT|ACT Composite or Total score in 2017|
|sat_participation_2017|float|SAT|Percentage of students who took the SAT in 2017| 
|sat_rw_2017|int|SAT|SAT Reading and Writing in 2017|
|sat_math_2017|int|SAT|SAT Math score for 2017| 
|sat_total_2017|int|SAT|Total SAT score for 2017|


## Data Importing and Cleaning

We were given a dataset to start so all that was required was for me to import the CSV file. One of the first things I noticed about the dataset was the participation rate was showing as a object. What I did was create a function using indexing that only returns back the number and not the percentage sign and then convert to a numeric data type. I used this convert function on Composite as well as I noticed an 'x' was making the entire column return as an object. Next I used a dictionary to change the names of the columns so there is no confusion as to which column belongs to what year. After that using pandas merge I was able to combine the different dataframes. 

## Exploratory Data Analysis

An interesting finding in my EDA was hardly any scores proved the Central Limit Theorem correct. I believe this is because the differences in participation rates across the country on different tests. For example, some states require the ACT to graduate where other states don't resulting in different test scores because the sample size is different.


## Conclusions and Recommendations

One thing I found interesting was that the state of Illinois went from 2017 having a low SAT participation to 2018 having 100% participation in the SAT. This was a result of allowing free SAT tests. However, it also resulted in low SAT scores. This was to be expected as the sample size grew. After reading in more detail part of the reason was neighborhoods of lower socioeconmic backgrounds not having the resources to prepare for the test the same way.

College Board does not have to ability to change the socioeconomic background from which students come from
With state of Illinois now providing free SAT tests we may want to look into aid we can provide students to perform better on our tests. For example, snacks prior to test starting. Free resources available to students to improve test scores
Possibly look at other states who are performing well(taking Central Limit Theorem into account) like MA.

Source: https://www.chicagotribune.com/news/ct-illinois-chooses-sat-met-20160211-story.html
Source: https://www.chicagotribune.com/news/breaking/ct-met-illinois-school-report-card-20171030-story.html

slides link: https://docs.google.com/presentation/d/1TRypyG9QB7EEPWkDNdd-275msilGAXIkIutl_Bn2WyE/edit?usp=sharing


 