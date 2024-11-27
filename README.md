# Helios: Project Progress Report

## Overview

This README provides an overview of our current progress on the Helios project, focusing on the team's work, challenges, and next steps.

## Team Members

Jacob Bachtarie

Nikolas Velazquez 

Tam Nguyen 

Braddock Mitchell Parks 

## Project Goals

The goal of the Helios project is to develop and implement methods to analyze spatial data and identify potential hotspots. We are utilizing Python to develop kernel density function methods and applying K-Nearest-Neighbor (KNN) as one of our primary analysis techniques.

## Current Progress

The team has divided the tasks among all members, focusing on understanding the dataset and developing kernel density functions.

For those new to Python, time has been allocated for learning and familiarizing with libraries like NumPy, Seaborn, and Matplotlib to perform data analysis and visualization.

We have made significant progress on developing initial models and are in the process of creating visual representations to accompany our findings using Seaborn and Matplotlib.

## Hotspot Discovery Algorithm

We are actively discussing approaches for implementing a hotspot discovery algorithm.

Our current plan involves examining intensity percentiles to determine areas that could be classified as significant hotspots.

We are evaluating several methods, including Kernel Density Estimation, to determine which approach will provide the best results for our specific dataset.

# Implementation Details

## Data Analysis and Preprocessing

We used Python libraries such as Pandas and NumPy for data analysis and preprocessing.

Data visualization was performed using Matplotlib and Seaborn, which helped in understanding trends and distributions within the dataset.

## Models Implemented

Model 1: XGBoost Regressor (XGBRegressor) was used with parameters such as learning rate = 0.248, max depth = 10, and n_estimators = 546. The target variable was total.counts, and the input features included attributes like duration.s, peak.c/s, and energy.kev.i.

Model 2: RandomForest Regressor was applied after adding an intensity attribute to the dataset. The intensity was calculated as the average energy multiplied by the duration. The target variable for Model 2 was intensity, and input features included temporal and spatial attributes.

## Model Performance

XGBoost Regressor (Model 1): Mean MAE was 138029.805 (17625.737).

RandomForest Regressor (Model 2): Mean MAE was 4162.393 (193.812).

Several other regression models were implemented for comparison, including Support Vector Regressor (SVR), Ridge Regression, and Linear Regression. The performance of these models was evaluated using Mean Absolute Error (MAE), and the results were documented for each approach.

## Visual Representations

Visualizations were created using Seaborn and Matplotlib to better understand the relationships between features and target variables. These visualizations are integral to interpreting model performance and making decisions about feature engineering.

## Challenges
Re-evaluating Assumptions: There is a need to re-evaluate assumptions made about the dataset to ensure that the models and methods used are appropriate for the data characteristics and distributions.
Time Management: Limited time availability is proving to be a constraint for effective collaboration and task completion.

## Next Steps

Complete the implementation of the K-Nearest-Neighbor method and begin evaluation of its effectiveness.

Finalize the hotspot discovery algorithm and determine the thresholds for classifying high-intensity regions.

Continue developing visual representation tools to aid in communicating our findings.

## Technologies Used

Python: For data analysis and model development.

Jupyter Notebooks: For interactive coding and sharing insights.

Seaborn and Matplotlib: For visualization of data and model results.

XGBoost, RandomForest, SVR, Ridge Regression: For building and evaluating predictive models.
