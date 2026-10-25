# correlation-between-education-and-career
הקובץ מכיל נתונים על קריירה של עובדים והצלחתם בשוק העבודה, תוך התמקדות בקשרים בין סוגי ההשכלה שהשיגו לבין הצלחתם המקצועית. המידע שבקובץ כולל פרטים על מקצועותיהם של העובדים, רמות השכר שלהם, רמות ההשכלה (תיכון, אקדמאי, תארים נוספים), גילם, מגדרם, תחום העיסוק ועוד

## Project files
- [`education_career_analysis.ipynb`](education_career_analysis.ipynb): the full analysis notebook (EDA course project). It reads the data straight from this repository.
- [`job_placement.csv`](job_placement.csv): 700 Bachelor's graduates with field of study, college, GPA, years of experience, gender, age, whether they were hired, and salary.

## Research questions
1. Does work experience change the chance of getting hired?
2. Do students with higher grades get hired more often?
3. Does the university you went to affect your chance of getting hired?
4. Among those hired, do better grades mean a higher salary?
5. Are some fields of study easier to get hired in or better paid?
6. Is there a gender gap in hiring or salary?

## Key insights
1. **Where you studied decides whether you get hired.** Most universities placed 97% of their graduates, while three (Penn, UNC Chapel Hill, UC Riverside) placed only 4%, even though their students' grades are just as good.
2. **Experience and grades only look like they matter for hiring.** Overall, 3 years of experience seems to lift the hiring rate from 70% to 97%, but inside each group of colleges experience makes no difference. The colleges that hardly place anyone simply have no students with 3 years of experience (a confounding variable).
3. **Grades pay off in salary.** Among those hired, each extra 0.1 GPA point is worth about $480 more per year, even when comparing graduates of the same college with the same experience.

Field of study and gender showed no significant difference in hiring or pay.

## How to run
```bash
pip install pandas numpy matplotlib seaborn scipy statsmodels jupyter
jupyter notebook education_career_analysis.ipynb
```
