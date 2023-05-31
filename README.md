# pandas-challenge
In this challenge, I leveraged Python/Pandas to manipulate data from two CSV files, (files can be found in Resources folder), in order to perform analysis on school performance. 
## Conclusions Based On Analysis
1. 
2.
These conclusions are based on the below analysis, summarized first at a high-level that is then followed by an in-depth review of the data. 
## Analysis Summary

### District Summary
This dataframe shows how the district as whole has performed based on Math and Reading scores averaged across fifteen schools. The dataframe includes the below points:
* Total number of unique schools
* Total students
* Total budget
* Average math score
* Average reading score
* Percentage of students passing math (math test score of 70% or higher)
* Percentage of students passing reading (reading test score of 70% or higher)
* Percentage of students passing both math *and* reading (math test score of 70% or higher as well as reading test score of 70% or higher)

### School Summary
While the District Summary is useful in its own right, not all schools are created equal. Within the district, there are schools of varying types, sizes, and budgets. Using groupby School Name, the School Summary dataframe provides more granular data on school-by-school performance.
* School name
* School type (district or charter)
* Total students per school
* Total school budget
* Average math score per school
* Average reading score per school
* Percentage of students at school passing math (math test score of 70% or higher)
* Percentage of students at school passing reading (reading test score of 70% or higher)
* Percentage of students at school passing both math *and* reading (math test score of 70% or higher as well as reading test score of 70% or higher)

### Highest-Performing Schools (by % Overall Passing)
These are the five schools with the highest rate of students who passed both Math and Reading with scores of 70% or higher in both subjects:
1. Cabrera High School
2. Thomas High School
3. Griffin High School
4. Wilson High School
5. Pena High School

### Lowest-Performing Schools (by % Overall Passing)
These are the five schools with the lowest rate of students who passed both Math and Reading, meaning they scored less than 70% on either Math, Reading, or both:
1. Rodriguez High School
2. Figueroa High School
3. Huang High School
4. Hernandez High School
5. Johnson High School

### Math Scores by Grade
In This dataframe, math scores were grouped by grade (9th, 10th, 11th, and 12th), within each high school to see how they fluctuate over time. Teachers can compare this data with math curriculums for each grade to determine whether there are sub-subjects within math where students are falling behind or getting ahead. Overall, however, performance in math seems to remain within a 1-2% range for each school for each grade.
### Reading Scores by Grade
In This dataframe, reading scores were grouped by grade (9th, 10th, 11th, and 12th), within each high school to see how they fluctuate over time. Teachers can compare this data with reading curriculums for each grade to determine whether there are certain types of literature or writing practice where students are falling behind or getting ahead. Overall, however, performance in reading seems to remain within a 1-2% range for each school for each grade.
### Scores by School Spending
As mentioned earlier, not all schools are schools are created equal - especially when it comes to funding. I used binning to group schools by their spending range per student to determine what degree of influence money has on student success. Spending ranges include:
* Less than $585 per student
* $585-$630 per student
* $630-$645 per student
* $645-$680 per student
### Scores by School Size
Here I used binning to group schools by student count. Using this metric, I was able to compare the academic success of students at smaller schools versus larger ones. School size ranges are defined as follows:
* Small - fewer than 1000 students
* Medium - 1000 to 2000 students
* Large - 2000 to 5000 students
### Scores by School Type
Finally, I grouped schools by type. This dataframe compares average test scores in district schools versus charter schools.
