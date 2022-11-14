# Final-project
# Analysis and prediction in Mercamadrid (Second most important wholesale in Europe)

Manuel Buendía García

### Index:

<img src="Images/r3.png"/>

* [Purpose of the study](#section1)
* [Materials and Methods](#section2)
* [Tableau](#section3)
* [Web Scrapping](#section4)
* [Time Series and Machine learning Models](#section5)
* [Conclusion](#section6)

<a id='section1'></a>
### Purpose of the study

In my last project involved in Data Analyst bootcamp, I wanted to analyze one of the most important wholesale in Europe and the main in Spain for foodstuff
I wanted to answeer two questions and make a prediction:
Prediction:
Which would be the price per kg for certain food at the end of the year?
Questions:
which factor is encouraging a huge increase in the price?
Is there any relationship between demand and offert to impose the price per kg?

 
<a id='section2'></a>
### Materials and Methods

A dataset with more than four years of monthly data (2022 included until July) where there is information about the price per kg, ubication where food comes from, different kinds of products (fish, meat, chicken) and so on. Regarding my prediction model, I would use time series analysis in which it allows me to do it just for several foods like chicken and beaf because there is a relationship between the price and time. For other products like vegetables does not exist any relation with time and price because of the production of this kind of products do not remain steady during the year. For categories in which it is impossible to use time series (like vegetables), I create different machine learning model in which I got the best result for ramdom forest with a score for my test over 70%. As to the answeers for my question (which factor is encouraging for a huge increase in the price and if there is
any relationship between demand and offert to impose the price per kg, I use tableau to understand pattern and variation throughout years.

The methods of this study include the followings:
* Get data
* Exploratory data analyses
* Data cleaning
* Data visualization
* Check for multicollinearity
* Hypothesis testing
* Data wrangling
* Build model

<a id='section3'></a>
### Tableau
[Link to Tableau](https://public.tableau.com/app/profile/buendia.garcia/viz/Book2_16651275076100/Story2?publish=yes)

From the original dataset, I create relevant tables to analyse patterms and figure out the answers for my questions

<a id='section4'></a>
### Web Scrapping
Before making predictions and creating machine learning models, I look at economic indicators that might have a strong relationship with the price for foodstuff.

<a id='section5'></a>
### Time Series and Machine learning Models

My dataset contains a huge number of food categories. Through using the whole wheight in percent for each category compared to the rest of categories, I splitted two tables: the first one would show food categories regarding the amount of KG (If a food category value is upper or equal to 1%, I consider these category foods as relevant in KG sold) and for the next table, the same porcess but using the $ generated.

Regarding time series, as I commented before, I have used it to predict the price at the end of the year for certain food. The final result are shown in my notebook.
For the rest of categories (the vast majority), I have created three machine learning models to figure out which would be the best for my data set. Afterword, I select the machine learning model with best score. 

Machine Learning models

Decision Tree Regressor: 0.62
Linear Regression: -3.41
KNN: 0.48
Random Forest: 0.64

Random Forest would be the best one so I pick it up as my model for my data set

Train : 0.66
Test : 0.70

<a id='section6'></a>
### Conclusion
Prediction:
Which would be the price per kg for certain food at the end of the year?
Beef from caceres:
According to my predictions, the price per kg will reach almost 6 $ per KG
Chicken from Zaragoza:
The price will remain steady with a decreasing tendency at the end of the year
Regarding my questions:
which factor is encouraging a huge increase in the price?
According to what we can see in tableau and taking the example for beef (from all the origins), from january 2021 there is an increase in the trend. It could be driven by post covid effects and the sad war between Russian and Ukraine which encourage and inflaction never seen during 10 years ago.
Is there any relationship between demand and offert to impose the price per kg?
For beef products, there is not any relationship. An increase of prices do not generate a reductions of demand. It makes sense because we are talking about basic neccessities.

