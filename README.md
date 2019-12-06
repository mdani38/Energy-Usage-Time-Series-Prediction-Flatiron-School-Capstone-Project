# Energy Usage Prediction

## Flatiron School Capstone Project

### Author: Matthew Danielson

This project is the capstone project for the Data Science Bootcamp at the Flatiron School. It is based on the kaggle competition ASHRAE Great Energy Predictor III. https://www.kaggle.com/c/ashrae-energy-prediction

## Presentation and visualizations

https://www.canva.com/design/DADs4iXg2PA/2skAA-7X3OdjeMpL2KuWuA/view?utm_content=DADs4iXg2PA&utm_campaign=designshare&utm_medium=link&utm_source=sharebutton

### Tableau dashboards

https://public.tableau.com/profile/matthew.danielson#!/vizhome/ASHRAEWeather/Temperatures?publish=yes

https://public.tableau.com/profile/matthew.danielson#!/vizhome/ASHRAE_Preds/3Preds

https://public.tableau.com/profile/matthew.danielson#!/vizhome/ASHRAE_Update/Meter_Predictions

https://public.tableau.com/profile/matthew.danielson#!/vizhome/ASHRAE_4/PrimaryUse_1


## Data 

The data must be accessed by going to the below link and accepting the kaggle rules to download the data. After doing so, put the data files into a folder called ashrae-energy-prediction and the notebooks will all run correctly.

https://www.kaggle.com/c/ashrae-energy-prediction/data

## Background

Buildings have been retrofit with energy saving improvements with a payment plan relative to difference in real consumption and predicted values. Accurate models are required to predict energy consumption as if improvements were never made. 

## Data Exploration

The training dataset contains a year of data (January - December 2016) with corresponding energy meter readings in kilowatt hours. There are 1449 separate buildings and 4 different meter types. 

The testing data contains a year and a half of data (January 2017 - May 2018).

There is attached building metadata that contains fields such as use type, number of floors and square footage. The buildings are split into 16 different sites but without any attached geographic data. 

Weather data is provided for both the training and testing time periods. The weather is tied to the different sites but the time is standardized due to the anonymized site ids. For modeling, the weather data was time shifted so peak temperature is at 3 pm for each site.

## Models

Below models are associated with similarly named notebooks. The notebooks for splitting csv is required for the GRU notebooks.

### Median Predictions: RMSLE 1.61
### GRU: RMSLE 2.66
### LGBM with Full FE: RMSLE 1.14
### LGBM with Light FE: RMSLE 1.12
### LGBM Half and Half: RMSLE 1.09

