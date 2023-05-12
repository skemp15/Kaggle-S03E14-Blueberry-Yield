# Predicting Blueberry Yield

## Introduction

This repository contains my entry for the Season 3, Episode 14 Kaggle competition, which aims to predict blueberry yield. The goal of the competition is to use various features related to the blueberry crop and environmental conditions to predict the yield of blueberries.

## Problem Statement

The task is to build a predictive model that can accurately estimate the yield of blueberries given various features related to the blueberry crop and environmental conditions. The dataset provided includes information on various features such as clone size, bee density, temperature, rainfall, and fruit characteristics. The model should be able to predict the yield with the lowest possible mean absolute error score.

## Data Analysis

To prepare the data for modeling, I began by performing exploratory data analysis to get an idea of the distribution of the various features and their relationships with the target variable. I binned some continuous features into categories and encoding these features into numerical features. I also dropped features with high collinearity to reduce the number of features and prevent overfitting.

## Modelling

After preprocessing the data, I built several models using various machine learning algorithms, including Random Forest Regressor, Gradient Boosting Regressor, and XGBoost. I evaluated the models using k-fold cross-validation and Optuna, and compared their mean absolute error scores to select the best-performing model.

## Results

The best-performing model was the Random Forest model, which achieved a mean absolute error score of 355.35. The results demonstrate that the various features related to the blueberry crop and environmental conditions can be used to accurately predict the yield of blueberries, with total_seeds (seeds * fruitset), fruitset, seeds and total_mass (fruitmass * fruitset) the most important features for the model. 

## Conclusion
Overall, this Kaggle competition provided a great opportunity to work on a real-world data science problem and learn new techniques for feature engineering, data preprocessing, and model selection. By carefully analysing the data, binning some continuous features into categories and encoding them, dropping features with high collinearity, and building several models and comparing their mean absolute error scores, I was able to develop an accurate predictive model that can help farmers estimate the yield of their blueberry crops.