# Credit_Risk_Analysis

# Overview of the analysis

For this project we are tasked by the LendingCLub a peer-to-peer lending services company the task to predict credit risk using a set of data we were provided by the company.
To do so we are to use different algorithm used in Machine Leanrning to resample our dat with the help of libraries like imbalanced-learn and scikit-learn offered by Python.
We are using these different libraries to build models and evaluate them using a resampling method. In the first couple of models we oversampled the data using randomoversampler and smote algorithms and undersample the data with the clustercentroid algorithm. In the remaining models we used a combination approach to over and undersample the data using smoteenn. Finally, we compared two machine learning models that minimize bias, balancedrandomforestclassifier and easyensembleclassifier.

# Results

Below I will be showing the different models used as well as the results:

- Naive Random Oversampling results: Our balanced accuracy test it 65%, the precision for the high_risk has a very low positivity at 1% and the recall is 58% 


![image](https://user-images.githubusercontent.com/99924850/176739068-e763814f-d6bb-4d69-ae57-0dc9684eb990.png)

- Smote Oversampling results: Our balanced accuracy test is approximately 65%, the precision for the high_risk has a very low positivity at 1% and the recall is 68% over all

![image](https://user-images.githubusercontent.com/99924850/176739825-89e47674-a190-41d7-af7d-3a50ffc33f65.png)

- Undersampling results: Our balanced accuracy test is approximately 65%, the precision is at 99% and recall at 0.68% overall 


![image](https://user-images.githubusercontent.com/99924850/176740551-90d3ec55-0421-4481-9b34-0f6430c5611f.png)

- Combination of over and under sampling results: balanced accuracy score is 64%, the precision is 99% and the recall is 57% overall 

![image](https://user-images.githubusercontent.com/99924850/176742213-c292fb8d-07ab-429e-afae-731b9df88eba.png)



![image](https://user-images.githubusercontent.com/99924850/176742151-ae94710f-4c16-49f8-8a57-1e55f2fa1403.png)

- Balanced Random Forest Classifier results :  balanced accuracy score is 78%, the precision is 99% and the recall is 87% overall

![image](https://user-images.githubusercontent.com/99924850/176743265-56dd56ba-a66b-46fc-9ff1-61c629275f7b.png)

- Ensemnle AdaBoost Classifier results: balanced accuracy score is 93%, the precision is 99% and the recall is 94% overall

![image](https://user-images.githubusercontent.com/99924850/176745240-006fa2a7-d79a-49e1-b7fc-79fd6193db73.png)

# Summary

The common thing for all the models used is that they show a low risk precision in performing the prediction. The Ensemble Classifier seem to provide better resu;ts as its balanced accuracy score is 93% the precision is 99% and the recall rate is at 94% for high and low risk loans this means that if the model was to be used it will be able to correctly identify the high-risk cases.

As a recomendation the company migh need to further analyze the high risk cases before reaching a conclusion.




