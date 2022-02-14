# Credit_Risk_Analysis

Using a dataset from LendingClub, a peer-to-peer lending services company, we will use different techniques to train and evaluate models with unbalanced classes. We will use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Also, we will Oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. We will compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, in order to predict credit risk. 


## Resources
Data Source: LoanStats_2019Q1.csv
Software: 
* Python
* Anaconda Navigator 
* Conda 
* Jupyter Notebook 

## Results

1. RandomOverSampler
* Balanced Accuracy Score

![randomoversamplerBAS](https://user-images.githubusercontent.com/88118587/153804072-be3d9dee-b628-41e4-ac18-c4d8cf47d3da.jpg)

* Imbalace Clasification Report

![randomoversamplerICR](https://user-images.githubusercontent.com/88118587/153804074-2e425926-3281-49ad-ad31-6f64c6c372dd.jpg)

* Confusion Matrix

![randomoversamplerCM](https://user-images.githubusercontent.com/88118587/153804075-e8c09f3f-7998-48de-bf16-16590b124f61.jpg)

2. SMOTE

* Balanced Accuracy Score

![SMOTEBAS](https://user-images.githubusercontent.com/88118587/153804774-66f19035-ccb4-45c0-89d5-b7daba45eebc.jpg)

* Imbalace Clasification Report

![SMOTEICR](https://user-images.githubusercontent.com/88118587/153804773-86149aa4-2bbe-4b77-9d43-f0c048af1ccb.jpg)

* Confusion Matrix

![SMOTECM](https://user-images.githubusercontent.com/88118587/153804771-544d5d17-c6a8-4bf0-80c5-5d0ebafa5591.jpg)

3. ClusterCentroids

* Balanced Accuracy Score

![SMOTEUNDERSAMPINGBAS](https://user-images.githubusercontent.com/88118587/153805286-a47731ec-8f10-4564-880f-9902185c0cad.jpg)

* Imbalace Clasification Report

![SMOTEUNDERSAMPINGICR](https://user-images.githubusercontent.com/88118587/153805284-0bd8f94f-f0b9-46f6-9481-b1b05b0b18dc.jpg)

* Confusion Matrix

![SMOTEUNDERSAMPINGCM](https://user-images.githubusercontent.com/88118587/153805285-f2aa1ca7-63f0-4aca-a7cc-d1b5775d392a.jpg)

4. SMOTEENN

* Balanced Accuracy Score

![SMOTECOMBBAS](https://user-images.githubusercontent.com/88118587/153805619-e254f261-77e8-4212-a83e-449937fc7e08.jpg)

* Imbalace Clasification Report

![SMOTECOMBCRI](https://user-images.githubusercontent.com/88118587/153805617-f20881a9-2eba-4a9f-be35-3e820288f39d.jpg)

* Confusion Matrix

![SMOTECOMBCM](https://user-images.githubusercontent.com/88118587/153805618-34b7632d-2ac5-47f4-b329-2a3927c28550.jpg)


5. BalancedRandomForestClassifier


* Balanced Accuracy Score

![blfcBA](https://user-images.githubusercontent.com/88118587/153806422-6e3428d5-6ed0-44d6-852d-f442c6662a4a.jpg)

* Imbalace Clasification Report

![blfcicr](https://user-images.githubusercontent.com/88118587/153806420-4905ab11-ed1f-4961-994b-1e5fbeb837c3.jpg)

* Confusion Matrix

![blfccm](https://user-images.githubusercontent.com/88118587/153806423-68fc84bd-e42a-4a30-9d2a-606f537ba5d5.jpg)

6. EasyEnsembleClassifier

* Balanced Accuracy Score

![ADABAS](https://user-images.githubusercontent.com/88118587/153806669-5a81872d-a68c-41f3-9cd3-0b319e26e38e.jpg)


* Imbalace Clasification Report

![ADACRI](https://user-images.githubusercontent.com/88118587/153806667-321c4a88-8d9b-48e5-aa91-f5eaa6b42635.jpg)


* Confusion Matrix

![ADACM](https://user-images.githubusercontent.com/88118587/153806670-2afc0ca4-8e61-4745-8704-03129d2d19b3.jpg)



## Summary

After reviewing all six models, the Easy Ensemble Classifier accuracy score was exceptionally high, at 92.4% and a 7% precision rate. With these numbers, we can be sure that the most positive applications have been accurately identified. Nevertheless, the precision rate of high risk was low at 0.7. We should be aware that this might not be suitable for this business model, since we cannot rely on the model to recognize all high risk applications correctly.
Despite the fact that this was the most accurate model, it cannot be completely trusted, since it doesn't recognize the high risk applications.  We should look for new ways to improve this model, and try different variables in our other models. 

