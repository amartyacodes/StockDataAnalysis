# StockDataAnalysis
Code for Breakout prediction using ML Methods

## Extraction of Data
The data was extracted using Yahoo Finance API for the MRF stock from the year of 01/01/2000- 20/05/2018. The MRF stock data was chosen because it had quite a frequent breakouts during the time. 

## Methodology of Labelling

The data points were considered as a possible candidate of breakout using the following logic.
At first, we check if consolidation occured. Meaning, if the stock traded maintaining a very narrow range in the last 15 days. If min close value from last 15 days is greater than 98% of the max close from last 15 days, we can say consolidation occured. If consolidation occured, then, if the close price is greater than max close from last 15 days or close price is less than min close from last 15 days, we identify the stock as breakout candidate. 

## ML Techniques Used

The ML techniques that were used are KNN, Decision Tree, Random Forest Classifier, SGD Classifier, Adaboost Classifier, SVM and Multi layer Perceptron and the results were noted.

The following paper was implemented: https://enpesj.enp.edu.dz/index.php/enpesj/article/view/173
