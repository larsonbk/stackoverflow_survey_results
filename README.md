# stackoverflow_survey_results

## Installations:
* Pandas
* Numpy
* Matplotlib
* Seaborn

## Business Understanding
I wanted to know what some variables were involved in knowing a developer's Job and Career Satisfaction. In my current role, understanding unit costing and the cost to replace individuals is very high. Good developers are extremely important to furthering my company's future goals. Knowing some of the variables that go into what keeps developers happy is vital to understanding why some developers leave. Furthermore, understanding if companies are at a dissadvantage for simply being the company that they are will help to understand if additional offered benefits are required to keeping good developers. 

The questions that I want answered are:
1. What company type has the the highest career satisfaction rate for developers?
2. What company type has the the highest job satisfaction rate for developers?
3. What company types have the most developers working from home?
4. If job satisfaction for developers is attributed to Auditory Environment?

## Data Understanding
I am using the 2019 Stackoverflow Survey results which contains nearly 90,000 respondents. You can find the link to the data here [https://insights.stackoverflow.com/survey]. This survey provided 154 variables that help understand many of the differences between people that code.

## Data Preperation
Because my questions are based specifically on developers, I removed all data rows where the respondent did not identify as a developer.

I created 3 dataframes for the different groups to answer the different questions. For my developer dataframe, I dropped all rows where the respondent did not select a company type. I decided to leave the answers, "I don't know", "I prefer not to say", and "Something else" because these answers may be valuable in the analysis. I did not want to remove too many rows, I decided to replace any NaNs with the mean values for both Job and Career Satisfaction. I then converted those responses to integers to assist with analysis.

For the auditory dataframe and remote work dataframe, I decided that I would drop any row where the respondent did not identify those variables.

## Modeling
The questions that I had about the data did not require modeling.

## Evaluation
Developers who work for startups generally have a higher Job and Career satisfaction than developers from other types of companies. They are also more likely to be able to work remotely. For better job satisfaction, developers prefer to have no background noise or listen to music.

## File Descriptions
The analysis work was completed in a Jupyter Notebook named: survey_results.ipynb. There is also an html file with the same information called: survey_results.html

