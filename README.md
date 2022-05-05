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

- Balanced Accuracy Score = 64.61%
- High Risk Precision ~1% with a sensitivity of ~64% and F1 of ~2%
- Low Risk Precission ~100% with a sensitivity of ~68%


### SMOTE Oversampling

![SOS_acc](https://user-images.githubusercontent.com/22451540/166972148-19ab603b-bf30-40bf-84e8-ef61e817f239.PNG)

![SOS_cm](https://user-images.githubusercontent.com/22451540/166972181-5e3c69f2-7a65-4077-975c-ec80e77413c9.PNG)

![SOS_icr](https://user-images.githubusercontent.com/22451540/166972199-781b4dec-3d99-4c2d-9e7c-c7fc21fec30c.PNG)

- Balanced Accuracy Score = 62.50%
- High Risk Precision ~1% with a sensitivity of ~63% and F1 of ~2%
- Low Risk Precission ~100% with a sensitivity of ~62%


### ClusterCentroids Undersampling

![cc_acc](https://user-images.githubusercontent.com/22451540/166972779-099327da-6ccd-4ba1-9314-1169bf95dc1f.PNG)

![cc_cm](https://user-images.githubusercontent.com/22451540/166972803-e548cab0-91a4-4625-8e52-130d1d474785.PNG)

![cc_icr](https://user-images.githubusercontent.com/22451540/166972817-ca8f6ed7-c617-4b4c-acca-d23259296798.PNG)

- Balanced Accuracy Score = 52.57%
- High Risk Precision ~1% with a sensitivity of ~59% and F1 of ~1%
- Low Risk Precission ~100% with a sensitivity of ~47%


### SMOTEENN (Over and Under) Sampling

![com_acc](https://user-images.githubusercontent.com/22451540/166974028-563521f5-bd65-4c4d-868b-bf87882b787b.PNG)

![com_cm](https://user-images.githubusercontent.com/22451540/166974047-a1a6f28e-e670-409f-a275-1ba679434c0c.PNG)

![com_icr](https://user-images.githubusercontent.com/22451540/166974080-e7f855a8-d4e3-4408-abaf-b4c4bb510ca2.PNG)

- Balanced Accuracy Score = 61.26%
- High Risk Precision ~1% with a sensitivity of ~68% and F1 of ~1%
- Low Risk Precission ~100% with a sensitivity of ~55%


### Balanced Random Forest Classifier

![brf_acc](https://user-images.githubusercontent.com/22451540/166978268-a53a4845-e84d-4372-aeae-15ef7f2008fb.PNG)

![brf_cm](https://user-images.githubusercontent.com/22451540/166978288-0bbd1ac0-e9b1-405d-8ce6-d27a83d3140f.PNG)

![brf_icr](https://user-images.githubusercontent.com/22451540/166978314-6e016c89-2637-4945-9be3-9e782a1786bd.PNG)

- Balanced Accuracy Score = 78.77%
- High Risk Precision ~4% with a sensitivity of ~67% and F1 of ~7%
- Low Risk Precission ~100% with a sensitivity of ~91%


### Easy Ensemble Classifier

![eec_acc](https://user-images.githubusercontent.com/22451540/166980073-286601fe-c011-40e2-81cf-11118d437767.PNG)

![eec_cm](https://user-images.githubusercontent.com/22451540/166980103-811ac609-42e9-4af8-b9b9-aadef6214e03.PNG)

![eec_icr](https://user-images.githubusercontent.com/22451540/166980123-a6c399ac-824e-49b6-b075-a38905d5c766.PNG)


- Balanced Accuracy Score = 92.54%
- High Risk Precision ~7% with a sensitivity of ~91% and F1 of ~14%
- Low Risk Precission ~100% with a sensitivity of ~94%


## Summary
All six models used in the credit analysis show a significant weak precision in determining if a credit risk is high (The highest being ~7% using the EasyEnsembleClassifier Model) 
This model, the EasyEnsembleClassifier also shows the highest Balanced Accuracy Score, however a significant amount of Actual High Risk Loans are wrongly classified wich would provide insufficient information for credit loaners to truly determine the risk. 
