# Airbnb_Seattle_data_analysis- A sneak peak into Airbnb listings at Seattle.

## Table of contents
1. List of libraries used
2. Motivation for the project
3. Files in the repository
4. Summary of the analysis
5. Acknowledgements

## 1. List of libraries used
The following python libraries are imported for my analysis:
a. Numpy
b. Pandas
c. Matplotlib
d. Seaborn
e. SKlearn
f. NLTK

## 2. Motivation for the project
I chose this project as I was interested to know the aspects by which Airbnb can be able to pull customers and to help businesses monitor stay sentiment based on customer feedback and make appropriate changes:

a. Knowing the busisest times of the year as they can help understand peak seasons and price variation based on neighborhood in Seattle which allow AirBnB to regulate inventory accordingly and can acquire maximum customer satisfaction. During the off season, they can pull customers by optimizing pricing,using flexible cancellation policy,remove extra charges etc.

b. Understanding the vibe of Seattle neighborhoods can be done by **Sentiment analysis** which is often performed on textual data.

c. Price correlation to all other numerical variables in our dataset.

## 3. Files in the repository
a. The jupyter notebook with the extension .ipynb contains the code for our analysis which goes through the CRISP-DM process. It contains both the code cells and markdown cells to give a clear picture of documentation of the code.
b. README.md file which gives the synopsis of the whole project.
c. The .csv files used as datasets for the project
   reviews.csv- includes unique id for each reviewer and detailed comments.
   listings.csv-includes full description of host,neighbourhood etc and average review score  
   calendar.csv -includes listing id and the price and availability for that day.

## 4. Summary of the analysis
Using this dataset, I am going to dive in to answer the following questions and summary of the findings are as follows:
### Questions
1. What are the busiest times of the year to visit Seattle?
2. What are the price variations based on neighborhood ?
3. What is the vibe of each Seattle neighborhood using listing descriptions?
4. What are the numerical variables which have high correlation to price?

### Findings
1. **Max occupancy** at Airbnb in Seattle is recorded in the months of **June to August** with peak at **July** and min occupnacy at the start of the year from January to March.
2.a. **Southeast Magnolia** is the highest pricing neighborhood with mean price of $231.7 followed by **Portage Bay** with $227.85 and the least pricing neighborhood is **Rainier beach** with $68.5
2.b.Considering the two major property types i.e., House and Apartment, we can conclude that :
    1. **House in Portage Bay** is the highest pricing neighborhood with $340 .
    2. **Apartment in Portage Bay** is the lowest pricing neighborhood with $113.8 in the top5 neighborhoods.
3. **Roxhill** is the neighbourhood having the highest positive reviews followed by Cedar Park and Pinehurst and  **Broadway,Minor and University District** have the most negative reviews.
4. After modelling the data, I was able to get an r2score of 0.52 on  training and 0.51 on test data sets.Based on the above coefficient analysis, the features that have the most impact on price are bathrooms,bedrooms and some of the amenities like Wireless Intercom,HotTub,Air Conditioning etc.

## 5. Acknowledgements
a. The dataset was taken from Kaggle <a href="https://www.kaggle.com/datasets/airbnb/seattle?resource=download"></a>
b. Sentiment Analyzer and polarity scores are implemented from <a href="https://www.analyticsvidhya.com/blog/2021/12/different-methods-for-calculating-sentiment-score-of-text/"></a>