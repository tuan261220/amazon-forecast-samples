# Amazon Forecast Samples

Workshops, Notebooks and examples on how to learn and use various features of Amazon Forecast

### Introduction, Best Practices, and Cheat Sheet Tutorial

[Getting Started Guide and Best Practices Cheat Sheet Tutorial](https://github.com/aws-samples/amazon-forecast-samples/blob/master/ForecastCheatSheet.md) serves as a guide to onboarding and continued learning how to improve forecasts using Amazon Forecast Best Practices.

<br>

### Workshops

- **[Pre-POC workshop](https://github.com/aws-samples/amazon-forecast-samples/tree/master/workshops/pre_POC_workshop)** is a hands-on, leave-in-place, guided learning (and demo) that is meant to accelerate a Forecast POC.  The workshop covers Best Practices for working with Amazon Forecast.  Targeted to Developers, Line-of-business, and Data Scientists who will be doing the execution work of a Forecast POC.  
  - Data used:  NYC Taxi
  - Resources used:  
    - [Getting Started Guide and Best Practices Cheat Sheet Tutorial](https://github.com/aws-samples/amazon-forecast-samples/blob/master/ForecastCheatSheet.md)
    - [Improving Forecast Accuracy with Machine Learning Solution](https://github.com/aws-samples/amazon-forecast-samples/blob/master/workshops/pre_POC_workshop/install-forecast-solution.md)
- **No code workshop** can be used in 2 ways:
  - [**Introduction demo**](https://github.com/aws-samples/amazon-forecast-samples/blob/master/workshops/no_code_workshop/forecast-with-console.md).  Developers and Line-of-business folks can follow-along this markdown file to learn start-to-finish how to create forecasts.  100% no-code, through UI screens using console only.  
  - **[Notebook using Amazon Forecast Python SDK](https://github.com/aws-samples/amazon-forecast-samples/blob/master/workshops/no_code_workshop/forecast-with-api-completed.ipynb)** to make API calls to perform exactly the same tasks as the 100% no-code demo.  Targeted at Integration Partners, MLOps Engineers, and Developers responsible for putting forecasts into production.
  - Data used:  Energy consumption
- Immersion Day Workshop is an older version of the No code workshop notebook portion.

<br>

## Notebooks

This folder is mainly for Integration Partners, MLOps Engineers, and Developers.  Here you will find examples how to use Amazon Forecast Python SDK to make API calls to use when putting forecasts into production.

- Basic folder contains introductory notebooks to show API calls to:
  - [import data containing 1 single item](https://github.com/aws-samples/amazon-forecast-samples/blob/master/notebooks/basic/Tutorial/1.Getting_Data_Ready.ipynb)
  - [train a predictor and forecast on a single item](https://github.com/aws-samples/amazon-forecast-samples/blob/master/notebooks/basic/Tutorial/2.Building_Your_Predictor.ipynb)
  - [query and evaluate one item at a time](https://github.com/aws-samples/amazon-forecast-samples/blob/master/notebooks/basic/Tutorial/3.Evaluating_Your_Predictor.ipynb)
- Advanced folder contains notebooks to show API calls for more complex tasks:
  - [Evaluating your predictor using backtest item-level forecasts](https://github.com/aws-samples/amazon-forecast-samples/blob/master/notebooks/advanced/Item_Level_Accuracy/Item_Level_Accuracy_Using_Bike_Example.ipynb) 
  - [Running an experiment without re-training by API call](https://github.com/aws-samples/amazon-forecast-samples/blob/master/notebooks/advanced/WhatIf_Analysis/WhatIf_Analysis.ipynb)
  - [Adding built-in AWS-hosted weather data](https://github.com/aws-samples/amazon-forecast-samples/tree/master/notebooks/advanced/Weather_index) 
  - [Adding Related data](https://github.com/aws-samples/amazon-forecast-samples/blob/master/notebooks/advanced/Incorporating_Related_Time_Series_dataset_to_your_Predictor/Incorporating_Related_Time_Series_dataset_to_your_Predictor.ipynb) 
  - [Adding Metadata](https://github.com/aws-samples/amazon-forecast-samples/blob/master/notebooks/advanced/Incorporating_Item_Metadata_Dataset_to_your_Predictor/Incorporating_Item_Metadata_Dataset_to_your_Predictor.ipynb) 
  - [Forecasting "cold-start" or new product introductions by generating test data explicitly filled with "NaN" for new items and running Forecast-only (that is inference only) using already trained predictor](https://github.com/aws-samples/amazon-forecast-samples/blob/master/notebooks/advanced/Forecast%20with%20Cold%20Start%20Items/Forecast%20with%20Cold%20Start%20Items.ipynb) 

<br>

## MLOps 

This folder has been superceded by the [Improving Forecast Accuracy With Machine Learning Solution](https://aws.amazon.com/solutions/implementations/improving-forecast-accuracy-with-machine-learning/).  [Follow these instructions](https://github.com/aws-samples/amazon-forecast-samples/blob/master/workshops/pre_POC_workshop/install-forecast-solution.md) to deploy an automated end to end pipeline from training to visualization of your Amazon Forecasts in Amazon QuickSight.

<br>


## License Summary

This sample code is made available under a modified MIT license. See the LICENSE file.
