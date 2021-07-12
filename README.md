# heart-disease-classification
<p align="center">
<img src="https://user-images.githubusercontent.com/86231828/125233921-ec6ea700-e322-11eb-9489-69c68c285727.png" width="500" height=auto>
</p>

## An end-to-end machine learning analysis to predict heart disease
This is a repository storing a complete data analysis and modeling workflow which aims to predict heart disease in a patient, provided a patient's record. A Jupyter notebook detailing the statement of the problem, data exploration, and supervised model training is provided above, along with the trained models and dataset in CSV format. 

### Summary
I studed heart disease patient records from the UCI Machine Learning repository (publicly available [here](https://archive.ics.uci.edu/ml/datasets/heart+disease), as well as on [Kaggle](https://www.kaggle.com/ronitf/heart-disease-uci)) using Logarithmic Regression, K-Neighbor, and Random Forest classifiers taken from the [Scikit-Learn library](https://scikit-learn.org/stable/index.html) and [CatBoost](https://catboost.ai/). 

From the Scikit-Learn models, I found that the Logarithmic Regression performed the best after tuning the hyperparameters with a 5-fold cross validation grid-search and scored the same accuracy, 88.52%, as the CatBoost model, the latter of which was optimized to minimize log loss of the test data. CatBoost had marginally better scores in precison, recall, and therefore F1, which the receiver of characteristic curves and confusion matrices show below: 

### Evaluation of Logarithmic Regression
<p align="center">
<img src="https://user-images.githubusercontent.com/86231828/125233521-1a072080-e322-11eb-8a24-b7b679228a3e.jpg" width=auto height="300">
<img src="https://user-images.githubusercontent.com/86231828/125233399-cbf21d00-e321-11eb-9510-07e16040e6ef.png" width=auto height="300">
</p> 



## Evaluation of CatBoost Classifier
<p align="center">
<img src="https://user-images.githubusercontent.com/86231828/125233343-ae24b800-e321-11eb-9e21-cb4951f784c4.png" width=auto height="300">
<img src="https://user-images.githubusercontent.com/86231828/125233352-b41a9900-e321-11eb-80e3-085360f2d7e9.png" width=auto height="300">
</p> 
