# Predict Carbon Emissions in Rwanda

## Overview

The ability to accurately monitor carbon emissions is a critical step in the fight against climate change. Precise carbon readings allow researchers and governments to understand the sources and patterns of carbon mass output. While Europe and North America have extensive systems in place to monitor carbon emissions on the ground, there are few available in Africa.

The objective of this challenge is to create a machine learning models using open-source CO2 emissions data from Sentinel-5P satellite observations to predict future carbon emissions.

These solutions may help enable governments, and other actors to estimate carbon emission levels across Africa, even in places where on-the-ground monitoring is not possible.

This challenge is part of 2023 edition of Kaggle's Playground Series, i.e. [Season 3 - Episode 20](https://www.kaggle.com/competitions/playground-series-s3e20/overview).

## Dataset Description

The objective of this challenge is to create machine learning models that use open-source emissions data (from Sentinel-5P satellite observations) to predict carbon emissions.

Approximately 497 unique locations were selected from multiple areas in Rwanda, with a distribution around farm lands, cities and power plants. The data for this competition is split by time; the years 2019 - 2021 are included in the training data, and your task is to predict the CO2 emissions data for 2022 through November.

Seven main features were extracted weekly from Sentinel-5P from January 2019 to November 2022. Each feature (Sulphur Dioxide, Carbon Monoxide, etc) contain sub features such as column_number_density which is the vertical column density at ground level, calculated using the DOAS technique. You can read more about each feature in the below links, including how they are measured and variable definitions. You are given the values of these features in the test set and your goal to predict CO2 emissions using time information as well as these features.

The provided dataset contains 103376 entries, each with 76 features. The model will be tested on 24353 entries. The dataset files can be found under the Data folder in this repository.

## Implementation

The current version of the model uses Random Forest Regression and achieved a RMSE score of around 31. Full notebook which contains all necessary steps (i.e. EDA, Feature Engineering, Model Selection, Fine-tuning Parameters, Evaluation) can be found under the Main folder in this repository. 
