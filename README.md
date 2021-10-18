# School_District_Analysis
Module 4 School District Analysis

## Overview of Project
We were hired by Maria to conduct an anlysis of a school district using python and Pandas dataframes. After conducting our initial analysis, we found evidence of academic dishonesty, so we had to clean up the data that was no longer useful. Specifically, the 9th grade reading and math scores for Thomas High School had to be dropped from our analysis. Then, we would conduct our analysis once more. Maria asked us to note the differences between the two analyses.

## Results
 
 - How is the district summary affected?
   https://github.com/rharazim/School_District_Analysis/blob/main/Resources/district_summary.png
   There were no major changes to this summary, mostly due to all the schools being compiled and averaged together. The most notable differences was the increase in average math score from 78.9 to 79.0. 
   
 - How is the school summary affected?
   https://github.com/rharazim/School_District_Analysis/blob/main/Resources/per_school_summary.png
   Thomas High School's statistics (average math & reading scores, passing percentages) were slightly altered by the omittance of the 9th grade data. The overall passing percentage decreased from 90.94% to 90.63%. For a school the size of 1635 students, this difference is about 5 students. Average math score decreased by 0.06% while average reading score actually increased by 0.05%.  
   
 - How does replacing Thomas High School's 9th grade reading and test scores affect its performance relative to other schools?
   https://github.com/rharazim/School_District_Analysis/blob/main/Resources/top_schools.png
   Thomas High School's ranking did not change; it still remains the #2 school in terms of % of students passing
   
 - How does replacing the 9th grade scores affect the following:
    - Math and reading scores by grade
      https://github.com/rharazim/School_District_Analysis/blob/main/Resources/math_scores_by_spending.png <-- file name error, should be math_scores_by_grade
      https://github.com/rharazim/School_District_Analysis/blob/main/Resources/reading_scores_by_grade.png
      These metrics now contain "nan" for the 9th grade column of Thomas High School because that data was omitted. This makes it a poor comparison target for other schools if they were using this data.
      
    - Scores by school spending
      https://github.com/rharazim/School_District_Analysis/blob/main/Resources/scores_by_school_spending.png
      Thomas High School is in the $630-645 group of spending per student. These metrics were unaffected by the new anlysis. 
      
    - Scores by school size
      https://github.com/rharazim/School_District_Analysis/blob/main/Resources/scores_by_school_size.png
      Thomas High School is in the 'Medium' size school group. These metrics were also unaffected.
      
    - Scores by school type
      https://github.com/rharazim/School_District_Analysis/blob/main/Resources/scores_by_school_type.png
      Thomas High School is a charter school. This portion of the analysis was also unaffected. 
      
## Summary
After replacing the 9th grade math and reading scores of Thomas High School, there were several minor, yet meaningful, changes to our initial anlysis. Its average reading and math scores changed by around 0.05%, and the overall passing rate decreased by about 0.30%. It was not enough to change the school's position/rank, but it may affect how other schools compare their metrics to Thomas High School. Given that about 25% of Thomas High School's data had to be omitted, its own metrics became less reliable, since, like with smaller schools, the calculations are susceptible to larger fluctuations due to the smaller sample size.
