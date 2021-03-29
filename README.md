# Machine Learning Models to Predict the Deaths Associated with COVID-19
- [Problem Statement](#Problem-Statement)
- [Executive Summary](#Executive-Summary)
- [project-5-part1.ipynb contents](#project-5-part1.ipynb-contents)
- [External Research](#External-Research)
- [Summary & Outlook](#Conclusions-&-Future Steps)
- [Data Sources](#Data-Sources)

---
## Problem Statement:
COVID-19 is an emergent disease that had no historical data to guide predicting/forecasting over time. The ability to predict the progress of COVID-19 is crucial to decision making aimed at controlling the damage from the pandemic.
Our goals for this project can be divided into two parts:
(1) We want to build a regression model to predict the number of deaths caused by COVID-19 over a six-month timeframe. We are particularly interested in identifying the variables that contribute the most predictive capabilities in determining COVID-19 deaths. We will use R-squared and RMSE to evaluate our production model and aim to beat the null model.
(2) We want to take the most predictive features from our regression model and apply them to a multivariate time series model that can predict future COVID-19 deaths.
Overall, we want to utilize features from a regression model to create a time series model that can forecast the future number of deaths due to COVID-19 with an accuracy score higher than that of the null model.

---

Citations
<br>
1: https://github.com/CSSEGISandData/COVID-19

---

## Executive Summary

**METHODOLOGY**
A **data science workflow** was implemented to conduct this analysis. Firstly, the **problem statement** was defined—the JHU data needed to determine how to predict COVID-19 deaths. Next, **data scraping** was performed by locating credible sources that housed the appropriate datasets. Before beginning any analysis of the data, each individual dataset was imported to a **Pandas DataFrame**. Next, **data cleaning** was conducted to ensure that all datatypes were accurate and any other errors were fixed. Using all data from a six month period, **exploratory data analysis** was conducted to determine any parameters. Since the COVID-19 datasets contain data from all states, we narrowed our focus and selected Texas data for our analysis and used our findings to perform **data visualization**. Once all data was visualized and all statistical summaries were conveyed, **predictive statistical analysis** was conducted to describe what the distributions were and if any trends appeared in the data.  To confirm and support the observations made, **external research** about the COVID-19 and any other relevant data was conducted. Finally, well-informed **data-driven recommendations** for the COVID-19 were compiled. The most significant finding from our regression model was that confirmed cases and active cases have the largest impact on predicting COVID-19 related deaths.

**Work Flow Elements:**
- Imports and reading Data
- Exploratory data analysis
- Models testing: Null model, linear regression
- PCA
- Ridge modeling
- Lasso modelling
- Time series modeling
- Heat map
- Histograms
- Boxplots
- Scatterplots
- Software requirements: Pandas, Missingno, Sklearn, Matplotlib

### Code Contents:
- Description of the COVID-19 death data columns
- Data Import & Cleaning
- Exploratory Data Analysis
- Data Visualization
- Predictive Statistical analysis
- External Research
- Summary and Future outlook

---

## Summary & Outlook:
We found that the COVID-19 data is indeed important to predict a good score. we have build a regression model to predict the number of deaths caused by COVID-19 over a six-month timeframe. We have identified the variables that contribute the most predictive capabilities in determining COVID-19 deaths. We have used R-squared and RMSE to evaluate our production model.


**Future Outlook**

In order to achieve more reliable data-driven predictions, we will focus on the following in the future: multivariate time series analysis that incorporates the important variables identified in the regression model.

Citations
<br>
1: https://people.duke.edu/~rnau/411arim.htm
<br>
2: https://www.quantstart.com/articles/Autoregressive-Integrated-Moving-Average-ARIMA-p-d-q-Models-for-Time-Series-Analysis/

---

## External Research

We wanted to analyze the time series data. Here, due to shortage of time, we did preliminary analysis for the stationary time data for Texas only. However, we would be interested in predicting time series analysis of COVID-19 for a longer period of time. We did preliminary research and import and played with data from all 58 states. With time, we will keep on updating and working on this project.
Citations
<br>
1: https://people.duke.edu/~rnau/411arim.htm
<br>
2: https://www.quantstart.com/articles/Autoregressive-Integrated-Moving-Average-ARIMA-p-d-q-Models-for-Time-Series-Analysis/

---

## Data Sources
The sources of the datasets used in this analysis:
- [COVID-19 dataset](https://github.com/CSSEGISandData/COVID-19)
JHU data was used in this project. JHU updates the daily U.S. covid case counts on a daily basis. To acquire the data, we went to JHU's Covid-19 data repository. To ingest the data, we forked and cloned the repository to our local computers and removed any files we were not using in the project. To clean the data, our primary steps involved identifying missing values and applying the KNN imputation method.