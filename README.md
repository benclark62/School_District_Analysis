# School_District_Analysis

## Overview of the school district analysis: 
We have been tasked with assisting the City School District Chief Data Scientist in aggregating, cleaning, and analyzing standardized test data.  The final output highlights trends in school funding, the impact of funding on student performance, and is intended to inform the School Board's upcoming decisions on school funding. 

Upon discovering grading irregularities in the Thomas High School ninth grade class, the reading and math grades for all students in that cohort were converted to "NaN" values while grading processes were being evaluated.  For this exercise, we were then tasked with refreshing the overall District-, School-, and Grade-level analysis.

## Results: 

### How is the district summary affected?
- Removing the questionable Thomas High School ninth grade test scores (THS) had resulted in slight reductions in % passing results for the entire District
- % Passing Math and % Passing Reading were each reduced by -22bps and -15bps in the updated analysis (from 74.98% to 74.76% and from 85.81% to 85.66%, respectively)
- % Overall Passing was reduced -31bps (from 65.17% to 64.86%)

**District Summary BEFORE Changes**
![district_summary_df_BEFORE](https://github.com/benclark62/School_District_Analysis/blob/main/Resources/district_summary_df_BEFORE.png)

**District Summary AFTER Changes**
![district_summary_df_AFTER](https://github.com/benclark62/School_District_Analysis/blob/main/Resources/district_summary_df_AFTER.png)


### How is the school summary affected?
- Removing the questionable THS test scores resulted in slight changes in average scores and passing rates
- Average Math Scores (-7bps) and % Passing Math (-9bps) saw minor reductions
- Average Reading Scores were a mixed bag with a small increase in Average Reading Score (+5bps) but a reduction in passing rates (-29bps)
- Overall Passing Percentage dropped from 90.95% to 90.63%
- The minor impacts to Thomas High School performance indicate that the contested ninth grade scores were in-line with performance observed in grades 10-12

**Top 5 Schools Summary BEFORE Changes**
![School Summary BEFORE](https://github.com/benclark62/School_District_Analysis/blob/main/Resources/ths_per_school_summary_df_BEFORE.png)

**Top 5 School Summary AFTER Changes**
![School Summary AFTER](https://github.com/benclark62/School_District_Analysis/blob/main/Resources/ths_per_school_summary_df_AFTER.png)


### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
- Thomas High School rankings relative to other schools did not change based after removing ninth graders' scores
- Based on Overall Passing Percentage, Thomas High School remained the second highest ranked school behind Cabrera High School


### How does replacing the ninth-grade scores affect the following:
#### Math and reading scores by grade
- While only Thomas High School ninth-grade scores were affected, the overall district ninth-grade average math scores dropped -20bps (from 78.94 to 78.74) and reading scores declined by -7bps (from 81.91 to 81.84)
- Math and Reading scores for tenth- through twelfth-grade students across the district were unaffected

**District Level Ninth-Grade Average Scores BEFORE Changes**
![Ninth Grade Averages BEFORE](https://github.com/benclark62/School_District_Analysis/blob/main/Resources/ninth-grade_averages_BEFORE.png)

![Average Math by Grade BEFORE](https://github.com/benclark62/School_District_Analysis/blob/main/Resources/math_by_grade_BEFORE.png)

![Average Reading by Grade BEFORE](https://github.com/benclark62/School_District_Analysis/blob/main/Resources/reading_by_grade_BEFORE.png)

**District Level Ninth-Grade Average Scores AFTER Changes**
![Ninth Grade Averages AFTER](https://github.com/benclark62/School_District_Analysis/blob/main/Resources/ninth-grade_average_scores_AFTER.png)

![Average Math by Grade AFTER](https://github.com/benclark62/School_District_Analysis/blob/main/Resources/math_by_grade_AFTER.png)

![Average Reading by Grade AFTER](https://github.com/benclark62/School_District_Analysis/blob/main/Resources/reading_by_grade_AFTER.png)

#### Scores by school spending
- The $630 - $644 bin, which includes Thomas High School, was the only bin affected by the grade updates
- Average math (-2bps) and average reading (+2bps) scores saw minor changes
- Passing percentages also reflected minor negative impacts: % Passing Math (-2bps), % Passing Reading (-7bps), and % Overall Passing (-8bps)

**Results by Spending Group BEFORE Changes**
![Performance by Spend BEFORE](https://github.com/benclark62/School_District_Analysis/blob/main/Resources/perf_by_spend_BEFORE.png)

**Results by Spending Group AFTER Changes**
![Perfromance by Spend AFTER](https://github.com/benclark62/School_District_Analysis/blob/main/Resources/perf_by_spend_AFTER.png)

#### Scores by school size
- The Medium (1000 - 2000) cohort, which includes Thomas High School, was the only cohort affected by the grade updates
- Average math (-1bps) and average reading (+1bps) scores saw minor changes
- Passing percentages also reflected minor negative impacts: % Passing Math (-2bps), % Passing Reading (-6bps), and % Overall Passing (-6bps)

**Results by School Size Group BEFORE Changes**
![Performance by Size BEFORE](https://github.com/benclark62/School_District_Analysis/blob/main/Resources/perf_by_size_BEFORE.png)

**Results by School Size Group AFTER Changes**
![Perfromance by Size AFTER](https://github.com/benclark62/School_District_Analysis/blob/main/Resources/perf_by_size_AFTER.png)

#### Scores by school type
- The Charter school type, which includes Thomas High School, was the only type affected by the grade updates
- Average math and reading scores saw changes of <1bps
- Passing percentages also reflected minor negative impacts: % Passing Math (-1bps), % Passing Reading (-4bps), and % Overall Passing (-4bps)

**Results by School Type BEFORE Changes**
![Performance by Type BEFORE](https://github.com/benclark62/School_District_Analysis/blob/main/Resources/perf_by_type_BEFORE.png)

**Results by School Type AFTER Changes**
![Perfromance by Type AFTER](https://github.com/benclark62/School_District_Analysis/blob/main/Resources/perf_by_type_AFTER.png)


## Summary: 
- Thomas High School saw a -32bps reduction in Overall Passing % after removing the ninth-grade scores, dropping from 90.95% to 90.63%
- The entire District's Overall Passing % saw a -31bps reduction, dropping to 64.86% from 65.17%
- Average Math Scores and % Passing Math were more negatively impacted than Reading in all categories by the replacement of the Thomas High School ninth-grade scores
- Impacts to scores and passing percentages in each group remained below ~30bps, reflecting the relatively small impact had by removing above average scores for 1.2% (461 of 39,170 students) of the overall District student population
