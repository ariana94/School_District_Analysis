# School_District_Analysis

## Overview
In this Analysis, we were given data by Maria to help her analyze the data on student funding and test scores. We have uncovered some academic dishonesty involving the math and reading grades for 9th graders at Thomas High School. With this information we will be redoing their district analysis to better assist the school board in making decisions regarding the school budgets and priorities.

## The Results
Here are the results of Thomas High School before we replaced the 9th grade scores:
![Org_Thomas_High](https://user-images.githubusercontent.com/19378130/174450392-a29e8a95-0a6c-4676-8eca-c3c1ce6dce11.png)

Here are the results after the replacment:
![After_Thomas_High](https://user-images.githubusercontent.com/19378130/174450487-15016f61-7b08-40df-92e3-26781984fe5a.png)


### Q&A
- How is the district summary affected?
   - Overall, it had very little affect on the district summary. It was only 461 grades that were removed which is a very small percentage in relevance to the amount of students.
- How is the school summary affected?
    - As we can see in the before and after images, it was very minimaly affected. Overall the scores were only very slightly increased (reading) or decreased (math).
- How does replacing the ninth graders' math and reading scores affect Thomas High School's performance relative to the other schools?
    - Thomas High School remained in the second spot as a top five school once the code was readjusted to ignore the NaN 9th grade scores
![Top five after](https://user-images.githubusercontent.com/19378130/174451355-21ae2225-ad78-4df5-ab44-b4d269ab35c2.png)
- How did replacing the scores affect:
  - Math and reading scores by grade
      - When sorted by grade level, it only changed that 9th grade was shown as "NaN". However, if we didn't redo our code to ignore the 9th graders when running formulas, it would show THS's passing rate as doing much worse as all the scores for 9th graders were considered to be 0 instead of ignored.
![Before](https://user-images.githubusercontent.com/19378130/174457386-43970f93-5aa8-42d8-9ae9-31abbd8322f6.png)
      - After the code was redone to only take account for the 10th to 12th graders, it showed them at almost the same levels as the original
![After](https://user-images.githubusercontent.com/19378130/174457404-25751307-c4ae-4bec-a180-b0652386a446.png)

  - Scores by school spending
      - Unaffected
      - ![Spending Ranges](https://user-images.githubusercontent.com/19378130/174457483-980f82a7-587e-469d-9a8b-7f6018679df9.png)

  - Scores by school size
      - Both were only affected by about .01, not even enough to change the formatting(Top: New, Bottom: Original)
      - ![New_scores_by_size](https://user-images.githubusercontent.com/19378130/174456768-7b8f9121-916d-4d84-a718-9e2c6c4556ab.png)
      - ![OG_scores_by_size](https://user-images.githubusercontent.com/19378130/174456773-553e8764-973a-408c-bce5-d74f8d97c764.png)

  - Scores by school type
      - Also affected by about .01, again not enough to reflect change after formatting (Top: New, Bottom: Original)
      - ![New_scores_by_type](https://user-images.githubusercontent.com/19378130/174456825-2068abda-07ad-4b34-9de6-e9a5a89a8e32.png)
      - ![OG_scores_by_type](https://user-images.githubusercontent.com/19378130/174456830-9b71c5bd-db38-4a24-8c66-1ece37bd78b9.png)

## Changes Summary
Once the grades for the 461 9th grade students were set to NaN, and the calculations and formulas set to ignore the 9th graders non-existant scores Thomas High School was shown as performing at the same levels as the original district analysis. Prior to the calculations and formulas being updated, THS had dropped from 2nd to 8th in ranking of % Overall Passing. They went from an original 93.27% to a redone 66.91% to an updated 93.19% of students passing math and an original 97.31% to a redone 69.66% to an updated 97.02% of students passing reading. This calculated out to an original 90.95% to a redone 65.08% and an updated 90.63% overall passing rate.
