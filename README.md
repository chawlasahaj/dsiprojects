# Project 1: Standardized Testing, Statistical Summaries and Inference

### Overview

In this project, the main focus is to analyze data from SAT and ACT college entrance  exams in 2017 and 2018. Using various methods of data analysis, visualization, and hypothesis testing, this project aims to tackle one central question - 

## How can SAT drive participation rates across the nation?


## Executive Summary

TBD!

### Contents:

- [2017 Data Import & Cleaning](#2017-Data-Import-and-Cleaning)
- [2018 Data Import and Cleaning](#2018-Data-Import-and-Cleaning)
- [Exploratory Data Analysis](#Exploratory-Data-Analysis)
- [Data Visualization](#Visualize-the-data)
- [Descriptive and Inferential Statistics](#Descriptive-and-Inferential-Statistics)
- [Outside Research](#Outside-Research)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)


### Data Dictionary


|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|object|ACT/SAT|State where ACT/SAT was taken| 
|act_participation_2017|float|ACT|Percentage of students that took the ACT in 2017|
|act_english_2017|float|ACT|Average score for ACT English in 2017|
|act_math_2017|float|ACT|Average score for ACT Math in 2017|
|act_reading_2017|float|ACT|Average score for ACT Reading in 2017|
|act_science_2017|float|ACT|Average score for ACT Science in 2017|
|act_composite_2017|float|ACT|Average composite score for ACT English, Math, Reading and Science in 2017|
|sat_participation_2017|float|SAT|Percentage of students that took the SAT in 2017|
|sat_ebrw_2017|int|SAT|Average score for SAT Evidence-Based Reading & Writing (EBRW) in 2017|
|sat_math_2017|int|SAT|Average score for SAT Math in 2017|
|sat_total_2017|int|SAT|Average total score for SAT EBRW & Math in 2017|
|act_participation_2018|float|ACT|Percentage of students that took the ACT in 2018|
|act_english_2018|float|ACT|Average score for ACT English in 2018|
|act_math_2018|float|ACT|Average score for ACT Math in 2018|
|act_reading_2018|float|ACT|Average score for ACT Reading in 2018|
|act_science_2018|float|ACT|Average score for ACT Science in 2018|
|act_composite_2018|float|ACT|Average composite score for ACT English, Math, Reading and Science in 2018|
|sat_participation_2018|float|SAT|Percentage of students that took the SAT in 2018|
|sat_ebrw_2018|int|SAT|Average score for SAT Evidence-Based Reading & Writing (EBRW) in 2018|
|sat_math_2018|int|SAT|Average score for SAT Math in 2018|
|sat_total_2018|int|SAT|Average total score for SAT EBRW & Math in 2018|


### Recommendations

Based on the insights derived from the data, Iowa is a good target state for SAT to focus its efforts on.

It does not have an existing affiliation with either SAT or ACT. With average ACT participation (non-mandatory), it may be possible to lobby the Iowa board of education in order to provide state-level funding for the SAT to provide students for free, or even require it to be mandatory. Based on data across the nation as well as observational evidence, providing such incentives can drive participation across the state. 

Note that with increased participation, Iowa may expect lower average scores on the SAT going forward - as evidenced by SAT and ACT data from 2017/2018.