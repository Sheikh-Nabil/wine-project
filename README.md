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
5. [Facebook Prophet](#facebook-Prophet)
6. [Flask App](#Flask-App)
7. [End Note](#End-Note)


## Introduction:

This work of this project is based on two different segmentation 
The first part of this project was to do preliminary exploration of wine data, with a goal of selecting right attributes for classifying wine into one of the quality categories: low, medium and high. Since the data was already in tidy structure, not much attention was payed in data wrangling, but finding relationships among the attributes and between attributes and the wine quality. And the second part of includes machine learning model. 



## Assessed Data:

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

