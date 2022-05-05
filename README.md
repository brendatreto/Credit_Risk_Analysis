# Credit_Risk_Analysis

## Analysis Overview
The purpose of this project was to use Python to build different machine learning modes in order to predict credit risk based off on several key features.

The steps taken were as follows:
- Oversampling the data with **RandomOverSampler** algorithm
- Undersampling the data with **ClusterCentroids** algorithm
- Combinational approach of over and uncersampling with **SMOTEENN** algorithm
- Compare models with **BalancedRandomForestClassifier** and **EasyEnsembleClassifier**

## Resources
- Data: LoanStats_2019Q1.csv
- Software:
-   Python 3.7
-   Anaconda Navigator
-   Jupyter Notebook


## Results
For each of the method Balanced Accuracy Scores, Confusion Matrixes and Imbalanced Classification Reports are displayed

### Naive Random Oversampling

![ROS_acc](https://user-images.githubusercontent.com/22451540/166970693-80128886-619b-4c2b-bb02-d06c141c7d8d.PNG)
![ROS_cm](https://user-images.githubusercontent.com/22451540/166970709-2aca8eab-0852-4c9c-a9bf-a1d6c70bd5f2.PNG)
![ROS_icr](https://user-images.githubusercontent.com/22451540/166970720-9e5b0249-270f-4686-8b0d-aadc784be6a6.PNG)

Balanced Accuracy Score = 64.61%
High Risk Precision ~1% with a sensitivity of ~64% and F1 of ~2%
Low Risk Precission ~100% with a sensitivity of ~68%
