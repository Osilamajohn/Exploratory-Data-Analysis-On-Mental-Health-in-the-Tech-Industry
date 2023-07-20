# Exploratory-Data-Analysis-On-Mental-Health-in-the-Tech-Industry


##Dataset Information

This data is from Open Source Mental Illness (OSMI) using survey data from years 2014, 2016, 2017, 2018 and 2019. Each survey measures and attitudes towards mental health and frequency of mental health disorders in the tech workplace. 


##Content

The SQLite database contains 3 tables. Survey, Question, and Answer.

Survey (PRIMARY KEY INT SurveyID, TEXT Description)
Question (PRIMARY KEY QuestionID, TEXT QuestionText)
Answer (PRIMARY/FOREIGN KEY SurveyID, PRIMARY KEY UserID, PRIMARY/FOREIGN KEY QuestionID, TEXT AnswerText)

SuveyID are simply survey year ie 2014, 2016, 2017, 2018, 2019.
The same question can be used for multiple surveys
Answer table is a composite table with multiple primary keys. SurveyID and QuestionID are FOREIGN KEYS.
