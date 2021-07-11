# School_District_Analysis

# Overview of the school district analysis

The purpose of analysis is to provide the high-level snapshot of the district's key metrics, an overview of the key metrics for each school and school performance based on type, size and school budget per student. 

## Resources
Data source: schools_complete.csv, students_complete.csv

## Deliverables
[PyCitySchools_Challenge.ipynb](https://github.com/xenia-e/School_District_Analysis/blob/main/PyCitySchools_Challenge.ipynb) Jupyter Notebook file containing script for the analisys
[README.md](https://github.com/xenia-e/School_District_Analysis/blob/main/README.md) - written analysis of project in markdown file


# Methods
Using Python and Jupyter Notebook we perform the analysis on provided dataset. To make sure the resultes would be correct we check the data consistemsy and exclude possible errors.

# Results 
New data set we have appeared to have some data inconsystensy in grades data.

- The error in grades data **affect district summary** is in reducing overall scores of school disctrict? As you can see in the two tables privided _overall score is reduced_ about 0.3%. Allother scores was aswell reduced 0.1-0.2%

![PyCitySchools_disctrict%20summary.png](https://github.com/xenia-e/School_District_Analysis/blob/main/Analysis/PyCitySchools_disctrict%20summary.png)
>Figure 1 - School district summary before data correction


![PyCitySchools_district_summary_corrected.png](https://github.com/xenia-e/School_District_Analysis/blob/main/Analysis/PyCitySchools_district_summary_corrected.png)
>Figure 1 - Corrected data school district summary

- **The school summary affected** was affected by this error in a more drustic way. As you can see in the tables below, the overall passing percentege of Tomas Hight School is down by more than 30% from 91.0% to 65.1%. Passing percentaeg on both math and reading are reduced from 93.3% &	97.3% to 66.9% and	69.7% accordingly. The average scores were not affected as much. 
- How does replacing the ninth graders’ math and reading scores affect Thomas High-School’s performance relative to the other schools?
- How does replacing the ninth-grade scores affect the following:
  - Math and reading scores by grade
  - Scores by school spending
  - Scores by school size
  - Scores by school type


# Summary

Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
