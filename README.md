# School District Analysis

## Project Overview
### The purpose of this project is to analyze the data of an entire School District, such as funding and student grades, to learn new insights and visually provide clear results on each school's performance. Additionally, to uphold state-testing standards, this analysis was conduced twice due to potential academic dishonesty among a group of students. The implications of omitting the potentially dishonest data is also discussed.
---
## Resources
**Resources:** All data used in this analysis is found inside of the [Resources](https://github.com/Mishkanian/School_District_Analysis/tree/main/Resources) folder.

**Software:** Python 3.7, Anaconda, Jupyter Notebook

## Results
Due to potential academic dishonesty by the ninth grade students of Thomas High School, this analysis was conducted twice. The first trial of this analysis included the full set of student data. In the second trial of this analysis, the ninth grade students of Thomas High School had their scores omitted from the calculations. For consistency, all DataFrames below are only generated from the second trial of analysis.

- Replacing the ninth graders' math and reading scores with NaN resulted in the following changes for Thomas High School:
  - The overall passing percentage for Thomas High School fell to 65%.
  - The overall passing percentage for the entire district fell to 64.9%.
  - Thomas High School was no longer included on the list of top five schools.

- When the ninth graders' of Thomas High School had their scores omitted from the calculations, the following changes occured:
  - Overall Passing Percentages and Average Scores were only slightly changed from the first trial.
    - Average Scores for Math and Reading *increased* by 0.06
    - Overall Passing Percentages decreased by 0.11%
  - **School rankings are unchanged.** Thomas High School is still the second best performing school in the district with an overall passing rate of 90.63% among their tenth through twelfth graders.

### The Effects of School Budget and School Size
It is found that Average Scores and Passing Percentages do not increase as spending per student increases. In fact, there appears to be a negative relation between spending and Overall Passing Percentages.

![school_budget_per_student_df](https://github.com/Mishkanian/School_District_Analysis/blob/main/DataFrames_PyCity/school_budget_per_student_df.png)


When considering School Size, "Large" Schools (Over 2,000 Students) have the lowest average scores and passing percentages. The difference in performance between "Small" and "Medium" Size Schools is negligible (< 1%).

![school_size_df](https://github.com/Mishkanian/School_District_Analysis/blob/main/DataFrames_PyCity/school_size_df.png)

### Charter vs. District Schools
Charter schools generally performed better than District schools in this analysis. The top five schools with the highest overall passing percentages are all Charter schools, whereas the bottom five are all District Schools. As seen in the DataFrame below, **Charter schools have a 36% higher overall passing percentage** than District schools.

![school_type_df](https://github.com/Mishkanian/School_District_Analysis/blob/main/DataFrames_PyCity/school_type_df.png)

## Summary
Omitting the ninth grade student scores of Thomas High School from the dataset did not materially change any outcomes of this analysis.

**Author: Michael Mishkanian**  

For all questions and inquireies, please contact me on [LinkedIn](https://www.linkedin.com/in/michaelmishkanian/).
