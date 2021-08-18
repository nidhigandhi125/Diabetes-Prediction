# Prediction of Diabeties using Machine Learning Algorithms
Diabetes scientifically termed Diabetes Mellitus is the chronic condition of high glucose in the bloodstream. The carbohydrate-rich food is broken down into glucose which is transferred into the blood. The pancreas produces a hormone known as insulin that brings the sugar from the blood to all the cells, which generates energy. However, when insulin does not play the role, glucose stays in the blood for a longer time, which can cause serious health problems. Undiagnosed diabetes can lead to serious and untreatable diseases ahead in life. The disease can affect the person irrespective of their age group and require periodic assessments for the same. There are broadly 3 types of diabetes types: Type 1, Type 2, and gestational diabetes. 
The detection at a budding stage is imminent because that can save millions of people from dying or at least extending their lifetime. In the world of technology and automation, using Artificial Intelligence for better predictive analysis can help identify it from the initial screening, and being an algorithmic process, the probability of facing an error is negligible. People of all gender and status can then afford and avoid the complications. The proposed paper gives a detailed view of understanding the work done in the field and their results.

# Overview

<ol>
  <li>Installment</li>
  <li>Dataset</li>
  <li>Methodology</li>
  <li>Resuls</li>
</ol>

# Installation
<ul>
  <li>Download Data_Analysis.ipynb </li>
  <li>Download the dataset in your working directory. </li>
  <li>Run this notebook in colab</li>
 </ul>
 
 # Dataset
 The dataset used for the implementation is PIMA dataset that is publicly available. The dataset can be downloaded from Kaggle: https://www.kaggle.com/uciml/pima-indians-diabetes-database.
 The dataset contains 768 instances and has 8 attributes that can help detect the presence of diabetes in a person. The selected dataset is a subset of a larger dataset held by the National Institutes of Diabetics and Digestive and Kidney Diseases, which targets the age from 21 years to 81 years. Diabetic patients account for 34.9% of the whole sample, whereas non-diabetic patients account for 65.1%. The dataset includes attributes like Pregnancies, Age, BMI, Insulin, Blood Pressure, Skin Thickness and Diabetes Pedigree Function. The results are marked in the outcome coulmn where '0' represents healthy person while diabetic person are marked with '1'.
 
 # Methodology
 The proposed approach first prepares the dataset to feed the module. Preprocessing helps cleaning the dataset that would further increase the efficiency of training the model. To process the module, six different algorithms are compared in order to understand which works better and more efficiently according to the approach.
 
 <ol>
  <li>Preprocessing</li>
  To seggregate important and dependent features. a correlation matrix is plotted. The correlation matrix defines the relationship between the attributes which further aids to determine important features from the rest. The values range from -1 to +1 where a positive relation is represented by the positive value while a negative value depicts a negative relationship. Top features are seperated from the rest namely Glucose, BMI, Insulin, and Age and with those attributes the dataset is fed to the model for prediction. The zero values from the dataset are filled with the mean of the individual attribute in order to let the dataset record count constant. The Min-Max Scalar is used to normalize the dataset and then finally the dataset is split into 8: 2 ratio i.e 80% for training dataset and 20% for testing and validation of the models. 
</br>
</br>
 <div align ="center">
  <img src="https://github.com/nidhigandhi125/Diabetes-Prediction/blob/main/corr.jpg" alt="Correlation Matrix" width="400" align="center"/>
</div>
  
   <li>Model Section</li>
  The approach is implemented with six machine learning algorithms individually to compare which algorithms works better than the others and can be further developed to upsurge the accuracy. The algorithms experimented are:
  <ul>
    <li>Logistic Regression</li>
    <li>K Nearest Neighbors</li>
    <li>Support Vector Machine</li>
    <li>Naive Bayes</li>
    <li>Decision Tree</li>
    <li>Random Forest</li>
    <li>XGBoost</li>
  </ul>
 </ol>
 
# Results and Evaluation
The confusion matrix evaluates the performance of the models by dividing the samples into 4 classes that represent True Positives, True Negatives, False Positives, and False Negatives. The total of all the sections is represented by ‘n’ which is the sample size of the test dataset. Each algorithm is evaluated based on the evaluation matrix that included: precision, recall, f1-score, and support. The accuracies achieved are displayed in the table below: 

<table  align="center">
  <th>Models</th>
  <th>Accuracy</th>
  <tr>
    <td>Logistic Regression</td>
    <td>79.87%</td>
  </tr>
  <tr>
    <td>K Nearest Neighbors</td>
    <td>81.81%</td>
  </tr>
  <tr>
    <td>Support Vector Machine</td>
    <td>80.51%</td>
  </tr>
  <tr>
    <td>Naive Bayes</td>
    <td>80.51%</td>
  </tr>
   <tr>
    <td>Decision Tree</td>
    <td>69.48%</td>
  </tr>
  <tr>
    <td>Random Forest</td>
    <td>77.92%</td>
  </tr>
  <tr>
    <td>XGBoost</td>
    <td>78.57%</td>
  </tr>
</table>
<div align ="center">
  <img src="https://github.com/nidhigandhi125/Diabetes-Prediction/blob/main/results.jpg" alt="Results" width="400" align="center"/>
</div>

Due to the reduced features and substitution of zero values with the mean of each attribute assisted in giving better training to the model which helped in achieving better outcomes. Based on the top four features, the models were developed that could easily reach up to 80%. Although there is quite a room to improve the accuracy and precision of the model that would benefit people in knowing if they are susceptible to diabetes early in life. 
Diabetes must be detected in its early stages if it is to be treated. This paper proposed a machine learning method for predicting diabetes levels. The method may also assist researchers in developing an accurate and useful tool that will reach physicians' tables to assist them in making better decisions about illness state.
 
