# Analysis of the Bank Marketing Data Set

We are working with a dataset from a Portuguese bank.  The data categorizes direct marketing efforts (phone calls) designed to sell term deposit products.  The [dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing) was donated to UCI's Machine Learning Repository. The goal is to predict which contacts are most likely to subscribe to a term deposit. Data range from May 2008 to November 2010

## Analysis

- Break data into training and test sets

- Build a few two-stage logistical regression model: propensity to answer, followed by likliehood to purchase a term loan given that the person answers.

- Build a random forest model and a tuned random forest model (using downsampling to optimize for an unbalanced sample)

## Dashboard

This is a simple decision tool that allows you to decide whether to use the tuned RF model to screen potential marketing candidates or just target the whole population based on demographics and the cost/benefit of making calls vs. capturing sales.  This is instrumented very simply right now - we use the test population and re-sample from it to try to capture true relationships between variables.  Given the relatively short time-frame, if relationships between variables changed in ways that were not captured in this dataset, the predictive ability of the model and the utility of the decision-making tool would of course be de-graded.

## LearnR

We can add to this / adapt as required.  Right now it's a simple "Intro to Tidyverse" demo that uses the bank marketing data.

