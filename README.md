# Predicting Passenger Satisfaction

## Framing the Problem

### Business Objective

We want to build a model that predicts passenger satisfaction to analyze what factors affect the flying experience. From uncovering those factors for different customer groups, we can optimize on them to create a better passenger experience and in turn improve retention of product, increase customer loyalty and drive up revenue.

### The Model

We will be using 2 types of models: Logistic Regression and Support Vector Machines. Both of these models are easy to implement and interpretable.

Since logistic regression assumes a linear relationship between the explanatory and response variables while SVM can assume a non-linear relationship, we can compare these 2 models to see which one fits the data better.

### Performance Assessment

We will be using the F1-score and the precision-recall (PR) curve to assess and compare our models.

We want to minimize the number of passengers that we misclassify as being satisfied (when they're actually dissatisfied) so that we can pinpoint what are areas of dissatisfaction). However, we also want to minimize the number of passengers we misclassify as not being satisfied (when they're actually satisfied) so that we can find factors that are contributing to a satisfied passenger.

A precision-recall curve is to support our F1 score and also because we should care more about misclassifying a disatissfied passenger, from a customer experience perspective.

### Assumptions

We're assuming that each entry of the dataset are independent from each other and that one passenger's satisfaction doesn't affect another passenger's. We're also assuming that each entry of the data is coming from the same distribution.