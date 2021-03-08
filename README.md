# PROJECT WINE

> “I cook with wine, sometimes I even add it to the food.”
― W.C. Fields

<p align="center">
<a href="https://www.animatedimages.org/cat-wine-706.htm"><img src="https://www.animatedimages.org/data/media/706/animated-wine-image-0042.gif" border="0" alt="animated-wine-image-0042" /></a>

# Table of Contents
1. [Introduction](#Introduction)
2. [Assessed Data](#Assessed-Data)
3. [Data Wrangling](#Data-Wrangling)
4. [Machine Learning](#Basic-Exploratory-Analysis)

1. Logistic Regression Model
2. K nearest neighbour 
3. Decision Tree Model 
4. [End Note](#End-Note)






## Introduction:

This work of this project is based on two different segmentation 
The first part of this project was to do preliminary exploration of wine data, with a goal of selecting right attributes for classifying wine into one of the quality categories: low, medium and high. Since the data was already in tidy structure, not much attention was payed in data wrangling, but finding relationships among the attributes and between attributes and the wine quality. And the second part of includes machine learning model. 



## Assessed Data: 

The data assessed in this project has the following attribute Information:

1  fixed acidity - The predominant fixed acids found in wines are tartaric, malic, citric, and succinic. Their respective levels found in wine can vary greatly but in general one would expect to see 1,000 to 4,000 mg/L tartaric acid, 0 to 8,000 mg/L malic acid, 0 to 500 mg/L citric acid, and 500 to 2,000 mg/L succinic acid.

2  volatile acidity - The primary volatile acid in wine is acetic acid, which is also the primary acid associated with the smell and taste of vinegar.

3  citric acid - Citric acid is often added to wines to increase acidity, complement a specific flavor or prevent ferric hazes. It can be added to finished wines to increase acidity and give a “fresh” flavor.

4  residual sugar - Residual sugar (or RS) refers to the sugars left unfermented in a finished wine. It is measured by grams of sugar per litre (g/l).

5  chlorides - Wine contains from 2 to 4 g L–1 of salts of mineral acids, along with some organic acids, and they may have a key role on a potential salty taste of a wine, with chlorides being a major contributor to saltiness

6  free sulfur dioxide - Free sulfur dioxide is a measure of the amount of SO2 that is not bound to other molecules, and is used to calculate molecular SO2. Sulfur Dioxide is used throughout all stages of the winemaking process to prevent oxidation and microbial growth.

7  total sulfur dioxide - Total Sulfur Dioxide (TSO2) is the portion of SO2 that is free in the wine plus the portion that is bound to other chemicals in the wine such as aldehydes, pigments, or sugars.

8  density - Density is generally used as a measure of the conversion of sugar to alcohol. Here, it’s expressed in g/cm3.

9  pH - The pH level of a wine ranges from 3 to 4. Red wines with higher acidity are more likely to be a bright ruby color, as the lower pH gives them a red hue.

10 sulphates - Both sulfates and sulfites are sulfur-based compounds.Sulfites are naturally occurring compounds found in all wines; they act as a preservative by inhibiting microbial growth. Consuming sulfites is generally harmless, and they are found in all kinds of things, from molasses to dried fruit.Even though sulfites are naturally occurring, most winemakers also add sulfur dioxide during the winemaking process to ensure against spoilage.

11 alcohol - The average glass of wine contains around 11% to 13% alcohol, but bottles range from as little as 5.5% alcohol by volume to as much as around 20% ABV.




<details>
<summary>Used Python Libraries</summary>
<pre>
import pandas as pd
import numpy as np
import statistics as st
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.model_selection import train_test_split
from collections import Counter
from sklearn.preprocessing import StandardScaler
from sklearn.preprocessing import LabelEncoder
from sklearn.linear_model import LogisticRegression
from sklearn.model_selection import cross_val_predict
from sklearn import metrics
from sklearn.metrics import accuracy_score
from sklearn.metrics import confusion_matrix
from sklearn.metrics import classification_report
from sklearn.model_selection import cross_val_score
from sklearn import svm
from sklearn.neighbors import KNeighborsClassifier
from sklearn.model_selection import GridSearchCV
from pylab import savefig


<p align="center">
<a href="https://www.animatedimages.org/cat-wine-706.htm"><img src="https://www.animatedimages.org/data/media/706/animated-wine-image-0005.gif" border="0" alt="animated-wine-image-0005" /></a><br></pre>
</details>




## Wine Type

![](https://placehold.it/100x60/ff0000/000000?text=Red)

![](https://placehold.it/100x60/157500/000?text=White)



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