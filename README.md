An Analysis Academic Performance of Standardized Tests Against Local Factors

Overview:
An analysis was conducted on the standardized test scores of students across 15 schools in a district.  The analysis factored in school population, funding, and the types of schools. The goal of this analysis was to identify trends in student funding and student standardized test scores in order to make funding decisions at the school and district level. This analysis will agregate data from a complete dataframe containing the students names, test scores, and information regarding the school they attended which include sizez, type, and level of funding. From the original report, there was evidence of grade tampering in the 9th grade standardized test scores from Thomas High School.  A re-analysis of the data was conducted in order to determine if there is evidence of cheating and if it had a significant impact on the conclusions made from the analysis.

Data Analysis Results:
The dataframes generated in this report differ from the data reported in the module.  Test scores of the 9th grade from Thomas High School were omitted for this analysis.

District Summary
With the removal of the 9th grade test scores from the dataset, 461 students scores were recoreded as null.  From a total population of 39170 it was expected that this would bias the district summary scores and passing rate low, however would have a marginal impact on the data.  Compared to the initial analysis, the district analysis with 9th grade scores from Thomas High School removed was roughly 0.1-0.2% lower in average score and overall passing rate.

Fig 1: Initial District Summary
![Fig 1](https://user-images.githubusercontent.com/108313294/181306302-e9926ca5-d0d0-4b43-bc5b-44e4e3b56fa9.png)

Fig 2: 9th Grade from Thomas High School Omittied District Summary
![Fig 2](https://user-images.githubusercontent.com/108313294/181306301-45ecb0e8-0fb5-4cb2-b39d-ded84ff3b14b.png)

School Summary 
The School Summary dataframe remained largely unaffected, and only affected the data for Thomas High School.  Initially omitting the 9th grade data from Thomas High School dropped the average math score, average reading score and overall passing rate to around 60%.  However when normalized against and adjusted population accounting for the removal of 9th grade students, the average scores and passing rate were nearly the same, and changed by <1% in each category.

Fig 3: Initial Analysis Summary for Thomas High School
![Fig 3](https://user-images.githubusercontent.com/108313294/181306334-d93336f9-4446-4aa9-87a3-a7421c772bf4.png)

Fig 4: 9th Grade Omitted Summary for Thomas High School
![Fig 4](https://user-images.githubusercontent.com/108313294/181306348-26f9084c-3f70-47a6-813d-d2cd6b46d59a.png)

Fig 5: Population Normalized Summary With 9th Grade Omitted for Thomas High School
![Fig 5](https://user-images.githubusercontent.com/108313294/181306364-d8b5557a-bcb9-4917-9580-a8d4ada2f123.png)

Ranking Against Ohter Schools
In the initial analysis, Thomas High School ranked among the top 5 schools in the district and was second in overall passing rate.  After removing the 9th grade scores, and normalizing the grades for the adjusted population size, Thomas High School still ranked among the top 5 schools and remained in second place by overall passing rate.  The actual scores and passing rates were slightly lower in the 9th grade omitted analysis which could suggest that the average 9th grade scores were higher than the agraggate average scores of the 10th to 12th grade.

Fig 6: Initial Summary Top 5 schools
![Fig 6](https://user-images.githubusercontent.com/108313294/181306389-0cbaf11e-6517-467d-85d1-bb201adee30f.png)

Fig 7: 9th Grade Omitted Top 5 schools
![Fig 7](https://user-images.githubusercontent.com/108313294/181306400-209d019a-1083-4f68-931f-1ed1901b0fdd.png)

Omitted Grade 9 Data Grade Level Aggregated Analysis

  * Group by grade: The aggregated dataframe containing math and reading scores grouped by grade remained the same with the exception of the 9th grade average scores for Thomas High School being reported as NaN in the table of the second analysis.

Fig 8: NaN Entry in Grade Level Average Aggregated Data
![Fig 8](https://user-images.githubusercontent.com/108313294/181306410-09e12f84-edf9-4425-a1d1-9b378f877304.png)

 * Scores by School Spending: The agregated dataframe containing average scores and passing rates were identical across both analysis despite omitting 9th grade data from Thomas High School.  Thomas High School was originally binned in the $631-645 per student spending bracket.  The removal of 9th grade data should not change the budget per student, since although those scores were not counted, they students still exist, and absorb part of the budget.  Therefore this data should not change.
 
 * Scores by School Size: The aggregated dataframe containing the average scores and passing rates grouped by school size also remained identical to the first analysis.  The total population of Thomas High School was 1635, of which 9th graders made up 461 students.  The population of the school minus the 9th graders was 1174, which still placed Thomas High School in the Medium bin defined as 1000-1999 students. The average scores may have been slightly smaller given enough precision but do not significantly impact the data.

* Scores by School Type: The aggregated dataframe containing the average scores and passing rates by school type also did not change, since at no point did Thomas High School change types with the removal of the 9th grade scores. The average score and passing rate may be slightly lower given enough precision but does not significantly impact the data.

Summary:
The purpose of the secondary analysis was to determine the impact of a suspected case of academic dishonesty in the 9th grade class of Thomas High School and how it may have impacted the data.  Based on the findings, there was little to no impact on the data, and therefore there was likely no cheating involved, OR the cheater knew to keep the grade averages close to the school grade average of around 83%.  The few changes that were identified were the slightly lower math, reading, and overall passing rates in the district summary, and school summary. The school rankings remained the same, however the overall passing rate was slightly lower for Thomas High School. Finally, the groupby grade dataframes for the 9th grade of Thomas High school, showed NaN instead of a value which was expected since those values were omitted in the second analysis.



