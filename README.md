# School_District_Analysis

## Overview of the Project

The project is a data analysis of school district using Pandas library in Python code. The data is obtained from separate CSV files, which are pulled and read into Pandas, in order to analyze it.

## Purpose of the Project

The purpose of the project is to provide an analysis to the PyCitySchools school district, by analizing the student testing data for all schools in the district. The school district wants to analyze the following KPI's for all the schools in the district:

- Average math score for each grade
- Average reading score for each grade
- Percentage of passing students that passed math for each grade
- Percentage of passing students that passed rading for each grade
- Performance of each school by size
- School performance based on the budget (Correlation between budget and passing students)
- School performance based on the type

In addition, The School board suspects that math and reading grades for students in 9th grade at Thomas High School have been altered. They would like to know how the altered grades affect the overall school district analysis.

## Deliverable 1 

For this part of the project, the analysis was done by using the loc method, to execute logical arguments, compare, filter, and replace the math and reading scores for the 9th grades students at Thomas High School to NaNs.

![Reading_scores_to_NaN](https://user-images.githubusercontent.com/98929742/158083052-7bc6d348-362a-4d1a-abfa-09976924dfd6.JPG)


![Reading_scores_to_NaN_DF](https://user-images.githubusercontent.com/98929742/158083055-19b8243d-8755-4b5e-9a7b-b6ffd6547e91.JPG)


![Math_scores_to_NaN](https://user-images.githubusercontent.com/98929742/158083071-1f72604e-fe2e-468c-bba6-a0cf9dc4c351.JPG)


![Math_scores_to_NaN_DF](https://user-images.githubusercontent.com/98929742/158083074-483b69af-fd81-4097-b82c-216d3ad4f21d.JPG)


![Check_NaN_values](https://user-images.githubusercontent.com/98929742/158083080-fd87e426-2018-4295-bfb0-eccc34470f85.JPG)


![Check_NaN_values_df](https://user-images.githubusercontent.com/98929742/158083087-776af1ac-79d7-420a-9d4e-215a989b4682.JPG)


## Deliverable 2

### The district summary

Results including the 9th grade scores

![Before_NaN_School_District_DF](https://user-images.githubusercontent.com/98929742/158087790-f0660e96-0193-4861-ad88-b554cab30642.JPG)


Results not including the 9th grade scores

![After_NaN_School_District_DF](https://user-images.githubusercontent.com/98929742/158087825-2926489e-37f6-4e81-bd0e-ae1cd5a11103.JPG)

As is shown from the table, the data from The Thomas High School 9th grade scores for reading and math have a small to none impact on the school district analysis. Meaning that the school district overall analysis is not affected.

Variances:

-

### The school summary



The top 5 and bottom 5 performing schools, based on the overall passing rate
The average math score for each grade level from each school
The average reading score for each grade level from each school
The scores by school spending per student, by school size, and by school type







