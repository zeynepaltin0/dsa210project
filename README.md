# Dsa210 Project

## Project Overview
In this project , I will analyze suicide rates across countries from 2015 to 2016 and explore how socio-economic factors (e.g., GDP) and happiness indicators (e.g., social support, freedom, corruption) influence these rates. By combining two datasets—Suicide Rates Overview and World Happiness Report— I aim to uncover patterns, correlations, and potential predictors of suicide rates. 

## Motivation
This project will provide valuable insights into the factors influencing suicide rates globally. The findings can be used by policymakers, mental health organizations, and researchers to develop targeted interventions and strategies to reduce suicide rates.

This project can also be hope and a reminder that suicide is caused by many factors and is in fact preventable for people.

## Description of Datasets
I will be using two different datasets for this project:

**1. Suicide Rates Overview 1985 to 2016**  
 Contains suicide rates by country, year, age group, and gender, along with socio-economic data like GDP per capita and HDI.  
 Source: https://www.kaggle.com/datasets/russellyates88/suicide-rates-overview-1985-to-2016

**3. World Happiness Report**  
    Provides happiness scores and related factors (e.g., social support, freedom, corruption) by country and year.  
    Source: https://www.kaggle.com/datasets/unsdsn/world-happiness?select=2019.csv  

## Plan
**Data Preparation:**

+ Both datasets will be clean and preprocessed.  
+ Datasets weill be merged through country and year (if necessary).

**Exploratory Data Analysis (EDA):**

+ Visualizing trends in suicide rates over time and across countries.  
+ Exploring correlations between suicide rates and socio-economic/happiness factors.  
+ Analyzing differences in suicide rates by age group and gender.  

**Statistical Analysis And Machine Learning:**
   
+ Statistical models and predictive machine learning methods will be applied.

# Report
## Introduction

This report investigates that whether the countries with higher happiness scores tend to have lower suicide rates, even after controlling for economic and demographic variables (between year 2015-2016). By integrating data from global suicide statistics and world happiness reports, we aim to uncover potential patterns and associations between societal well-being and suicide prevalence. The findings could offer valuable insights for policymakers, mental health professionals etc.

## Hypothesis
Null Hypothesis (H₀): There is no significant relationship between happiness scores and suicide rates after controlling for economic and demographic variables.

Alternative Hypothesis (H₁): There is a significant relationship between happiness scores and suicide rates after controlling for economic and demographic variables.

## Methods 
**Data Collection**
I got both of my datasets from kaggle.

**Datasets**
1) Suicide Rates Overview 1985 to 2016 , which inlcudes: country, year, sex, age group, count of suicides, population, suicide rate, country-year composite key, HDI for year, gdp_for_year, gdp_per_capita, generation (based on age grouping average).
2) World Happiness Report (I used only years 2015 and 2016), which includes:

   For 2015: Country, Region, Happiness Rank, Happiness Score, Standard Error, Economy (GDP per Capita), Family, Health (Life Expectancy), Freedom, Trust (Government Corruption), Generosity, Dystopia Residual.

   For 2016: Country, Region,Happiness Rank, Happiness Score, Lower Confidence Interval, Upper Confidence Interval, Economy (GDP per Capita), Family, Health (Life Expectancy), Freedom, Trust (Government Corruption), Generosity, Dystopia Residual.

**Data Preprocessing**
+ Checked the data for missing values and duplicates for all datasets.
+ Deleted unncessesary columns.
+ Merged all datasets into one by year and countries.
+ Deleted unmatched rows after merging.
+ Converted the data into the  appropriate format.

**Visualization Techniques**
+ Univariate Analysis:
  + Histogram for suicide rate per 100k frequency distribution.
  + Histogram for happiness scores frequency distribution.

+ Bivariate Analysis:
  + Barplot of Average Suicide Rate by Country Ordered by Happiness Score
  + Scatterplot for happiness score versus suicide rate per 100k
  + Boxplot of suicide rate per 100k differentiated by sex


+ Multivariate Analysis:
  + Scatterplot for happiness score versus suicide rate per 100k colored by reigons
  + Scatterplot for happiness score versus suicide rate per 100k differentiated by sex
  + Heatmap of correlation matrix for key variables

 **Machine Learning Models**
 + Linear Regression
  







   
