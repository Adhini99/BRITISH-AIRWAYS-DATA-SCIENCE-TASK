# BRITISH-AIRWAYS-DATA-SCIENCE-TASK
British Airways Data Science Job Simulation on Forage - August 2024   
* * Completed a simulation focussing on how data science is a critical component of British Airways success
* * Scraped and analysed customer review data to uncover findings
* * Built a predictive model to understand factors that influence buying   behaviour

# SENTIMENTAL ANALYIS

website link from which data was extracted: [https://www.airlinequality.com/airline-reviews/british-airways].

Jupyter Notebook and Google Colab was used for this project.

Dataset was extracted from the skytrax and sentiment analysis was performed by following steps:

1.Web scraping : -> Packages used: BeautifulSoup ,Pandas and requests -> Data was extracted from the website and converted into a dataframe from list using pandas and stored in a file in csv format -> 1000 reviews were scrapped as a sampling procees and stored into 10 pages (100 reviews in each page)

2.Data preprocessing : -> Packages used: re,Pandas -> Text preprocessing and data manipulation was performed by removing unwanted words, Additionaly data cleaning can also be done ny removing stopwords(But was not done now but done when data visualized)

3.Analysis : -> Packages used: nltk,requests and pandas -> 'vader_lexicon' was downloaded for using SentimentIntensityAnalyzer and sentiment score was generated ~ if score > 0 => positive review ~ elseif score < 0 => negative review ~ else => neutral review

4.Data visualization : -> Packages used: Matplotlib and WordCloud -> A pie chart is plotted representing the Sentiment Analysis -> A barchart is plotted representing keywords count used in the reviews -> A Wordcloud is displayed after removing stopwords from the dataset

# CUSTOMER BEHAVIOUR PREDICTION

For predicting customer buying behaviour on British Airways, predictive modeling and exploratory data analysis was performed.

Packages used: pandas,sklearn (scikit-learn), matplotlib and numpy

Algorithm used: Random Forest Classificaton (XBG Classifier is another alternative)

To provide more context, below is a more detailed data description, explaining exactly what each column means:

num_passengers = number of passengers travelling

sales_channel = sales channel booking was made on

trip_type = trip Type (Round Trip, One Way, Circle Trip)

purchase_lead = number of days between travel date and booking date

length_of_stay = number of days spent at destination

flight_hour = hour of flight departure

flight_day = day of week of flight departure

route = origin -> destination flight route

booking_origin = country from where booking was made

wants_extra_baggage = if the customer wanted extra baggage in the booking

wants_preferred_seat = if the customer wanted a preferred seat in the booking

wants_in_flight_meals = if the customer wanted in-flight meals in the booking

flight_duration = total duration of flight (in hours)

booking_complete = flag indicating if the customer completed the booking

Procedure:

1.Dataset is imported

2.Unique attribute is days ,so they are mapped

3.Statistical and arithmetic methods are performed for all attributes with respect to instances

4.All the attributes data types are converted into int64 (few were objects earlier)

5.Mutual Information scores are generated

6.Bar graph is plotted with mi scores

7.Train Test Split is done

8.Random forest is implemented

9.Accuracy and AUC score is generated

RESULT:

ACCURACY:  84.84

AUC score:  0.5527766076821664
