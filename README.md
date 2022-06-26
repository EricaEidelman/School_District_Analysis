# PyCity Schools with Pandas

## Project Overview
The purpose of this project was to conduct an analysis of reading and math scores and passing percentages for a district's high schools and then provide a summary to be used for budgeting and strategic planning purposes. Upon finishing the analysis, it was discovered that one school's ninth grade scores had been tampered with; the scores were removed and the analysis rerun.

## Resources
Data Source: students_complete.csv, schools_complete.csv

Software: Python 3.7.6

## Results
Removing the altered scores resulted in the following changes:
- The district summary was affected in the following ways:
  - The average math score fell to 78.9 from 79.
  - The average reading score remained the same at 81.9. 
  - The percent passing math fell to 74.8% from 75%.
  - The percent passing reading fell to 85.7% from 86%.
  - The percent passing overall fell to 64.9% from 65%.
 
Below are images of the district summary before and after the score replacement.

![This is an image](https://github.com/EricaEidelman/School_District_Analysis/blob/main/Initial_district_summary.png)

![This is an image](https://github.com/EricaEidelman/School_District_Analysis/blob/main/Revised_district_summary.png)

- The overall school summary was affected only in the row relating to Thomas High School:
  - The average math score fell from 83.42 to 83.35.
  - The average reading score increased from 83.85 to 83.90.
  - The percent passing math fell from 93.27% to 93.19%.
  - The percent passing reading fell from 97.31% to 97.02%.
  - The percent passing overall fell from 90.95% to 90.63%.
- Thomas High School's performance relative to the other schools was affected in the following ways:
  - When ranked on the average math score, Thomas High School fell two places behind Shelton and Griffin High Schools.
  - When ranked on the average reading score, Thomas High School's ranking did not change.
  - When ranked on the percent passing math, Thomas High School's ranking did not change.
  - When ranked on the percent passing reading, Thomas High School fell two places behind Griffin and Cabrera High Schools.
  - When ranked on the percent passing overall, Thomas High School's ranking did not change.

Below are the images of the school level summary before and after the score replacement.

![This is an image](https://github.com/EricaEidelman/School_District_Analysis/blob/main/Initial_school_summary.png)

![This is an image](https://github.com/EricaEidelman/School_District_Analysis/blob/main/Revised_school_summary.png)

The district also requested to know if the replaced scores affected the summaries of scores by grade level, school spending, size, and school type.
- Because the only changed scores were from ninth graders at Thomas High School, the summary by grade level changed to show NaN for that category of students.
- Scores by spending were slightly affected for the $631-$645 per capita spending range as that is where Thomas High School falls.
  - Average math scores fell to 78.5 from 78.51.
  - Average reading scores fell to 81.62 from 81.64.
  - The percent passing math fell to 73.46% from 73.48%.
  - The percent passing reading fell to 84.32% from 84.39%.
  - The percent passing overall fell to 62.77% from 62.86%.
- Scores by size were slightly affected for the medium size schools (1,000 to 1,999 students) as that is where Thomas High School falls.
  - Average math scores fell to 83.36 from 83.37.
  - Average reading scores rose to 83.87 from 83.86.
  - The percent passing math fell to 93.58% from 93.60%.
  - The percent passing reading fell to 96.73% from 96.79%.
  - The percent passing overall fell to 90.56% from 90.62%.
- Scores by type were slightly affected for the charte schools as that is where Thomas High School falls.
  - Average math scores and reading scores remained unchanged at 83.47 and 83.90, respectively.
  - The percent passing math fell to 93.61% from 93.62%.
  - The percent passing reading fell to 96.55% from 96.59%.
  - The percent passing overall fell to 90.39% from 90.43%.

Because of the negligible changes, the three summaries still have the same output after formatting is applied (images below).

![This is an image](https://github.com/EricaEidelman/School_District_Analysis/blob/main/Spending_summary.png)

![This is an image](https://github.com/EricaEidelman/School_District_Analysis/blob/main/Size_summary.png)

![This is an image](https://github.com/EricaEidelman/School_District_Analysis/blob/main/Type_summary.png)

## Summary
The analysis showed a number of changes to average scores and percentage rates after the problematic scores were removed. On a district level, math and reading scores and passing percentages, as well as the percent of students passing overall, all decrease. On a school level, Thomas High School saw a decrease in its math scores and all passing percentages, although the average reading scores increased. This would indicate that the ninth grade reading scores for Thomas High School were lower than for the other grade levels. 

Another change was in Thomas High School's performance relative to the other schools, as removing the ninth grade scores caused its ranking in terms of the average math score and percent of students passing reading to fall. Lastly, removing the scores affected the summaries by spending, size, and school type as almost all indicators declined for the categories Thomas High School was classified in.
