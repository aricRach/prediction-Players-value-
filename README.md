# prediction Players value project

<p >
  <img src="https://upload.wikimedia.org/wikipedia/en/thumb/f/f2/Premier_League_Logo.svg/1200px-Premier_League_Logo.svg.png" width="300" height="180" align="center">
   <img src="https://e0.365dm.com/20/06/2048x1152/skysports-premier-league-restart_5015502.jpg" width="300" height="180" align="right">
</p>




# Our Goal

In this project we tried to predict the current value of football players in the Premier League in accordance with the statistics of their performance last season.

The aim of the project was to create a machine learning model that would predict the market value of defensive players in the English Premier League.


# Data Collection

To this end, we collected data of 103 defensive players who played in the Premier League in the 2019-2020 season. For each player, we collected statistics of 24 categories that characterize the the defensive players, and form the basis for determining the market value of each player.

In addition to all of these categories, we examined for each player his current market value. This is the same variable that the model we built tries to estimate, based on the data we collected on the players

<img src="https://imgur.com/05qSnBg.png">

+ [Learn more about  the data collection and categories](https://github.com/aricRach/prediction-Players-value-/blob/master/data%20collection.pdf)


# Describing the process

First, we loaded all the data into a CSV file in order to work with it in our code. Later, we divided the data into two different sets: a set of all the categories besides the market value, and a set of all the players' market values. Furthermore, we did another division of the data – 80% of it was used to train the model, and the left 20% was used to train it. There are several training techniques for a machine learning model, and we examined a few of them. 

At first, we tried to use multiple linear regression but we noticed that this technique yields lower accuracy percentage than the Random Forest technique. We got accuracy of 78% on the training set, i.e. in 78% percent of the cases the model predicted the right value market of the player. On the other hand, when we used Random Forest model, we got accuracy of 91% on the training set. We also tried to use logistic regression model, but it produced lower accuracy percentage than Random Forest (approximately 80%).


# The development environment

The code is written in python Jupyter development environment. To write the code, the following packages were imported:

Pandas - A software library written for the Python programming language and designed for data analysis and processing. In particular, it offers data structures and operations for processing numeric data structures. We used this library to load the data from the CSV file and to divide it into two sets with which we can work as described above. Finally, all data tables are represented using functions from this directory.

Sklearn.ensemble - RandomForestRegressor - Is a library that contains basic methods to improve the generality of the estimator in a machine learning algorithm. In our project we used the Regressor of the Random Forest algorithm and used it to build the learning model that yielded the highest accuracy percentages. Also, using the methods in the library, we made market value forecasts for 20% of the players with about 76% accuracy.

sklearn.model_selection - train_test_split - Additional methods from the sklearn library that we used to divide all the data into the model training data (80% of the data) and the model examination data (20% of the data).

<p >

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/1200px-Jupyter_logo.svg.png.png" width="250" height="180" align="left">
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/Scikit_learn_logo_small.svg/1200px-Scikit_learn_logo_small.svg.png" width="250" height="180" align="left">
<img src="https://s3.amazonaws.com/lintel-blogs-static-files/wp-content/uploads/2019/07/14165137/pandas.jpg" width="250" height="180" align="center">

</p>




# User interface

We used Tkinter to develop and design the Gui which the user insert the statistics data  of the player to it and will get the predicted value according to the data he inserted.

<img src="https://imgur.com/9oBJlt3.jpg" align="left">
<img src="https://imgur.com/i2mtCgB.jpg" align="center">




