# PROJECT WINE

> “I cook with wine, sometimes I even add it to the food.”
― W.C. Fields

<p align="center">
<a href="https://www.animatedimages.org/cat-wine-706.htm"><img src="https://www.animatedimages.org/data/media/706/animated-wine-image-0042.gif" border="0" alt="animated-wine-image-0042" /></a>

# Table of Contents
1. [Introduction](#Introduction)
2. [Assessed Data](#Assessed-Data)
3. [Data Processing](#Data-Processing)
4. [Machine Learning](#Basic-Exploratory-Analysis)
5. [End Note](#End-Note)






## Introduction:

This work of this project is based on two different segmentation 
The first part of this project was to do preliminary exploration of wine data, with a goal of selecting right attributes for classifying wine into one of the quality categories: low, medium and high. Since the data was already in tidy structure, not much attention was payed in data wrangling, but finding relationships among the attributes and between attributes and the wine quality. And the second part of includes machine learning model. 



## Assessed Data: 

The data assessed in this project has the following attribute Information:

 fixed acidity - The predominant fixed acids found in wines are tartaric, malic, citric, and succinic. Their respective levels found in wine can vary greatly but in general one would expect to see 1,000 to 4,000 mg/L tartaric acid, 0 to 8,000 mg/L malic acid, 0 to 500 mg/L citric acid, and 500 to 2,000 mg/L succinic acid.

volatile acidity - The primary volatile acid in wine is acetic acid, which is also the primary acid associated with the smell and taste of vinegar.

citric acid - Citric acid is often added to wines to increase acidity, complement a specific flavor or prevent ferric hazes. It can be added to finished wines to increase acidity and give a “fresh” flavor.

residual sugar - Residual sugar (or RS) refers to the sugars left unfermented in a finished wine. It is measured by grams of sugar per litre (g/l).

chlorides - Wine contains from 2 to 4 g L–1 of salts of mineral acids, along with some organic acids, and they may have a key role on a potential salty taste of a wine, with chlorides being a major contributor to saltiness

free sulfur dioxide - Free sulfur dioxide is a measure of the amount of SO2 that is not bound to other molecules, and is used to calculate molecular SO2. Sulfur Dioxide is used throughout all stages of the winemaking process to prevent oxidation and microbial growth.

total sulfur dioxide - Total Sulfur Dioxide (TSO2) is the portion of SO2 that is free in the wine plus the portion that is bound to other chemicals in the wine such as aldehydes, pigments, or sugars.

density - Density is generally used as a measure of the conversion of sugar to alcohol. Here, it’s expressed in g/cm3.

pH - The pH level of a wine ranges from 3 to 4. Red wines with higher acidity are more likely to be a bright ruby color, as the lower pH gives them a red hue.

sulphates - Both sulfates and sulfites are sulfur-based compounds.Sulfites are naturally occurring compounds found in all wines; they act as a preservative by inhibiting microbial growth. Consuming sulfites is generally harmless, and they are found in all kinds of things, from molasses to dried fruit.Even though sulfites are naturally occurring, most winemakers also add sulfur dioxide during the winemaking process to ensure against spoilage.

alcohol - The average glass of wine contains around 11% to 13% alcohol, but bottles range from as little as 5.5% alcohol by volume to as much as around 20% ABV.



<p align="center">
<a href="https://www.animatedimages.org/cat-wine-706.htm"><img src="https://www.animatedimages.org/data/media/706/animated-wine-image-0005.gif" border="0" alt="animated-wine-image-0005" /></a><br></pre>
</details>




 Wine Type found in the data -

![](https://placehold.it/100x60/ff0000/000000?text=Red)

![](https://placehold.it/100x60/157500/000?text=White)


## Data Processing:

The wine quality data set used here are was presented by [[Cortez et al., 2009]](https://www.sciencedirect.com/science/article/abs/pii/S0167923609001377?via%3Dihub). It was very well structured regarding the data types,Null values and duplicates. Processing the data was only for finding specific insights. 


## Machine Learning: 


[Decision Tree](https://scikit-learn.org/stable/modules/tree.html): 

From a high level, decision tree induction goes through 4 main steps to build the tree:

1) Begin with  training dataset, which should have some feature variables and classification or regression output.

2) Determine the “best feature” in the dataset to split the data on; more on how we define “best feature” later.
 
3) Split the data into subsets that contain the possible values for this best feature. This splitting basically defines a node on the tree i.e each node is a splitting point based on a certain feature from our data. 
 
4) Recursively generate new tree nodes by using the subset of data created from step 3. We keep splitting until we reach a point where we have optimised, by some measure, maximum accuracy while minimising the number of splits / nodes.


<p align="center">
  <img width="500" height="300" src="https://static.javatpoint.com/tutorial/machine-learning/images/decision-tree-classification-algorithm.png">
</p>




[K Nearest Neighbour](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html):

The KNN Algorithm

1) Load the data
2) Initialize K to your chosen number of neighbors
3) For each example in the data, Calculate the distance between the query example and the current example from the data.
Add the distance and the index of the example to an ordered collection

4) Sort the ordered collection of distances and indices from smallest to largest (in ascending order) by the distances
5) Pick the first K entries from the sorted collection
6) Get the labels of the selected K entries
7) If regression, return the mean of the K labels
8) If classification, return the mode of the K labels

