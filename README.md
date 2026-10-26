# correlation-between-education-and-career
הקובץ מכיל נתונים על קריירה של עובדים והצלחתם בשוק העבודה, תוך התמקדות בקשרים בין סוגי ההשכלה שהשיגו לבין הצלחתם המקצועית. המידע שבקובץ כולל פרטים על מקצועותיהם של העובדים, רמות השכר שלהם, רמות ההשכלה (תיכון, אקדמאי, תארים נוספים), גילם, מגדרם, תחום העיסוק ועוד

## Project files
- [`education_career_analysis.ipynb`](education_career_analysis.ipynb): the full analysis notebook (EDA course project by Aharon). It reads the data straight from this repository.
- [`job_placement.csv`](job_placement.csv): 700 Bachelor's graduates with field of study, college, GPA, years of experience, gender, age, whether they were hired, and salary.

## Research questions
1. Does work experience change the chance of getting hired?
2. Do students with higher grades get hired more often?
3. Does the university you went to affect your chance of getting hired?
4. Among those hired, do better grades mean a higher salary?
5. Are some fields of study easier to get hired in or better paid?
6. Is there a gender gap in hiring or salary?

Deeper questions that combine three or more columns:

7. Is there a gender gap that the overall numbers hide (gender × college × field × hiring)?
8. Which colleges pay more or less than their graduates' GPA and experience predict?
9. When every column goes into one model, how much of the salary does each one explain?

## Key insights
1. **Where you studied decides whether you get hired.** Most universities placed 97% of their graduates, while three (Penn, UNC Chapel Hill, UC Riverside) placed only 4%, even though their students' grades are just as good.
2. **Experience and grades only look like they matter for hiring.** Overall, 3 years of experience seems to lift the hiring rate from 70% to 97%, but inside each group of colleges experience makes no difference. The colleges that hardly place anyone simply have no students with 3 years of experience (a confounding variable).
3. **College also sets the salary, and grades add only a small bonus.** All columns together explain 94% of salary differences, and college alone explains about 63%. With the same GPA and experience, Delaware graduates earn about $2,000 more than predicted and Rochester graduates about $3,300 less. GPA still adds about $480 per 0.1 point.

Also found along the way: outside the three low-placement colleges, all 134 men were hired while 9 of 151 women were not (p = 0.004), a gap hidden in the overall numbers. Field of study, gender overall and age made no significant difference.

## How to run
```bash
pip install pandas numpy matplotlib seaborn scipy statsmodels jupyter
jupyter notebook education_career_analysis.ipynb
```
