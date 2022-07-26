An Analysis Academic Performance of Standardized Tests Against Local Factors

Overview:
An analysis was conducted on the standardized test scores of students across 15 schools in a district.  The analysis factored in school population, funding, and the types of schools. The goal of this analysis was to identify trends in student funding and student standardized test scores in order to make funding decisions at the school and district level. This analysis will agregate data from a complete dataframe containing the students names, test scores, and information regarding the school they attended which include sizez, type, and level of funding.

Data Analysis Results:
The dataframes generated in this report differ from the data reported in the module.  Test scores of the 9th grade from Thomas High School were omitted for this analysis.

District Summary
With the removal of the 9th grade test scores from the dataset, 461 students scores were recoreded as null.  From a total population of 39170 it was expected that this would bias the district summary scores and passing rate low, however would have a marginal impact on the data.  Compared to the initial analysis, the district analysis with 9th grade scores from Thomas High School removed was roughly 0.1-0.2% lower in average score and overall passing rate.

Fig 1: Initial District Summary
Fig 2: 9th Grade from Thomas High School Omittied District Summary

School Summary 
The School Summary dataframe remained largely unaffected, and only affected the data for Thomas High School.  Initially omitting the 9th grade data from Thomas High School dropped the average math score, average reading score and overall passing rate to around 60%.  However when normalized against and adjusted population accounting for the removal of 9th grade students, the average scores and passing rate were nearly the same, and changed by <1% in each category.

Fig 3: Initial Analysis Summary for Thomas High School
Fig 4: 9th Grade Omitted Summary for Thomas High School
Fig 5: Population Normalized Summary With 9th Grade Omitted for Thomas High School

Ranking Against Ohter Schools
In the initial analysis, Thomas High School ranked among the top 5 schools in the district and was second in overall passing rate.  After removing the 9th grade scores, and normalizing the grades for the adjusted population size, Thomas High School still ranked among the top 5 schools and remained in second place by overall passing rate.  The actual scores and passing rates were slightly lower in the 9th grade omitted analysis which could suggest that the average 9th grade scores were higher than the agraggate average scores of the 10th to 12th grade.

Fig 6: Initial Summary Top 5 schools
Fig 7: 9th Grade Omitted Top 5 schools
