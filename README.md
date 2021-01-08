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
- % Passing Math and % Passing Reading were each reduced by -22bps and -15bps in the udpated analysis (from 74.98% to 74.76% and from 85.81% to 85.66%, respectively)
- % Overall Passing was reduced -31bps (from 65.17% to 64.86%)

![district_summary_df_BEFORE](https://github.com/benclark62/School-District-Analysis/blob/main/resources/district_summary_df_BEFORE.png)

![district_summary_df_AFTER](https://github.com/benclark62/School-District-Analysis/blob/main/resources/district_summary_df_AFTER.png)

### How is the school summary affected?
-- add THS from per_school_summary_df
- Removing the questionable THS test scores resulted in slight changes in average scores and passing rates
- Average Math Scores (-7bps) and % Passing Math (-9bps) saw minor reductions
- Average Reading Scores were a mixed bag with a small increase in Average Reading Score (+5bps) but a reduction in passing rates (-29bps)
- Overall Passing Percentage dropped from 90.94% to 90.63%
- The minor impacts to Thomas High School performance indicate that the contested ninth grade scores were in-line with performance observed in grades 10-12

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
- Thomas High School rankings realtive to other schools did not change based after removing ninth graders' scores
- Based on Overall Passing Percentage, Thomas High School remained the second highest ranked school behind Cabrera High School

### How does replacing the ninth-grade scores affect the following:
#### Math and reading scores by grade
-- add tables for district-level ninth-grade math and reading before and after; overall grade-level tables --
- While only Thomas High School ninth-grade scores were affected, the overall district ninth-grade average math scores dropped -20bps (from 78.94 to 78.74) and reading scores declined by -7bps (from 81.91 to 81.84)
- Math and Reading scores for tenth- through twelfth-grade students across the district were unaffected

#### Scores by school spending
-- add perf_by_spend before and after
- The $630 - $644 bin, which includes Thomas High School, was the only bin affected by the grade udpates
- Average math (-2bps) and average reading (+2bps) scores saw minor changes
- Passing percentages also reflected minor negative impacts: % Passing Math (-2bps), % Passing Reading (-7bps), and % Overall Passing (-8bps)

#### Scores by school size
-- add perf_by_size before and after
- The Medium (1000 - 2000) cohoort, which includes Thomas High School, was the only cohort affected by the grade updates
- Average math (-1bps) and average reading (+1bps) scores saw minor changes
- Passing percntages also reflected minor negative impacts: % Passing Math (-2bps), % Passing Reading (-6bps), and % Overall Passing (-6bps)

#### Scores by school type
-- add perf_by_type before and after
- The Charter school type, which includeds Thomas High School, was the only type affected by the grade updates
- Average math and reading scores saw changes of <1bps
- Passing percentages also reflected minor negative impacts: % Passing Math (-1bps), % Passing Reading (-4bps), and % Overall Passing (-4bps)


## Summary: 
Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
- Thomas High School saw a -32bps reduction in Overall Passing % after removing the ninth-grade scores, dropping from 90.95% to 90.63%
- The entire District's Overall Passing % saw a -31bps reduction, dropping to 64.86% from 65.17%
- Average Math Scores and % Passing Math were more negatively impacted than Reading in all categories by the replacement of the Thomas High School ninth-grade scores
- Impacts to scores and passing percentages in each group remained below ~30bps, reflecting the relatively small impact had by removing above average scores for 1.2% (461 of 39,170 students) of the overall District student population
