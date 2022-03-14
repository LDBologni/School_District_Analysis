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

- Average Math score (**-0.1**) After adjusting
- Average Reading score same as before
- Percentage Passing Math (**-0.02%**) After adjusting
- Percentage Passing reading (**-0.03%**) After adjusting
- Overall Percentage (**-0.01%**) After adjusting

### The school summary

#### Original Analysis

![Before_NaN_School_Summary_DF](https://user-images.githubusercontent.com/98929742/158089519-57b55cb3-7827-45c2-871e-a1600c836ca8.JPG)


#### Adjusted Analysis

![After_NaN_School_Summary_DF](https://user-images.githubusercontent.com/98929742/158091145-f04c84ca-1e09-494b-9a10-f24286074a0d.JPG)


As is shown in the previous tables, the data has been impacted by removing the 9th grade test result to

- Average Math score dropped **0.06**
- Average Reading score increased **0.14**
- Percentage passing Math dropped **26.36%**
- Percentage passing Reading dropped **27.64%**
- Percentage overall passing dropped **25.87**

### Thomas High School’s performance vs the other schools

![After_NaN_School_Summary_DF](https://user-images.githubusercontent.com/98929742/158091145-f04c84ca-1e09-494b-9a10-f24286074a0d.JPG)

As the table shows the Thomas High School has the lowest % Passing in Math, Reading and Overall in all schools in the district:

- Percentage Math passing **66.911315%
- Percentage Reading passing **69.663609%	
- Overall Percentage **65.076453%

### By Replacing the Grades

#### Math and reading scores by grade after replacing the grades

- Math Averages
![After_Nan_School_Averages_Math](https://user-images.githubusercontent.com/98929742/158095358-f49d7407-6efc-4646-81c6-76fda529d54b.JPG)

- Reading Averages
![After_Nan_School_Averages_Reading](https://user-images.githubusercontent.com/98929742/158095349-e7ec5e15-d099-44ed-8698-c147cf519e38.JPG) 

In the original analysis, Thomas High School had  for the 9th grade scores an average for Math of 83.6  and for reading an average 83.7. Now the scores have been replaced with NaN,as is shown in the previous tables.

#### Scores by school spending

![Table_of_schools_by_spending](https://user-images.githubusercontent.com/98929742/158096181-b2159e00-25d3-47d1-bf32-b929628fe9d2.JPG)

![Table_of_schools_by_spending_math](https://user-images.githubusercontent.com/98929742/158096190-7c22daf3-d6fe-47f1-9b93-eb23c4d5c40e.JPG)

Thomas High School falls in the spending range of $630-$644

####  Scores by school size

-Before 

![Math_scores_by_size_before](https://user-images.githubusercontent.com/98929742/158096722-a5d629de-54cc-4fbf-9fd3-b333bacb1b58.JPG)

- After

![Math_scores_by_size](https://user-images.githubusercontent.com/98929742/158096737-3c67b067-174a-4044-8333-4a8807d4a88e.JPG)



#### Scores by school type

-Before 

![Math_scores_by_type_before](https://user-images.githubusercontent.com/98929742/158096753-6a09b912-6620-4262-b8fb-2b3d9c62ed83.JPG)

-After

![Math_scores_by_type](https://user-images.githubusercontent.com/98929742/158096854-6a5ec67c-3d5e-450f-9ab5-04a0d2d8c90e.JPG)


## Summary


Unfortunately, it is not possible to determine the extent of the potential academic dishonesty or identify soecific indivuals to exclude from the dataset. As a consequence of this, the entire ninth grade of students from Thomas High School have had their scores omitted from the results. This is a suboptimal situation because a full set of data is ideal for creating the most accurate results.

Replacing the ninth graders' scores with NaN caused Thomas High School's overall passing percentages and average scores to plummet. The district as a whole has also had its average math and reading scores decrease, as well as the overall passing percentage for students. Furthermore, Thomas High School lost its placement as a top five school within this District. However, after updating the total student counts to exclude the Thomas High School ninth graders and omitting their scores from the dataset, Thomas High School regained its high average scores and retained its position as the number two school in the District. To view the full script, please open PyCitySchools_Challenge.ipynb in Jupyter Notebook.



