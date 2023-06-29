# H1N1 Vaccine Uptake: Learning From the Past to Inform the Future

## Project Overview

The aim of this study is to predict uptake likelihood of the H1N1 (swine flu) vaccine.  We believe our prediction outputs modelling predictions and subject area-informed analysis of this study will give public and private health professionals a clear understanding of factors associated with high and low vaccination uptakee. This enables stakeholders to focus on demonstrated successes while improving upon unsuccessful areas.

We used the survey data from the CDC's National Flu Survey (NHFS, 2009) to predict whether or not respondents got the H1N1 vaccine. It is important to understand past vaccination patterns in order to understand those of more recent pandemics, such as COVID-19. The most influential factors determining vaccination status are found to be Doctor Recommendation of H1N1 vaccine, Age, Health Insurance Status, Opinion of H1N1 Vaccine Effectiveness, and Opinion of H1N1 Risk by our final model. 

## Data Overview

This data comes from a NHFS National Flu Survey from 2009, which inquires about whether or not people received the seasonal flu and/or the H1N1 flu vaccination, as well as their demographic, behavioral, and health factors. There are 26,000 respondents in the data we used, though over a million respondents on the final survey.  In this project we chose H1N1 vaccination rate as our target variable. We used all features in the survey, and filled missing values using the Iterative Imputer.

## Methods

We used four machine learning models to make our predictions, settling on GridSearchCV-tuned HistGradientBoostingClassifer with SMOTE re-sampling from Sci-Kit Learn.. We paid special attention to test scores, since overfitting on imbalanced data is a major concern. F1, confusion matrices, and ROC-AUC scores were also important, again given the data imbalances and types.

## Project Results

We looked into the model's feature importances to understand the relationship between the features and vaccination behavior. We saw that the demographic and behavioral features are not that important compared to health related factors and opinions, although demographic information was often missing or encoded. Doctor recommendation, middle age (45-54),  health insurance status, opinion of vaccine efficiency, and opinion of H1N1 risk are the top important factors in determining people's vaccination status.


## Conclusion

We recommend that public health officials at the American Public Health Association (APHA) communicate to doctors the importance of recommending to patients that they get the H1N1 vaccine. We also recommend that they find a way to make the vaccine accesible to people regardless of health insurance status. Additionally, because opinion on H1N1 vaccine effectiveness and H1N1 risk to health are highly influential in determining vaccination status, we recommend that public health stakeholeders make educational outreach a priority, especially in the wake of extreme mis-information.

## Next Steps

For our next steps, we would like to look at more recent survey data, so as to get the most recent results, and integrate this with the original data. We would also like to do more data clearning, imputation , and feature engineering to improve results. Lastly, since we chose to focus only on predicting H1N1 vaccination status, we would like to focus in the future on predicting not only H1N1 and seasonal flu vaccination, but the particular combinations thereof, using enhanced data manipulation and modeling techniques.


## Repository Navigation

### Data:
- https://www.drivendata.org/competitions/66/flu-shot-learning/page/213/

### Survey Info:
- https://www.cdc.gov/nchs/nis/data_files_h1n1.htm
- https://www.cdc.gov/flu/fluvaxview/coverage_0910estimates.htm


### Notebooks
- Final notebook: https://github.com/Lou-Hines/H1N1_and_Seasonal_Flu_Vaccine_Prediction_2009/blob/main/H1N1%20Vaccine%20Final%20Notebook.ipynb


### Presentation

https://github.com/Lou-Hines/H1N1_and_Seasonal_Flu_Vaccine_Prediction_2009/blob/main/H1N1%20Vaccine%20Uptake%20.pdf

### Contact

lou.m.hines@gmail.com
