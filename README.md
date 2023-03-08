# Machine Learning for Time Series Prediction: Volume of Google Searches on "Entrepreneur"
## Project information
- **Author**: Ava Baker, Computation and Design (Computer Science), Class of 2025, Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Problem Set 2 for [STATS201 Introduction to Machine Learning for Social Science, 2023 Spring Term (Seven Week - First)](https://ms.pubpub.org/) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: I would like to thank my professor, Luyao Zhang, for her patience and wisdom in guiding me through this assignment. I would also like to thank my classmate, Ace Asim, for giving me feedback on my poster and project.
- **Project Summary**: Financial crises tend to have effects on unexpected areas of life, and force people to find new ways to survive and earn money. Particularly, during the COVID-19 pandemic, certain industries were nearly destroyed while others found themselves thriving. New needs were created and old values tossed out as people’s priorities and abilities changed. In the stock market crash of 2008, however, nearly all industries took a hit and in high income countries around 14 million people lost their jobs, with half of that occurring in 2009 alone (United Nations 2011, 28). Furthermore, the quality of employment deteriorated worldwide (United Nations 2011, 27). During both of these times of uncertainty, a spike was observed in interest in entrepreneurship and new trends emerged within the industry. By applying causal inference to search data from Google Trends on the term “entrepreneur,” this study has identified a relationship between financial crises and interest in entrepreneurship. By understanding the link between financial crisis and entrepreneurship, preperations can be better made to mitigate the economic after affects of financial disasters.

### Table of Contents

| Item  | Link |
| ------------- | ------------- |
| Data  | https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/tree/main/data  |
| Code  | https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/tree/main/code  |
| Spotlight  | https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/tree/main/spotlight  |
| More About the Author  |   |
| References  |   |

### Data

#### Meta-Data

| Type  | Link | Data Files | Data Content |
| ---- | ---- | ---- | ----- |
| Data Source  | https://trends.google.com/trends/explore?date=all&q=Entrepreneur  | https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/tree/main/data/Queried_Data/interestOverTime.csv | A table including the score of searches for "Entrepreneur" and their corresponding Year/Month. |
| Queried Data  | https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/tree/main/data/Queried_Data  | interestOverTime.csv, interestOverTime_March2023.csv, references.csv | interestOverTime.csv is the Data Source (refer to above row) and interestOverTime_March2023.csv is the same file with an additional row for March 2023. references.csv contains the bibliographic information for 21 journal articles, books, and book chapters discussing recent trends in entrepreneurship and post-pandemic spikes in entrepreneurship. |
| Processed Data  | https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/tree/main/data/Processed_Data  | Regression_Train.csv, Regression_Test.csv, Classification_Train.csv, Classification_Test.csv | 

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
| Query Data  | https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/tree/main/code/Query_Data.ipynb  |
| Process Data  | https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/tree/main/code/Process_Data.ipynb  |
| Analyze Data  | https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/tree/main/code/Analyze_Data.ipynb  |
| Machine Learning for Explanation  | https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/tree/main/code/MachineLearningforExplanation.ipynb  |
| Causal Inference  | https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/tree/main/code/causal_inference.ipynb  |

### Spotlight

**Figure No.1 Project Poster**

<img src="https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/blob/363afe427bd01c754e2056549239a11cde4116d2/spotlight/figures/poster.jpg>

*Figure No.1 created by [Google Slides](https://docs.google.com/presentation/u/0/)*

This project poster describes the different facets of the study step by step and discusses the results and of the study. It presents several figures related to the study and provides a brief and concise description of what the study is on. It elaborates on the background and the intellectual merits of the study and discusses the methodology in depth.

**Figure No.2 Word Cloud of Related Literature Abstracts**

<img src="https://user-images.githubusercontent.com/42778678/221403919-eca175e9-9ff3-4cbe-8816-680e640dd4e4.png" width="800">

*Figure No.2 Source: [Related Literatures: Entrepreneurship Post Pandemic](https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/tree/main/data/Queried_Data/references.csv), created by [wordcloud](https://pypi.org/project/wordcloud/)*

The second figure is a word cloud of frequently used terms in the abstracts of related literatures. As you can see, along with "entrepreneur" and "entrepreneurship," terms such as "crisis," "pandemic," and "covid" were also common, showing the relationship between the two.

**Figure No.3 Random Tree Regression**

<img src="https://user-images.githubusercontent.com/42778678/221403886-8c08dc39-887c-4555-b553-547605a8ae71.png">

*Figure No.3 Source: [Google Trends: Entrepreneur](https://trends.google.com/trends/explore?date=all&q=entrepreneur), created by [sklearn.ensemble.RandomForestRegressor](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html)*

Figure No.3 is the Random Tree Regression of the google trend search data for "Entrepreneur." This is a supervised learning alogrithm that uses an ensemble learning method to determine the strength and character of the relationship between two variables. The green is the actual data whereas the blue is the predicted data, meaning that the search volume for "Entrepreneur" is expected to shrink quite a bit.

**Figure No.4 Causal Inference**

<img src="https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/blob/ec4747b9848cf6b8278b7d83388fde642f235c5d/spotlight/figures/prediction_figure.png" width="500">

*Figure No.4 created by [Whimsical](https://whimsical.com/)*

It is predicted that the causal inference algorithm will reveal a disparity in the search volume for "entrepreneur" before and after financial crises, mainly the 2008 stock market crash and the COVID-19 pandemic. This study's hypothesized that although there will be a disparity before and after both the 2008 stock market crash and the COVID-19 pandemic, the latter will be significantly greater. Furthemore, it was thought that despite these disparities, all linear regressions would have positive slopes.


**Figure No.5 Annual % of World GDP Growth**

<img src="https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/blob/0bb218ade90eb6291957504fa1c51bd853e58c00/spotlight/figures/gdp_growth.png" width='450' height='300'>

*Figure No.5 Source: [The World Bank](https://data.worldbank.org/indicator/NY.GDP.MKTP.KD.ZG?end=2021&start=2004)*

Here the annual world GDP is displayed from 2004 to 2021. Two large dips can be observed in 2009 and 2020, respectively. These correlate to the 2008 stock market crash and the COVID-19 pandemic. Due to the pandemic, a recession was declared in most countries in February 2020 which would explain the second dip. The stock market crash occured late in the year of 2008, which caused 2009 to be so low.


**Figure No.6 Monthly Google Search Volume for "Entrepreneur"**

<img src="https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/blob/0bb218ade90eb6291957504fa1c51bd853e58c00/spotlight/figures/search_trend.png">

*Figure No.6 Source: [Google Trends](https://trends.google.com/trends/explore?date=all&q=entrepreneur)*

Here, the google search volume for the term "Entrepreneur" can be observed from 2004 to early 2023. In December 2008, an upward trend begins which only seems to steady itself in December of 2010. Contrarily, in late 2021 a massive spike occurs only to result in a spiky downward trend. These events line up, with slight delay, with the 2008 stock market crash and the start of the 2020 recession, which was a by product of the COVID-19 pandemic.


**Figure No.7 Linear Regression of Data**

<img src="https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/blob/77da9e0c365f502d983b3e5666bd050d2a381938/spotlight/figures/causal_inference.png" width='500'>

*Figure No.7 created with [Google Colab](https://colab.research.google.com/) and [numpy.polyfit](https://numpy.org/doc/stable/reference/generated/numpy.polyfit.html)*

In this graph a linear regression line has been fitted to the google search volume of "Entrepreneur' before the 2008 stock market crash, after, and after the declaration fo the 2020 global recession. Before the 2008 crash, the linear regression shows a downward trend in searches for "Entrepreneur" but a huge jump in searches occurs once the crash occurs. After 2008, the search volume plateaus but is still significantly greater than before the crash. There is little difference in search volume immediately after the world recession is declared in February of 2020 but the following months show an upward trend as a huge spike occurs in October of 2021. Contrarily to the hypothesis, there is little-to-none disparity in search volume immediately after February 2020, but rather a dramatic change in slope. Conversely, there is a large jump in search volume before and after the 2008 stock market crash, and the linear regression lines' slopes also changed from negative to a plataeu.

**Figure No.8 AI Ethics**

<img src="https://github.com/Rising-Stars-by-Sunshine/stats201-final-Ava/blob/00b9f0510bb0ee7eaabecfcae801ac3abceeade8/spotlight/figures/ai_ethics.jpg">

*Figure No.8 created with [Google Slides](https://www.google.com/slides/about/)*

This poster showcases some of the leading issues with AI and also summarizes the relevant issues to this study. Many of the issues brought up on the poster were discussed in class, such as the issue of flippant use of AI, especially by students or novices to the industry, as well as misapropiation of results generated by AI. It is pivotal that researchers and developers keep in mind the ethical pitfalls of AI while using it, and that moving forward greater awareness about AI ethics is prioritized and protective cautions taken.

## More About the Author

<img src="https://user-images.githubusercontent.com/42778678/215335060-e59274ff-82d3-4a29-8a04-ffc320dcf81b.png" width="300">

  Ava Baker is a Computation and Design major with an emphasis on Computer Science at Duke Kunshan University. She will graduate with the class of 2025 and is currently traveling Europe while attending her studies online, although she completed her first year at Duke University and attended a semester abroad in Barcelona, Spain in the fall semester of her sophomore year. Ava was born in raised in the Bay Area, California and has been set on majoring in computer science since childhood. She spent the summer before college assisting in the creation of a a non-profit organization where she distrubuted free portable chargers and cell phones to the homeless, provided them with tech help, and assisted in setting up a free weekly computer lab. Ava has also worked several jobs including camp counselor, boba-barista, Chief Operator at a startup that provided labor for concession booths, and most recently as a summer intern in the Technology Services and Solutions department of Santa Clara County (Califonria). Ava is highly interested in software engineering and design, and is still exploring various relevant fields. Her greatest and most recent programming experience lies with Java, but she also has worked with HTML, Python, and C#. She has also taken coursework on the subjects of AI, machine learning, and quantum computing.
  
  
  In this course I have seen firsthand how machine learning can help tackle previously mis or mal-understood issues. By applying various algorithms to economic, societal, or other problems, we can use data to better understand the problem at hand, both by revealing its root and sometimes even potential solutions. Having the knowledge to do interdisciplinary work allows the researcher to not only have the skills to do such work but also the background knowledge in the subect that the research question you're posing lies in, to then diagnose and analyze the data you've processed. This can help you to move forward confidently and with solid evidence of what a promising solution might be. Learning some of these skills has not only piqued my interest in machine learning but also opened my eyes to how machine learning could be used to solve so many of the world's problemes, which I one day hope to participate in finding solutions to. Particularly, I'm really interested in education and would love to help make computer science courses accessible to people of all ages and demographics.

## References

### Data Source
[Google Trends: "Entrepreneur"](https://trends.google.com/trends/explore?date=all&q=Entrepreneur)

### Code Source
[stats201-tutorial-prediction/code](https://github.com/Rising-Stars-by-Sunshine/stats201-tutorial-prediction/tree/main/code)

Pandey, Shekhar. “NumPy Polyfit.” Linuxhint, 2021, linuxhint.com/numpy-polyfit/. Accessed 8 Mar. 2023.

### Articles

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

### Literature

“Regression Discontinuity | BetterEvaluation.” n.d. Www.betterevaluation.org. Accessed February 26, 2023. https://www.betterevaluation.org/methods-approaches/methods/regression-discontinuity.

“The Great Recession and the Jobs Crisis.” 2011. https://www.un.org/esa/socdev/rwss/docs/2011/chapter2.pdf.

United Nations. 2011. “The Global Social Crisis.” New York: United Nations. https://www.un.org/esa/socdev/rwss/docs/2011/rwss2011.pdf.

World Bank national accounts data, and OECD National Accounts data files.
