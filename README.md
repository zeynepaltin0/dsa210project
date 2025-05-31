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
  + Histogram for suicide rate (per 100k) frequency distribution.
  + Histogram for happiness scores frequency distribution.

+ Bivariate Analysis:
  + Barplot of Average Suicide Rate by Country Ordered by Happiness Score
  + Scatterplot for happiness score versus suicide rate (per 100k)
  + Boxplot of suicide rate per 100k differentiated by sex


+ Multivariate Analysis:
  + Scatterplot for happiness score versus suicide rate (per 100k) colored by reigons
  + Scatterplot for happiness score versus suicide rate (per 100k) differentiated by sex
  + Heatmap of correlation matrix for key variables

 **Machine Learning Models**
 + Linear Regression

## Results of the Analysis
  + Univariate Analysis
     + **Distribution of suicide rates (per 100k):**
       + Most countries have relatively low suicide rates, but a few show extremely high rates, making the distribution heavily skewed to the right.

     + **Distribution of happiness scores:**
       + The happiness scores are quite evenly distributed with mild clustering around scores of 5.7 and 7.0, no extreme outliers, and no strong skew. It can be said that happiness is moderately high overall, but not perfectly uniform.

   + Bivariate Analysis
     + **Average uicide rate by country ranked by happiness score**
       + In general, lower happiness scores are associated with higher suicide rates, but there are important exceptions where countries break this pattern. This suggests that while happiness and suicide are correlated, they are not perfectly inversely related — other factors likely play a major role too.

     + **Hapiness score and suicide rate (per 100k)**
       + The plot shows a very weak negative relationship between happiness scores and suicide rates, meaning happier countries tend to have slightly lower suicide rates, but the connection is not strong. There is significant variability, suggesting other factors also heavily influence suicide rates.

      + **Suicide rate per 100k differentiated by sex**
        + Suicide rates are notably higher among males than females, with males also showing a wider range and more extreme outliers. This highlights a significant gender disparity in suicide rates.

   +  Multivariate Analysis
      + **Happiness score versus suicide rate (per 100k) by reigons**
        + The relationship between happiness and suicide rate varies widely by region, with Central and Eastern Europe showing notably higher suicide rates regardless of happiness, while other regions like Latin America and Sub-Saharan Africa maintain generally lower rates across all happiness levels. Across all regions, the data highlights that happiness scores alone are insufficient to predict suicide rates.

      + **Happiness score versus suicide rate (per 100k) differentiated by sex**
        + Gender matters a lot when examining suicide rates. Happiness score alone is not a strong predictor, especially for females. For males, higher happiness scores are slightly associated with lower suicide rates, but the relationship is very weak.

      + **Correlation matrix for key variables**
        + There is no strong simple correlation between suicide rate and happiness, family, health, or wealth. However, happiness itself is strongly positively related to family, health, and income. Thus, while happier countries are generally richer and healthier, 
        these factors alone don't seem to directly explain suicide rates in a simple, straight-line relationship.

## Findings

+ **Suicide Rates Distribution:**
  + Suicide rates are heavily right-skewed, with a few countries showing extremely high rates.

+ **Happiness Scores Distribution:**
  + Happiness scores are moderately high overall, with no major skew or extreme outliers.

+ **Happiness vs. Suicide Rates:**
  + Weak negative relationship, lower happiness is slightly associated with higher suicide rates, but the correlation is weak.

+ **Gender Differences:**
  + Males have significantly higher suicide rates than females, with greater variability and more extreme outliers.

+ **Regional Patterns:**
  + Central and Eastern Europe exhibit high suicide rates regardless of happiness; Latin America and Sub-Saharan Africa show generally low suicide rates across happiness levels.

+ **Happiness and Other Factors:**
  + Happiness is strongly correlated with family support, health, and income, but these factors do not directly explain suicide rates.

## Limitations
This data analysis is based on cross-sectional data, which limits the ability to infer causality. While happiness, GDP, family support, and health were important factors, other unmeasured variables such as cultural or societal influences may also affect suicide rates. Also regional differences highlight that results may not be universally generalizable.



  




 

  







   
