# School_District_Analysis

# Overview of the school district analysis

The purpose of the analysis is to provide a high-level snapshot of the district's key metrics, an overview of the key metrics for each school, and school performance based on type, size, and school budget per student. And reveal the effect of missing data on the end results. 

## Resources
Data source: schools_complete.csv, students_complete.csv

## Deliverables
[PyCitySchools_Challenge.ipynb](https://github.com/xenia-e/School_District_Analysis/blob/main/PyCitySchools_Challenge.ipynb) Jupyter Notebook file containing the script for the analysis
[README.md](https://github.com/xenia-e/School_District_Analysis/blob/main/README.md) - written analysis of the project in the markdown file


# Methods
Using Python and Jupyter Notebook we perform the analysis on provided dataset. To make sure the results would be correct we check the data consistency and exclude possible errors.

# Results 
New data set we have appeared to have some data inconsistency in grades data which affected the results of the analysis.

- The error in grades data ** affects district summary** by reducing the overall scores of the school district. As you can see in the two tables provided the overall score is reduced_ about 0.3%. All other scores were as well reduced 0.1-0.2%

![PyCitySchools_disctrict%20summary.png](https://github.com/xenia-e/School_District_Analysis/blob/main/Analysis/PyCitySchools_disctrict%20summary.png)
>Figure 1 - School district summary before data correction

![PyCitySchools_district_summary_corrected.png](https://github.com/xenia-e/School_District_Analysis/blob/main/Analysis/PyCitySchools_district_summary_corrected.png)
>Figure 1 - Corrected data school district summary

- Since data corrections were within only Tomas High School (THS) **The School Summary** was not affected by this error as much. This school performance was affected more drastically. 
 As you can see in the tables below, the overall passing percentage of THS is down by 25.1% (from 91.0% to 65.1%). Passing math and reading percentages are reduced from 93.3% and 97.3% to 66.9% and 69.7% accordingly. The average scores were not affected as much. 

![PyCitySchools_school_summary.png](https://github.com/xenia-e/School_District_Analysis/blob/main/Analysis/PyCitySchools_school_summary.png)
>Figure 1 - The School Summary before data correction

![PyCitySchools_school_summary_corrected.png](https://github.com/xenia-e/School_District_Analysis/blob/main/Analysis/PyCitySchools_school_summary_corrected.png)
>Figure 1 - Corrected data school summary

- Replacing the ninth-grade students’ math and reading scores led to a decrease in THS performance relative to the other schools and losing its position as one of the most successful schools in the district. In order to correct this error in the analysis, we removed all ninth-grade students from our calculations and got relatively correct scores back to the final results table, and put THS in the second position among district schools.
- The replacement of the ninth-grade scores affect the following:
 - Math and reading scores by grade: didn't affect any results but THS, where results were replaced for the NaN
 - Scores by school spending: didn't affect
 - Scores by school size: didn't affect
 - Scores by school type: didn't affect

# Summary

As a summary of the performed analysis, we can conclude that after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs we can say that this affected THS itself more than overall school district data, none the less:
1. The overall passing percentage lowered from 65.2% to 64.9% and if rounded to one place will not show any difference. The average district's scores for math and reading were not affected by more than 0.1-0.2% as well.
2. The overall passing percentage of THS is down by 25.1% (from 91.0% to 65.1%). Passing math and reading percentages are reduced from 93.3% and 97.3% to 66.9% and 69.7% accordingly if ninth-grade students are not removed from the calculations. The average scores were not affected as much. 
3. The position of the school among other schools in the district was no affected if removing ninth-grade students from the calculations of the average scores.
4. The scores by size, spendings per student, or school type were not affected.

All this was possible by clearing the data and correcting the calculations based on the new student count (without the ninth-grade student of THS). If we left the total number of students unchanged it would lead to errors in analysis results and school performance. 

