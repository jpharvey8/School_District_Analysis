# School_District_Analysis
## Overview of the school district analysis 

### Purpose: 
The purpose of this analysis is to find the overall passing percentages of the students and find a correlation with the buget per student, if any. While analyzing the data, we noticed that there were missing 9th grade test scores from Thomas High School. We had to go back through and reevaluate all of the scores from the high school because there was a chance it would skew the overall numbers and percentages.

### Resources
Pandas & Numpy libraries Jupyter Notebook (PythonData environment created using Python 3.7 and Anaconda)
csv’s provided: schools_complete.csv, students_complete.csv

## Results 
### How is the district summary affected?
When comparing the disctrict summaries from the pycityschools and pyscityschools_challenge, the total schools and total students numbers are not affected. The average math score decreased from 79.0 to 78.9 and the average reading score decreased by 0.1%. The overall passing percentage decreased by 0.3%. 

### Fig 1: District summary before removing Thomas High School 9th grade scores 
<img width="364" alt="2022-01-02 (1)" src="https://user-images.githubusercontent.com/92167429/147890229-1c064052-86db-4aa2-9f09-0effa3296724.png">

### Fig 2: District summary after removing Thomas High School 9th grade scores 
<img width="357" alt="2022-01-02 (2)" src="https://user-images.githubusercontent.com/92167429/147890246-bddf5bfd-14ca-41a9-844e-bb914c74ea95.png">


### How is the school summary affected? 
The school summary dataframe changes only with regard to Thomas High School since we are still using the total number of students in each school to calculate the percentage of students that pass math, reading, and math and reading together at each school. 

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
There was a slight difference in average math and reading score, percent passing math and reading and overall passing percentage. The difference was less than 1% and did not shift the 2nd to top school rank that it held before or after removing the 9th grade scores. 

### Fig 3: Top 5 schools prior to removing Thomas High School 9th grade scores 
<img width="543" alt="2022-01-02 (4)" src="https://user-images.githubusercontent.com/92167429/147890613-e2f053d2-ea68-492f-b532-78fa8fdd21ef.png">

### Fig 4: Top 5 schools after removing Thomas High School 9th grade scores 
<img width="530" alt="2022-01-02 (5)" src="https://user-images.githubusercontent.com/92167429/147890615-8da40e14-b92d-485f-ac76-9b2152ff3ff5.png">

### How does replacing the ninth-grade scores affect the following:

### Math and reading scores by grade? 
The math and reading scores for all other schools are not affected when the Thomas High School 9th grade scores are removed. The scores for Thomas High School are voided and replaced with NAN. 

### Fig 5: Math scores by grade 
### Before removing Thomas High School 9th grade scores 
<img width="161" alt="2022-01-02 (6)" src="https://user-images.githubusercontent.com/92167429/147890990-b803a9f6-d0b6-463c-9616-75001db3cf74.png">

### After removing Thomas High School 9th grade scores 
<img width="228" alt="2022-01-02 (7)" src="https://user-images.githubusercontent.com/92167429/147891045-71c60feb-dc0a-4869-96a5-0cd3c2d14a22.png">

### Fig 6: Reading scores by grade 
### Before removing Thomas High School 9th grade scores 
<img width="174" alt="2022-01-02 (8)" src="https://user-images.githubusercontent.com/92167429/147891093-a5158bf8-813d-4b77-88c8-3c3b77271967.png">

### After removing Thomas High School 9th grade scores 
<img width="242" alt="2022-01-02 (9)" src="https://user-images.githubusercontent.com/92167429/147891132-74c91582-c04c-4b2d-9057-43f38ea63b4f.png">

### Scores by school spending? 
The only bin that was affected was the bin containing Thomas High School. Since Thomas High School's per student budget is $638, this is the $630-640 bin. 

### Scores by school size? 
Thomas High School has 1,635 students so it is categorized as a Medium School Size. There was no change in school size after removing Thomas High School 9th grade scores. 

### Fig 7: Summary by school size prior to removing Thomas High School 9th grade scores 
<img width="402" alt="2022-01-02 (11)" src="https://user-images.githubusercontent.com/92167429/147891576-66f26628-2026-4b06-9891-7a4affbfaf1e.png">

### Fig 8: Summary by school size after removing Thomas High School 9th grade scores  
<img width="386" alt="2022-01-02 (12)" src="https://user-images.githubusercontent.com/92167429/147891612-49fb9c97-0379-412c-8263-f45b1c232a23.png">

### Scores by school type?
There is no change in scores by school type. 

### Fig 9: Summary by school type prior to removing Thomas High School 9th grade scores 
<img width="352" alt="2022-01-02 (13)" src="https://user-images.githubusercontent.com/92167429/147891674-c0a62f50-03d7-4013-863b-9685f6f5cfcc.png">

### Fig 10: Summary by school type after removing Thomas High School 9th grade scores 
<img width="374" alt="2022-01-02 (14)" src="https://user-images.githubusercontent.com/92167429/147891697-bd8fb151-31f8-4ed1-85a1-58e945ec7fd3.png">

## Summary
There weren't any significant changes after replacing the scores of the 9th grade students. The scores that may have altered size, district, spending and overall passing percentage have been voided. 



