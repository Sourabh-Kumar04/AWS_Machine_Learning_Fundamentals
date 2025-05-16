# Exercise 3: ML Lifecycle Case Study

[App8 Case Study](https://aws.amazon.com/solutions/case-studies/app-8/)

Written response, select 3 of the 11 steps and write a short paragraph explaining how you would go about executing on these parts of the ML Lifecycle.

Exact solutions will vary but should be somewhat related to the answers below.

## Problem
The problem with restaurants and food-related businesses is not knowing future demand for your services. Because this is an unknown, you may create or purchase too much or too little of an item. Furthermore, there are also operational costs associated with not knowing demand as it may require additional personal and equipment. This leads to a mismatch in demand between the business and the customer, leading to a poor experience.

## Business Objective
Predict demand based on the restaurant's risk tolerance, and create "what if" scenarios to better prepare the business. This creates new tools for the restaurants to better serve their customer and overall create an improved experience.

## Obtain Data
App8 is a service that connects customers and restaurants. In doing so, and based on customer payment information, they can see how items from a business are purchased, returned, or denied. With enough businesses in aggregate, they can start finding trends based on customer behavior, business details, and time patterns.

## Process Data
As with any data, cleaning, and formatting, the data will be crucial. Not only will transactions be denied and data not being be captured within App8, but also every business is different leading to non-uniformity. Standardization and data pipelines will need to be in place to address all differences in the data.

## Analyze Data
After the data is processed, it can be loaded into an analytics system such as Pandas. From there, it can be visualized, described, and modified in order to make it robust and ready for model building.

## Build Model
Building a model will require time series analysis and prediction using the AWS Forecast Solution. It will create several quantiles: p10, p50, and p90. These are configurable depending on the business's risk tolerance. The model should be generalizable across all categories.

## Test Model
Testing of the model requires historical data on many businesses of all categories. Once the model is built, it should be back-tested and optimized to reduce the error while not over-fitting.

## Deploy Model
Deploying of the model is cloud-first, using AWS Solutions that are ready to train and deploy to production. Because these are managed through AWS and their partners, much of the overhead in managing deployments is out of our hands.

## Inference
The model uses AWS solutions, but all inferences should be tracked and logged. Inference data provides new insights into the accuracy of the forecasts and leads to building more robust models in the future. Also, having a model that is not only accurate but responsive, leads to a better user experience and overall improved satisfaction.

## Evaluate Model
After inference, evaluating how the model performed is just as important as producing the model initially. Evaluation can provide future iterations of the model and improved accuracy

## New Data
As new data enters the system that has been influenced by predictions, that will feed into the models to enhance their forecasts. Not only that, but it will also validate the current predictions in the real-world setting.