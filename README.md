# CodeX-Energy-Drink-Market-Analysis
Based on their survey, the German beverage firm CodeX requested a marketing analysis on how to increase brand recognition, market share, and product development. This project is a challenge given by codebasics.
# Presentation Link:
          https://youtu.be/IkQJBP6KJKo

# Data Cleaning and Analysis using Sql

## Genderwise respondents
SELECT count(Gender) GenderNum,Gender FROM fnbmarketing.dim_repondents
group by Gender
order by GenderNum;

## tried before =0
UPDATE fact_survey_responses
SET Tried_before = "No"
WHERE Heard_before ="No"; 

UPDATE fact_survey_responses
SET Taste_Experience = 0
WHERE Tried_before ="No"; 
