# School District Analysis

## Project Overview
### The purpose of this project is to analyze the data of an entire School District, such as funding and student grades, to learn new insights and visually provide clear results on each school's performance. Additionally, to uphold state-testing standards, this analysis was conduced twice due to potential academic dishonesty among a group of students. The implications of omitting the potentially dishonest data are also discussed.
---
## Resources
**Resources:** All data used in this analysis is found inside of the [Resources](https://github.com/Mishkanian/School_District_Analysis/tree/main/Resources) folder.

**Software:** Python 3.7, Anaconda, Jupyter Notebook

## Results
Due to potential academic dishonesty by the ninth grade students of Thomas High School, this analysis was conducted twice. The first trial of this analysis included the full set of student data. In the second trial of this analysis, the ninth grade students of Thomas High School had their scores omitted from the calculations. The entire ninth grade class of Thomas High School have had their scores replaced with NaN. The DataFrame below is a summary representing the District after replacing the ninth graders' scores with NaN.
![district_overview](https://github.com/Mishkanian/School_District_Analysis/blob/main/DataFrames_PyCity/district_overview.png)

- Replacing the ninth graders' math and reading scores with NaN resulted in the following changes for Thomas High School:
  - The overall passing percentage for Thomas High School fell to 65%
  - The overall passing percentage for the entire district fell to 64.9%
  - Thomas High School was no longer included on the list of top five schools.

- When the ninth graders' of Thomas High School had their scores omitted from the calculations, the following changes occured:
  - The overall passing percentages of Thomas High School decreased by 0.11%
  - The average scores of Thomas High School for math and reading *increased* by 0.06
  - For the spending range of $630-644 per student, the overall passing percentage decreased by 0.1%
  - **School rankings are unchanged.** Thomas High School is still the second best performing school in the district with an overall passing rate of 90.63% among their tenth through twelfth graders.

### The Effects of School Budget and School Size
It is found that Average Scores and Passing Percentages do not increase as spending per student increases. In fact, the top performing school in the entire school district (Cabera High School) received $68 *less* per student than the lowest performing school (Johnson High School). This implies that there are more relevant factors than funding that decide average student scores.

![school_budget_per_student_df](https://github.com/Mishkanian/School_District_Analysis/blob/main/DataFrames_PyCity/school_budget_per_student_df.png)


When considering School Sizes, "Large" Schools (Over 2,000 Students) have the lowest average scores and passing percentages. The difference in performance between "Small" and "Medium" Size Schools is negligible (approximately 1%). Interestingly, all District schools in this dataset are characterized as "Large" schools. This may be an indication that students in this district learn and perform better in smaller, more intimate settings.

![school_size_df](https://github.com/Mishkanian/School_District_Analysis/blob/main/DataFrames_PyCity/school_size_df.png)

### Charter vs. District Schools
Charter schools generally performed better than District schools in this analysis. The top five schools with the highest overall passing percentages are all Charter schools, whereas the bottom five are all District Schools. Charter schools in this dataset were typically characterized as "Small" and "Medium" size schools. As seen in the DataFrame below, **Charter schools have a 36% higher overall passing percentage** than District schools.

![school_type_df](https://github.com/Mishkanian/School_District_Analysis/blob/main/DataFrames_PyCity/school_type_df.png)

### Average Scores by Grade Level
After analyzing the average scores for math and reading by grade level for each school, it is found that a students grade level does not affect their scores as much as the school that they attend. The average scores within each school only varries by 1-2% depending on grade level. However, the difference in scores is more apparent when comparing different schools. 

To see the detailed breakdown of Average Math Scores by grade, please click [here](https://github.com/Mishkanian/School_District_Analysis/blob/main/DataFrames_PyCity/math_scores_grade.png). Alternatively, if you would like to view the Average Reading Scores by grade, please click [here](https://github.com/Mishkanian/School_District_Analysis/blob/main/DataFrames_PyCity/reading_scores_grade.png).

## Summary
Unfortunately, it is not possible to determine the extent of the potential academic dishonesty or identify soecific indivuals to exclude from the dataset. As a consequence of this, the entire ninth grade of students from Thomas High School have had their scores omitted from the results. This is a suboptimal situation because a full set of data is ideal for creating the most accurate results.

Relacing the ninth graders' scores with NaN caused Thomas High School's overall passing percentages and average scores to plummet. The district as a whole has also had its average math and reading scores decrease, as well as the overall passing percentage for students. Furthermore, Thomas High School lost its placement as a top five school within this District. However, after updating the total student counts to exclude the Thomas High School ninth graders and omitting their scores from the dataset, Thomas High School regained its high average scores and retained its position as the number two school in the District. To view the full script, please open PyCitySchools_Challenge.ipynb in Jupyter Notebook.


**Author: Michael Mishkanian**  

For all questions and inquiries, please contact me on [LinkedIn](https://www.linkedin.com/in/michaelmishkanian/).
