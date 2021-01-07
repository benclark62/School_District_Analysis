# School_District_Analysis
Module 4 - Python &amp; Jupyter

## Overview of the school district analysis: 
We have been tasked with assisting the City School District Chief Data Scientist in aggregating, clenaing, and analyizing standardized test data.  The final output highlights trends in school funding, the impact of funding on student performance, and is intended to inform the School Board's upcoming decisions on school funding. 

Upon discovering grading irregularities in the Thomas High School ninth grade class, the reading and math grades for all students in that cohort were converted to "NaN" values while grading processes were being evaluated.  For this exercise, we were then tasked with refreshing the overall District-, School-, and Grade-level analysis.

## Results: 
Using bulleted lists and images of DataFrames as support, address the following questions.

### How is the district summary affected?
-- add district_summary_df images before / after ---
- Removing the questionable Thomas High School ninth grade test scores (THS) had resulted in slight reductions in % passing results for the entire District
- % Passing Math and % Passing Reading were each reduced by ~10bps in the udpated analysis (from 74.9% to 74.8% and from 85.8% to 85.7%, respectively)
- % Overall Passing was reduced ~20bps (from 65.1% to 64.9%)

### How is the school summary affected?
-- add THS from per_school_summary_df
- Removing the questionable THS test scores resulted in slight changes in average scores and passing rates
- Average Math Scores (-7bps) and % Passing Math (-9bps) saw minor reductions
- Average Reading Scores were a mixed bag with a small increase in Average Reading Score (+5bps) but a contraction in passing rates (-29bps)
- Overall Passing Percentage dropped from 90.94% to 90.63%
- The minor impacts to Thomas High School performance indicate that the contested ninth grade scores were in-line with performance observed in grades 10-12

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
- Thomas High School rankings realtive to other schools did not change based after removing ninth graders' scores
- Based on Overall Passing Percentage, Thomas High School remained the second highest ranked school behind Cabrera High School

### How does replacing the ninth-grade scores affect the following:
#### Math and reading scores by grade
-- add tables for math and reading before and after --

#### Scores by school spending
-- add perf_by_spend before and after

#### Scores by school size
-- add perf_by_size before and after

#### Scores by school type
-- add perf_by_type before and after

## Summary: 
Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
