# Predicting Airbnb Bookings in NYC
![image](https://user-images.githubusercontent.com/40476299/137991634-e0f96471-4ac0-4cc6-9bcd-f867b96701d2.png)

# Business  Understanding
The purpose of this project is to generate a model that produces the the probability of a listing being reserved based on the features the listing has. This tool can be useful for an airbnb host who would like to know if there listing has a chance of being booked or not.

# Data
This data comes from the Inside Airbnb website, which is an open source tool for airbnb listings all over the world. I will be focusing on the dataset for NYC. In this dataset it contains around 36,923 rows (listings) and 74 columns (features). Below is a link to the data.

http://insideairbnb.com/new-york-city/

#### Metric
My target I will be looking at the 'has_availability' column to see if the a listing is available to be booked or not. For this project my target is binary so I will be working with classifiaction models. For my metric I will be looking at accuracy and precision. For accuracy I will be looing how accurate my models are preforming and for precision I will be looking how well my model is correctly predicting if my listing has availability to be booked or not. 

# Exploritory Data Analysis

* A boxplot of the number of amentities for a listing based on if the listing is available to be booked or no.

<img width="962" alt="Screen Shot 2021-10-26 at 5 41 51 PM" src="https://user-images.githubusercontent.com/40476299/138965225-a9a83af9-0934-4de5-89d0-dfddc2854bc5.png">


* Average price of listing in NYC

<img width="702" alt="Screen Shot 2021-10-26 at 5 40 27 PM" src="https://user-images.githubusercontent.com/40476299/138965057-0bc01195-e720-4abf-ae64-2de2930c9ba9.png">


* Created a map of different attractions in Manhattan and calculated the distance from each listing from each attraction.

<img width="778" alt="Screen Shot 2021-10-26 at 5 37 51 PM" src="https://user-images.githubusercontent.com/40476299/138964761-8ffeab6f-3719-4f7d-a529-dfd3c9e84fca.png">


# Modeling
For modeling I used Logisitic Regression, XGBoost and Random Forest. 



# Conclusion
In conclusion, my best model for predicting the probabilty of whether a listing would be booked or not was Random Forest. This could be useful for airbnb host who would like to know based on how many or the type of features they have for there listing. For example seeing how many ameneites is good to have for your listing.

# Next Steps
1. Include data from other cities and comapre it to NYC

2. Look for more data with more features. For example, the date of when a listing was booked to see how maybe holidays could effecting booking
