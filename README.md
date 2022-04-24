# Film Award Prediction

## 💡 About

Welcome! This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on oscar-nominated films from [Kaggle](https://www.kaggle.com/datasets/unanimad/the-oscar-award). Our team decided to focus on oscar-nominated films, more specifically, the number of times each film has won at the Oscar Awards as we were curious about the kinds of variables that will contribute towards a film winning at the Oscar Awards.
  
## 🧠 Contributors

| Name              |                     Area of Focus                     |GitHub Acount|
|---|:---:|---|
| Lee Si-Ying Celest|        Data Preparation and Cleaning, EDA, GitHub Repository        |@rollingsushi|
| Song Eunbin  |     EDA, Presentation Slides and Script     |@eunbinsong20|
| Yeo Jian Kai Vernon |       Data Preparation and Cleaning, EDA, Linear Regression        |@vernonyo|

## 🏃 Notebook Walkthrough
For detailed walkthrough, please view the source code in order from:

1. Data Sampling and Data Cleaning, found in: [Clean Oscar Award](https://github.com/vernonyo/Film-Awards-Predictions/blob/main/Clean-Oscar-Award.ipynb)
2. Visualisation and Exploratory Data Analysis, found in: [Data Visualization and EDA](https://github.com/vernonyo/Film-Awards-Predictions/blob/main/Data-Visualisation-and-EDA.ipynb)
3. Data Modelling using Linear Regression, found in: [Prediction](https://github.com/vernonyo/Film-Awards-Predictions/blob/main/Prediction.ipynb)

## ❓ Problem Statement

- Can we predict the number of times a film can win at the Oscars based on our predictors?
- Which model would be the best to predict it?

## 💹 Our Predictors
1. Genre of the film
2. IMDB ratings of the film upon 10
3. Runtime of the film
4. Worldwide box office sales generated
5. Languages the film was released in
6. Age ratings
7. Film director's rank
8. Sum of Top 3 Cast's ranks
9. Country of origin

## Data Selection and Preparation
- After extensively searching for various film award datasets, our team settled on a dataset for the Oscar Awards as they are regarded by many as the most prestigious and significant awards in the entertainment industry worldwide. 
- Our original dataset, found in: [Original Oscar Award Dataset](https://github.com/vernonyo/Film-Awards-Predictions/blob/main/datasets/original/the_oscar_award.csv) contains the film winners of each category for a particular year. In order to determine the number of times a film wins at the Oscars, we need to add our predictors into the dataset.
- Hence, our team had to extract the data from each of the film's IMDB page to gather each of the film's information and store it in the dataset.

## Exploratory Data Analysis (this file needs to be opened on jupyter notebook to view all the graphs)
- Here, we looked at the relationships between different variables, more importantly, our predictors with the film's number of wins at the oscars
- Our visualisation of graphs was done using different python graphing libraries such as matplotlib, seaborn and plotly.
- To make our visuals more interactive, we used plotly to allow readers to hover their mouses over the graphs and get a quick look at each of our data points.

## 🤖 Models Used
1. Decision Tree
- Another model we chose to use is the decision tree as it predicts the value of a target variable by learning simple decision rules inferred from the data features.
2. Linear Regression
- For the prediction, we decided to use the Linear Regression Model. As our response is a numeric variable, classification models such as classification trees are unsuitable hence we will use the Linear Regression Model.

## 🏆 Conclusion
- The film's runtime and sales have the highest linear correlation values with the number of oscar wins.
- Director Rankings and Cast Rankings on the other hand have low linear correlation value with the number of oscar wins.
- By solely focusing on those films with casts and/or directors in the IMDB Top lists, we further established that summing the cast rankings is not a good predictor of the number of wins a film can obtain at the oscars as the correlation coefficient was near 0.
- Between the 2 models we used, the linear regression model is better at predicting the number of wins a film can get at the oscars as it gives us a numeric response, unlike the decision tree.
- From the results, we found that our mix of predictors is a poor way of predicting whether a film wins at the oscars, and how many times it wins. Hence, we can conclude that there are other factors contributing to the success of a film at the oscars. Some likely factors are trends which change rapidly over time, age group of audiences as they have their own tastes and preferences, etc.

## What did we learn from this project?
- Extracting data from various webpages using BeautifulSoup
- Linear Regression with multiple predictor variables
- Analysing our data to clean properly, such as when the film name was in the "category" column instead of the "film" column in the original dataset
- Collaborating using Github

## References
- <https://plotly.com/python/d>
- <https://matplotlib.org/3.1.1/contents.html>
- <https://plotly.com/python/d>
- <https://seaborn.pydata.org/>
- <https://www.musicgateway.com/blog/film-industry/filmmaking/movie-genres>
