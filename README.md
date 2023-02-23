# Machine Learning for Time Series Prediction: Volume of Google Searches on "Entrepreneur"
## Project information
- **Author**: Ava Baker, Computation and Design (Computer Science), Class of 2025, Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Problem Set 2 for STATS201 Introduction to Machine Learning for Social Science, 2023 Spring Term (Seven Week - First) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: I would like to thank my professor, Luyao Zhang, for her patience and wisdom in guiding me through this assignment.
- **Project Summary**: Using machine learning methods to complete time series forecasting on google search trend data. Searches for the term "Entrepreneur" spiked twice since 2004, both after major economic disasters. This led me to be interested in analyzing interest in entrepreneurship and how this might spike during times of financial crisis.

## Part I: Machine Learning for Explanation
[Github Repository: stats201-PS2-Ava](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Ava)

## Part II: Machine Learning for Prediction

### Table of Contents
| Item  | Link |
| ------------- | ------------- |
| Data  | https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Ava/tree/main/data  |
| Code  | https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Ava/tree/main/code  |
| Spotlight  | https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Ava/tree/main/spotlight  |

### Data
| Type  | Link | Data Files | Data Content | Data Dictionary |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| Data Source  | https://trends.google.com/trends/explore?date=all&q=Entrepreneur  | https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Ava/tree/main/data/Queried_Data/interestOverTime.csv | A table including the score of searches for "Entrepreneur" and their corresponding Year/Month. | count: "Numbers represent search interest relative to the highest point on the chart for the given region and time. A value of 100 is the peak popularity for the term. A value of 50 means that the term is half as popular. A score of 0 means there was not enough data for this term" (from Google). Date: Year-Month.
| Queried Data  | https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Ava/tree/main/data/Queried_Data  | interestOverTime.csv, PS2references.csv | interestOverTime.csv is the Data Source (refer to above row) and PS2references contains the bibliographic information for 21 journal articles, books, and book chapters discussing recent trends in entrepreneurship and post-pandemic spikes in entrepreneurship. | For interestOverTime definitions refer to row above. Item type: A classification of the data source documented (either Journal Article, Book, or Book Chapter). Authors: Contributers to the data source. Title: Title of the journal article, book, or book chapter. Journal: The journal the data source was published in (if applicable). Publication Year: The year the data source was published in. Volume: The volume of the data source if applicable. Pages: The selecetion of pages that the data source comes from if applicable. Date Published: The year and month that the data source was published in. ISBN: THe ISBN number of the data source if applicable. URLs: Links to the data source if applicable. DOI: The DOI of the data source if applicable. Abstract: A summary of the data source.
| Processed Data  | https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Ava/tree/main/data/Processed_Data  | Regression_Train.csv, Regression_Test.csv, Classification_Train.csv, Classification_Test.csv | 

### Code
| Type  | Link |
| ------------- | ------------- |
| Process Data  | https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Ava/tree/main/code/Process_Data.ipynb  |
| Analyze Data  | https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Ava/tree/main/code/Analyze_Data.ipynb  |

### Spotlight
![Confusion Matrix](https://github.com/yutongquan/STATS201_Problem_Set_2/blob/main/Spotlight/Confusion%20Matrix_Ridge%20Classfier.png)

**Figure No.1. The Confusion Matrix for Ridge Classification**

*Figure No.1. Source: [Alpha Vantage: Digital & Crypto Currencies/DIGITAL_CURRENCY_DAILY](https://www.alphavantage.co/documentation/#digital-currency), created by [scikit-learn: Ridge regression and classification](https://scikit-learn.org/stable/modules/linear_model.html#ridge-regression-and-classification)*

Figure No.1 is the confusion matrix of [Ridge Classification](https://scikit-learn.org/stable/modules/linear_model.html#ridge-regression-and-classification) algorithm for Bitcoin ROI prediction. The confusion matrix provides an evaluation of the performance of the classification algorithm we use. In this matrix, the X-axis is the predicted label and the Y-axis is the true label,where 0 indicates a negative ROI and 1 indicates a positive ROI. As it approaches yellow, the number is larger, and as it approaches purple, the number is smaller. The figure shows that our model correctly classifies all 141 Positive ROI cases (True Positive), but misclassifies all 192 negative ROI cases (False Positive). The model accuracy is (TP + TN)/(TP + TN + FP + FN) = 141/333 = 0.42, the recall is TP/(TP + FN) = 141/141 = 1.00, and the precision is TP/(TP + FP) = 141/333 = 0.42 (Formula reference: [Krukrubo 2019](https://pub.towardsai.net/the-confusion-matrix-for-classification-eb3bcf3064c7)).

## References

### Data Source
[Google Trends: "Entrepreneur"](https://trends.google.com/trends/explore?date=all&q=Entrepreneur)
### Code Source
[stats201-tutorial-prediction/code](https://github.com/Rising-Stars-by-Sunshine/stats201-tutorial-prediction/tree/main/code)
### Articles
[Time Series Prediction Using LSTM Deep Neural Networks](https://www.altumintelligence.com/articles/a/Time-Series-Prediction-Using-LSTM-Deep-Neural-Networks)

[The Confusion Matrix for Classification](https://pub.towardsai.net/the-confusion-matrix-for-classification-eb3bcf3064c7)
### Literature
ADD LITERATURE HERE!
