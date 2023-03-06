# Machine Learning for Time Series Prediction: Volume of Google Searches on "Entrepreneur"
## Project information
- **Author**: Ava Baker, Computation and Design (Computer Science), Class of 2025, Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Problem Set 2 for STATS201 Introduction to Machine Learning for Social Science, 2023 Spring Term (Seven Week - First) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: I would like to thank my professor, Luyao Zhang, for her patience and wisdom in guiding me through this assignment. I would also like to thank my classmate, Ace Asim, for giving me feedback on my poster and project.
- **Project Summary**: Financial crises tend to have effects on unexpected areas of life, and force people to find new ways to survive and earn money. Particularly, during the COVID-19 pandemic, certain industries were nearly destroyed while others found themselves thriving. New needs were created and old values tossed out as people’s priorities and abilities changed. In the stock market crash of 2008, however, nearly all industries took a hit and in high income countries around 14 million people lost their jobs, with half of that occurring in 2009 alone (United Nations 2011, 28). Furthermore, the quality of employment deteriorated worldwide (United Nations 2011, 27). During both of these times of uncertainty, a spike was observed in interest in entrepreneurship and new trends emerged within the industry. By applying causal inference to search data from Google Trends on the term “entrepreneur,” this study aims to identify the relationship between financial crises and interest in entrepreneurship.

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
![Random Forest Regression](https://user-images.githubusercontent.com/42778678/221403886-8c08dc39-887c-4555-b553-547605a8ae71.png)

**Figure No.1. Random Tree Regression**

*Figure No.1. Source: [Google Trends: Entrepreneur](https://trends.google.com/trends/explore?date=all&q=entrepreneur), created by [sklearn.ensemble.RandomForestRegressor](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html)*

![Abstract Wordcloud](https://user-images.githubusercontent.com/42778678/221403919-eca175e9-9ff3-4cbe-8816-680e640dd4e4.png)

**Figure No.2. Word Cloud of Related Literature Abstracts**

*Figure No.2. Source: [Related Literatures: Entrepreneurship Post Pandemic](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Ava/tree/main/data/Queried_Data/PS2references.csv), created by [wordcloud](https://pypi.org/project/wordcloud/)*

Figure No.1 is the Random Tree Regression of the google trend search data for "Entrepreneur." This is a supervised learning alogrithm that uses an ensemble learning method to determine the strength and character of the relationship between two variables. The second figure is a word cloud of frequently used terms in the abstracts of related literatures. As you can see, along with "entrepreneur" and "entrepreneurship," terms such as "crisis," "pandemic," and "covid" were also common, showing the relationship between the two.

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
