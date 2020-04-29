# Team-Quandary-Peak

## ABSTRACT
Coronavirus disease 2019 (COVID-19) is an infectious disease caused by severe acute respiratory syndrome coronavirus 2 (SARS-CoV-2).The disease was first identified in December 2019 in Wuhan, the capital of China's Hubei province, and has since spread globally, resulting in the ongoing 2019–20 coronavirus pandemic. Common symptoms include fever, cough and shortness of breath. Other symptoms may include fatigue, muscle pain, diarrhoea, sore throat, loss of smell and abdominal pain. The time from exposure to onset of symptoms is typically around five days, but may range from two to fourteen days. While the majority of cases result in mild symptoms, some progress to viral pneumonia and multi-organ failure. As of April 12, 2020, more than 1.8 million cases of COVID-19 have been reported in 210 countries and territories, resulting in more than 112,000 deaths. More than 415,000 people have recovered, although there may be a possibility of reinfection. Specifically, in the US, more than 549,000 cases have been reported, more than 32,000 people have recovered, while still resulting in more than 21,000 deaths. In Colorado, 6,893 cases have been reported and 274 deaths have happened. 
To better understand COVID-19 spreading in the past and the future in the United States, the project compared the outbreak among serious regions and the overall situation in the United States. We integrated both statistical aspect (predicting models) and texting mining technique.<br>
![Image](https://github.com/MSBX5420/Team-Quandary-Peak/blob/master/Docs/Purpose.png)

## Datasets
- Tableau COVID-19 Data Hub (https://www.tableau.com/about/blog/2020/3/coronavirus-data-hub-faq) [(link to Data)](https://github.com/MSBX5420/Team-Quandary-Peak/tree/master/Data)<br>
The data comes from the dataset maintained and updated by the Johns Hopkins University Center for Systems Science and Engineering. Tableau cleans, reshapes, and makes this data ready for your analysis. This dataset updated by 9:00am EST every day. This data contains Dates and Confirmed Cases and total deaths for each state by providing for all countries over the word. This data also contains the location (Lat and Long).

- COVID-19 in USA (https://www.kaggle.com/sudalairajkumar/covid19-in-usa#us_covid19_daily.csv) [(link to Data)](https://github.com/MSBX5420/Team-Quandary-Peak/tree/master/Data)<br>
This dataset has details information from 50 US states and the District of Columbia at daily level. This dataset contains date, total case of states, number of positive and negative cases, pending cases, number of recovered and death, and number of death increasing by daily. 

- COVID-19 Open Research Dataset Challenge (CORD-19)( https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge) [(link to Data)](https://github.com/MSBX5420/Team-Quandary-Peak/tree/master/Data)<br>
In response to the COVID-19 pandemic, the White House and a coalition of leading research groups have prepared the COVID-19 Open Research Dataset (CORD-19). CORD-19 is a resource of over 51,000 scholarly articles, including over 40,000 with full text, about COVID-19, SARS-CoV-2, and related coronaviruses. This freely available dataset is provided to the global research community to apply recent advances in natural language processing and other AI techniques to generate new insights in support of the ongoing fight against this infectious disease.

## Tools
### AWS	<br>
Amazon Web Services (AWS) is a subsidiary of Amazon that provides on-demand cloud computing platforms and APIs to individuals, companies, and governments, on a metered pay-as-you-go basis. In aggregate, these cloud computing web services provide a set of primitive abstract technical infrastructure and distributed computing building blocks and tools. We used Leeds EMR to save our coding files and data. We also uploaded our data from local to EMR cluster, then transformed the data to S3 Bucket. We can input data directly from S3 bucket to Jupyter File. Then we used Leeds Prod Cluster Jupyter Notebook to create Jupyter Notebook for coding and reviewing.
### Spark<br>
Apache Spark is an open-source distributed general-purpose cluster-computing framework. We used Pyspark for data cleaning and Word Cloud. The reason we used spark was because when we were working on a dataframe, we only needed to write codes for one row in spark, and then spark would assign slaves to work on each row of the dataframe instead of writing a for loop. This method optimizes a step-by-step process to a parallel process and will save a lot of time when we run the codes.
### Binder [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MSBX5420/Team-Quandary-Peak/master)<br>
The Binder Project is a software project to package and share interactive, reproducible environments. We used Binder to link our Github Project repo to review our teammates’ codes.
### Github<br>
We used Github for merging all parts and displaying our project.

## Development
![Image](https://github.com/MSBX5420/Team-Quandary-Peak/blob/master/Docs/Process.png)
Uploading the datasets from local to EMR Cluster, then transform to Amazon S3 Bucket , then use EMR jupyter notebook cluster to link the data.

## Code Reviewing
### Text Mining
- [Topic Model](https://github.com/MSBX5420/Team-Quandary-Peak/tree/master/Text%20Mining/Topic%20Modeling)
    - We used “tmtoolkit” and “nltk” packages to build our model. Moreover, we combined all text into one dictionary and set up the “stopwords”, “punkt”, “averaged_perceptron_tagger”, and “wordnet” for directory.  Additionally, we put the texts into document term matrix. Finally, we used “LDA TOPIC MODL” to extract top 16 models over all texts.
- [Word Cloud](https://github.com/MSBX5420/Team-Quandary-Peak/tree/master/Text%20Mining/Word%20Count)
    - We generated a word cloud for all news in the dataset and several GIFs for daily news word cloud.<br>
 ![Image](https://github.com/MSBX5420/Team-Quandary-Peak/blob/master/Text%20Mining/Word%20Count/freq_word_plot_1.gif)
### [Visualization](https://github.com/MSBX5420/Team-Quandary-Peak/tree/master/Data%20Visualization)
    - We used Data Visualization to analyze the current situitations of U.S.<br>
  ![Image](https://github.com/MSBX5420/Team-Quandary-Peak/blob/master/Data%20Visualization/Plots/Apr-27-2020%2014-29-20.gif)
### Predictive Modeling 
- [Time Series](https://github.com/MSBX5420/Team-Quandary-Peak/tree/master/Time%20Series)
    - We use time series to better understand COVID 19 spreading trends in the past (before 4/10/2020) and future (after 4/10/2020).
- [Random Forest](https://github.com/MSBX5420/Team-Quandary-Peak/tree/master/Random%20Forest)
    - We used Random Forest to the variables which has the most effects of COVID-19. 


## Conclusion and Suggestion<br>
In the first-10-day news (January 8, 2020 to January 19, 2020), the high frequent words were Wuhan, China, Chinese, SARS, and etc. People were focusing on the origin of coronavirus and analyzing the virus explosion in specific areas. However, the last-10-day news (March 16, 2020 to March 27, 2020), the high frequent words became COVID, people, time, new, and etc. The difference means that people’s attention has been transferred from specific areas, such as China or South Korea, to the whole world, because people realized that covid-19 became a global pandemic now. Both governments have done effective actions and people have concerned about the pandemic to slow down globally spreading
Both Confirmed and Death trend keeps increasing and “Economic”, “Education Level”, “Health” issues are more important than population density. We suggest government should take actions based on those low education level states or those states with high risks of potential mental illness. 
The United States is in dangerous situation. The East Coast is worse than the West Coast. Although CO is below the average, we still have to be careful. Government has done effective actions and people have concerned about the pandemic.
AWS cluster increases the productivity and has fast innovation, also increases the resource availability and strategic resource usage, really good for team works.We would like to make streaming data to generate covid-19 data in the future to optimize our project.

## Team Members:
- Candice Chuang(https://github.com/Candice-Chuang)
- Qingdi Xiao (https://github.com/Carina-Xiao)
- Wen Huang (https://github.com/HiwenH)
- Wenbin Yang (https://github.com/Wenbin-Yang)
- Yuxiang Wang (https://github.com/yuwa4103)

