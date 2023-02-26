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

#### Meta-Data
| Type  | Link | Data Files | Data Content |
| ---- | ---- | ---- | ----- |
| Data Source  | https://trends.google.com/trends/explore?date=all&q=Entrepreneur  | https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Ava/tree/main/data/Queried_Data/interestOverTime.csv | A table including the score of searches for "Entrepreneur" and their corresponding Year/Month. |
| Queried Data  | https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Ava/tree/main/data/Queried_Data  | interestOverTime.csv, PS2references.csv | interestOverTime.csv is the Data Source (refer to above row) and PS2references contains the bibliographic information for 21 journal articles, books, and book chapters discussing recent trends in entrepreneurship and post-pandemic spikes in entrepreneurship. |
| Processed Data  | https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Ava/tree/main/data/Processed_Data  | Regression_Train.csv, Regression_Test.csv, Classification_Train.csv, Classification_Test.csv | 

#### Data Dictionary
| Term  | Definition |
| ------------- | ------------- |
| count | "Numbers represent search interest relative to the highest point on the chart for the given region and time. A value of 100 is the peak popularity for the term. A value of 50 means that the term is half as popular. A score of 0 means there was not enough data for this term" (from Google).  |
| Date | Year-Month.  |
| Item type  | A classification of the data source documented (either Journal Article, Book, or Book Chapter).  |
| Authors  | Contributers to the data source.  |
| Title  | Title of the journal article, book, or book chapter.  |
| Journal  | The journal the data source was published in (if applicable).  |
| Publication Year  | The year the data source was published in.  |
| Volume  | The volume of the data source if applicable.  |
| Pages  | The selecetion of pages that the data source comes from if applicable.  |
| Date Published  | The year and month that the data source was published in.  |
| ISBN  | The ISBN number of the data source if applicable.  |
| URLs  | Links to the data source if applicable.  |
| DOI  | The DOI of the data source if applicable.  |
| Abstract  | A summary of the data source.  |

### Code
| Type  | Link |
| ------------- | ------------- |
| Query Data  | https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Ava/tree/main/code/Query_Data.ipynb  |
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

### Literature

Cardow, Andrew. "The Metaphorical Rise of Entrepreneurship".SSRN Electronic Journal (2010).

Hill, Stephen, Aileen, Ionescu-Somers, Alicia, Coduras, Maribel, Guerrero, Ehud, Menipaz, Fatima, Boutaleb, Przemysław, Zbierowski, Thomas, Schøtt, Sreevas, Sahasranamam, Jeffrey, Shay, and Global, Monitor. Global Entrepreneurship Monitor 2022/2023 Global Report: Adapting to a “New Normal”. 2023.

Elam, Amanda, Karen, Hughes, Maribel, Guerrero, Stephen, Hill, Catharina B, Nawangpalupi, M.Mar, Fuentes-Fuentes, Juan, González, Ana, Fernandez-Laviada, Catalina, Martínez, Alicia, Rubio Bañón, Nihel, Chabrak, Candida, Brush, Ben, Baumer, René, Heavlow, and the, (GERA). Women’s Entrepreneurship 2020/21. Thriving Through Crisis. 2021.

Bosma, Niels, Stephen, Hill, Aileen, Ionescu-Somers, Donna, Kelley, Maribel, Guerrero, Thomas, Schøtt, and the, (GERA). Global Entrepreneurship Monitor. 2020/2021 Global Report. 2021.

Behr, Rachael, and Virgil, Storr. "Understanding pandemic entrepreneurship as a unique form of crisis entrepreneurship".Journal of Entrepreneurship and Public Policy 11 (2022).

Sreenivasan, Aswathy, and Ma, Suresh. "Twenty years of entrepreneurship education: a bibliometric analysis".Entrepreneurship Education (2023): 1-24.

Elam, Amanda, Karen, Hughes, Maribel, Guerrero, Stephen, Hill, Catharina B, Nawangpalupi, M.Mar, Fuentes-Fuentes, Juan, González, Ana, Fernandez-Laviada, Catalina, Martínez, Alicia, Rubio Bañón, Nihel, Chabrak, Candida, Brush, Ben, Baumer, René, Heavlow, and the, (GERA). Women’s Entrepreneurship 2020/21. Thriving Through Crisis. 2021.

Verma, Amit. Entrepreneurship Amidst Pandemic COVID 19. 2022.

Monitor, Global, Amanda, Elam, Benjamin, Baumer, Thomas, Schøtt, Mahsa, Samsami, A., Dwivedi, Baldegger, Rico, Maribel, Guerrero, Fatima, Boutaleb, and Karen, Hughes. GEM 2021/22 Women’s Entrepreneurship Report: From Crisis to Opportunity. 2022.

Yerzhanova, A.M., and L.Zh, Ashirbekova. "THE ROLE OF SOCIAL ENTREPRENEURSHIP IN A PANDEMIC".Statistika, učet i audit 87 (2022): 37-48.

Pereira, Ygo, Priscilla, Sousa, Adams, Alves, Elis, Regina, and Washington, Monte. "Perception of entrepreneurship as alternative to facing the post-pandemic crisis".Revista de Gestão e Secretariado 14 (2023): 893-902.

Petersen, R., L., William, S., Shatner, and A., Ogleby. "Scalable Green Entrepreneurship in the Post- COVID-19 Pandemic World: The Australasian Case".Asian Journal of Economics, Business and Accounting (2021): 14-23.

Liñán, Francisco, and Inmaculada, Jaén. "The Covid-19 pandemic and entrepreneurship: some reflections".International Journal of Emerging Markets 17 (2022): 1165-1174.

Maldonado Castro, Jenny, Angel, Castro, Daniel, Gavilánez, and María, Guzmán Macías. "Post Pandemic Entrepreneurship Surge: Impact on Economic Growth".Centro Sur 6 (2022).

Tripalupi, Ramadhani, and Prameshwara, Anggahegari. "Strengthening Entrepreneurship: Sharia Empowerment for MSMEs Amidst the Covid-19 Pandemic".International Journal of Entrepreneurship and Sustainability Studies 2 (2022): 73-89.

Bapat, Gautam, Ravikumar, Chitnis, and Srinivas, Pasumarti. "The state of "Innovation" and "Entrepreneurship" in India -A Post Pandemic Bibliometric Analysis". (2022): 6820-6826.

Kang, Pengsheng, Lin, Guo, Zhou, Lu, and Lili, Zhu. "Evaluation of the early-stage entrepreneurship activity in the United States during the COVID-19 pandemic".Frontiers in Public Health 10 (2022).
