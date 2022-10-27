# Aphelion Algorithmic Trading
### Johnathan Overton, Dylan Olsen, Khalid A. 


## Overview of the Analysis

* The purpose of this analysis was to build and optimize an algorithmic trading system so as to accurately predict, and take action upon, trading signals.
* The financial information used was based off of the data pulled from Alpaca API and has the following dimension:
  * date
  * open
  * high
  * low 
  * close
  * volume
  * trade_count
  * vwap

* In this model, the following technologies were incorporated:
  * Jupyterlab Notebook
  * Pandas
  * DateOffset
  * Plotly
  * ScikitLearn
  * Standard Scaler
  * Classification Report
  * Alpaca Trade API

* How to Use
  * Simply clone the repository and execute tesla-remodeled.ipynb
  * Note: To use for your own needs, create an Alpaca Trading account at https://alpaca.markets/

* Machine Learning process stages
  * Establish a Baseline Performance
  * Tune the Baseline Trading Algorithm
  * Evaluate a New Machine Learning Classifier
  * Create an Evaluation Report

## Results

### Baseline Classification

![1](https://github.com/Johove83/Aphelion_Algorithmic_Superiority/blob/main/images/baselineclassification.png)

This model determines a 50% accuracy at -1.0 and 52% at 1.0 signals. With a weighted average of 51% for both precision and recall.

### Training Window Decreased from six to five years.

![2](https://github.com/Johove83/Aphelion_Algorithmic_Superiority/blob/main/images/optimizedclassification.png)


Optimizing the training window to five years/sixty months offered a significant improvement to 100% and 53% for sell and buy signals, respectively.
Overall, this model offered a 75% weighted average in precision and a 53% weighted average in recall.

## Summary

Most interestingly, the fully tuned model offered superior accuracy at both signals. Despite this, both seemed to offer similar, if not identical, buy and sell signals through the testing period. 

A summary consideration determines that the optmized model offers far superior results than the baseline model. 

Below is a graph offered to show the predicted buy and sell signals vs the actual returns. As seen, the results are replicative of the predictions.

![3](https://github.com/Johove83/Aphelion_Algorithmic_Superiority/blob/main/images/optimizedgraph.png)