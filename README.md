# Predicting Airbnb Bookings in NYC
![image](https://user-images.githubusercontent.com/40476299/137991634-e0f96471-4ac0-4cc6-9bcd-f867b96701d2.png)

# Business  Understanding
Airbnb is an online marketplace for vacation rentals, cabins, houses, boats and more. Airbnb has round 150 million users and has listings all over the world. What is great about airbnb is that anyone can create there own listing anywhere from renting out a single bedroom to a home.

The purpose of this project is to create a model that is able to predict the probability of an Airbnb Host listing to be booked or not based on the features the listing has. This would be helpful for Airbnb Host who might want to know if the listing has a good chance of being booked based on what the listing has to offer.
can be useful for an airbnb host who would like to know if there listing has a chance of being booked or not.

# Data
This data comes from the Inside Airbnb website, which is an open source tool for airbnb listings all over the world. I will be focusing on the dataset for NYC. In this dataset it contains around 36,923 rows (listings) and 74 columns (features). I also got information from kaggle that has a lists of different attractions in NYC, Manhattan based. Links to the data below.

* http://insideairbnb.com/new-york-city/

* https://www.kaggle.com/new-york-city/nyc-cultural-institutions-by-block-and-lot?select=cultural-institutions-by-block-and-lot.csv

#### Metric
For my target I will be looking at the 'has_availability' column to see if the a listing is available to be booked or not. For this project my target is binary so I will be working with classifiaction models. For my metric I will be looking at accuracy and precision. For accuracy I will be looing how accurate my models are preforming and for precision I will be looking how well my model is correctly predicting if my listing has availability to be booked or not. 

# Exploritory Data Analysis

* A boxplot of the number of amentities for a listing based on if the listing is available to be booked or no. Looking at this graph it is showing listing with no availiability had generally less amenities than those that did have availiability. So for an airbnb host, having a lot of amenities does not necessarily mean more bookings.

![image](https://user-images.githubusercontent.com/40476299/139118325-b1907b0e-27dc-4767-9cd4-6de69782f317.png)

 * Below the graph shows the number of reviews based on availiablity. You would think having more reviews would increase the chance of the listing to be booked but with this graph it is showing the opposite.


![image](https://user-images.githubusercontent.com/40476299/139117944-2cc5f0c1-2a00-4dcc-9a1c-622c92bd1628.png)


* Average price of listing in NYC

<img width="702" alt="Screen Shot 2021-10-26 at 5 40 27 PM" src="https://user-images.githubusercontent.com/40476299/138965057-0bc01195-e720-4abf-ae64-2de2930c9ba9.png">


* Created a map of different attractions in Manhattan and calculated the distance from each listing from each attraction.

<img width="778" alt="Screen Shot 2021-10-26 at 5 37 51 PM" src="https://user-images.githubusercontent.com/40476299/138964761-8ffeab6f-3719-4f7d-a529-dfd3c9e84fca.png">


# Modeling
* For modeling I used Logisitic Regression, XGBoost and Random Forest. I tried different techniques like SMOTE, standard scaling, onehotencoder and hyper-parameter tuning for my modeling processes to see which gives me the best model.

<img width="1012" alt="Screen Shot 2021-10-27 at 4 50 56 PM" src="https://user-images.githubusercontent.com/40476299/139145169-dec3f87c-d120-4cef-92cc-5aa4176b9718.png">

* For my final model, Random Forest was my best preforming model with an accuracy score of 94% and precision score of 83%.

![image](https://user-images.githubusercontent.com/40476299/139138731-69f17651-e4c6-4a38-bb0a-82971acefeb6.png)


# Conclusion
In conclusion, my best model for predicting the probabilty of whether a listing would be booked or not was Random Forest. This model is could also be useful for other airbnb listings in other cities. This model could also be useful for airbnb host to help figure out what features could help improve there listing to be booked.

# Next Steps
1. Include data from other cities and comapre it to NYC

2. Look for more data with more features. For example, the date of when a listing was booked to see how maybe holidays could effecting booking

#### Link to Presentation
https://docs.google.com/presentation/d/17BPPB0jqRJ7QcawzoOdgGGsHK9e_OlYvT2EbGRj9jf8/edit?usp=sharing
