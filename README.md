# School District Analysis

## Project Overview
### The purpose of this project is to analyze the data of an entire School District, such as funding and student grades, to learn new insights and visually provide clear results on each school's performance. Additionally, to uphold state-testing standards, this analysis was conduced twice due to potential academic dishonesty among a group of students. The implications of omitting the potentially dishonest data is also discussed.
---
## Resources
**Resources:** All data used in this analysis is found inside of the [Resources](https://github.com/Mishkanian/School_District_Analysis/tree/main/Resources) folder.

**Software:** Python 3.7, Anaconda, Jupyter Notebook

## Results
Due to potential academic dishonesty by the ninth grade students of Thomas High School, this analysis was conducted twice. The first trial of this analysis included the full set of student data. In the second trial of this analysis, the ninth grade students of Thomas High School had their scores omitted from the calculations. The entire ninth grade class of Thomas High School have had their scores replaced with NaN. The DataFrame below is a summary representing the District after replacing the ninth graders' scores.
![district_overview](https://github.com/Mishkanian/School_District_Analysis/blob/main/DataFrames_PyCity/district_overview.png)

- Replacing the ninth graders' math and reading scores with NaN resulted in the following changes for Thomas High School:
  - The overall passing percentage for Thomas High School fell to 65%.
  - The overall passing percentage for the entire district fell to 64.9%.
  - Thomas High School was no longer included on the list of top five schools.

- When the ninth graders' of Thomas High School had their scores omitted from the calculations, the following changes occured:
  - Overall Passing Percentages and Average Scores for Thomas High School were only slightly changed from the first trial.
    - Average Scores for Math and Reading *increased* by 0.06
    - Overall Passing Percentages decreased by 0.11%
  - **School rankings are unchanged.** Thomas High School is still the second best performing school in the district with an overall passing rate of 90.63% among their tenth through twelfth graders.

### The Effects of School Budget and School Size
It is found that Average Scores and Passing Percentages do not increase as spending per student increases. In fact, there appears to be a negative relation between spending and Overall Passing Percentages.

![school_budget_per_student_df](https://github.com/Mishkanian/School_District_Analysis/blob/main/DataFrames_PyCity/school_budget_per_student_df.png)


When considering School Size, "Large" Schools (Over 2,000 Students) have the lowest average scores and passing percentages. The difference in performance between "Small" and "Medium" Size Schools is negligible (approximately 1%).

![school_size_df](https://github.com/Mishkanian/School_District_Analysis/blob/main/DataFrames_PyCity/school_size_df.png)

### Charter vs. District Schools
Charter schools generally performed better than District schools in this analysis. The top five schools with the highest overall passing percentages are all Charter schools, whereas the bottom five are all District Schools. As seen in the DataFrame below, **Charter schools have a 36% higher overall passing percentage** than District schools.

![school_type_df](https://github.com/Mishkanian/School_District_Analysis/blob/main/DataFrames_PyCity/school_type_df.png)

### Average Scores by Grade Level
After analyzing the average scores for math and reading by grade level for each school, it is found that a students grade level does not affect their scores as much as the school that they attend. The average scores within each school only varries by 1-2% depending on grade level. However, the difference in scores is more apparent when comparing different schools. 

To see the detailed breakdown of Average Math Scores by grade, please click [here](https://github.com/Mishkanian/School_District_Analysis/blob/main/DataFrames_PyCity/math_scores_grade.png). Alternatively, if you would like to view the Average Reading Scores by grade, please click [here](https://github.com/Mishkanian/School_District_Analysis/blob/main/DataFrames_PyCity/reading_scores_grade.png).

## Summary
Relacing the ninth graders' scores with NaN caused Thomas High School's overall passing percentages and average scores to plummet. 

However, after updating the total student counts to exclude the Thomas High School ninth graders and omitting their scores from the dataset, there was not a drastic change in any of outcomes of this analysis.

**Author: Michael Mishkanian**  

For all questions and inquireies, please contact me on [LinkedIn](https://www.linkedin.com/in/michaelmishkanian/).