<p align="center">
  <img width="500" height="300" src="https://miro.medium.com/max/650/1*OyYyr9qY-w8RkaRh2TKo0w.png">
</p>

[Logistic Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html):

Logistic regression is a supervised learning classification algorithm used to predict the probability of a target variable.The nature of target or dependent variable is dichotomous, which means there would be only two possible classes.

Generally, logistic regression means binary logistic regression having binary target variables, but there can be two more categories of target variables that can be predicted by it. Based on those number of categories, Logistic regression can be divided into following types −

1) Binary or Binomial: 

In such a kind of classification, a dependent variable will have only two possible types either 1 and 0. For example, these variables may represent success or failure, yes or no, win or loss etc.

2) Multinomial:

In such a kind of classification, dependent variable can have 3 or more possible unordered types or the types having no quantitative significance. For example, these variables may represent “Type A” or “Type B” or “Type C”.

3) Ordinal:

In such a kind of classification, dependent variable can have 3 or more possible ordered types or the types having a quantitative significance. For example, these variables may represent “poor” or “good”, “very good”, “Excellent” and each category can have the scores like 0,1,2,3.


<p align="center">
  <img width="500" height="300" src="https://miro.medium.com/max/800/0*gKOV65tvGfY8SMem.png">


<details>
<summary>Refferences</summary>
<pre>

https://www.javatpoint.com/machine-learning-decision-tree-classification-algorithm

https://www.tutorialspoint.com/machine_learning_with_python/classification_algorithms_logistic_regression.htm

https://towardsdatascience.com/machine-learning-basics-with-the-k-nearest-neighbors-algorithm-6a6e71d01761


## End Note:

Please follow the social media links of the author_

<!-- Please don't remove this: Grab your social icons from https://github.com/carlsednaoui/gitsocial -->

<!-- display the social media buttons in your README -->


[![alt text][1.1]][1]
[![alt text][2.1]][2]


<!-- links to social media icons -->
<!-- no need to change these -->

<!-- icons with padding -->


[1.1]: http://i.imgur.com/yCsTjba.png (google plus icon with padding)
[2.1]: http://i.imgur.com/0o48UoR.png (github icon with padding)

<!-- icons without padding -->


[1.2]: http://i.imgur.com/VlgBKQ9.png (google plus icon without padding)
[2.2]: http://i.imgur.com/9I6NRUm.png (github icon without padding)


<!-- links to your social media accounts -->
<!-- update these accordingly -->


[1]: https://myaccount.google.com/profile
[2]: https://github.com/Sheikh-Nabil

<!-- Please don't remove this: Grab your social icons from https://github.com/carlsednaoui/gitsocial -->

<a href="#top">Back to top</a>

