# Credit_Risk_Analysis

## Project overview



## Resources

- Data Source: `LoanStats_2019Q1.csv`
- Data Tools: `Pandas`, `imbalanced-learn`, `scikit-learn`
- Software: `Jupyter Notebook`

## Results

### Naive Random Oversampling Algorithm

- The accuracy to predict credit risk is **66%**. For High Risk however, with a precision score of **0.01**, recall and sensitivity of **0.71**, and F1 score of **0.02** the  model labeled many Low Risk credits as High Risk. On the other hand, the model was better at predicting Low Risk credits, with a precision score of **1.0**, recall and sensitivity of **0.60**, and F1 score of **0.75*.

![image](https://user-images.githubusercontent.com/91766276/156068929-ae7bebfa-d8f9-4a73-bf7a-4fbf8ac26ff4.png)

### SMOTE Algorithm

- The accuracy to predict credit risk is **66%**. For High Risk however, with a precision score of **0.01**, recall and sensitivity of **0.63**, and F1 score of **0.02** the  model also labeled many Low Risk credits as High Risk. On the other hand, the model was also better at predicting Low Risk credits, with a precision score of **1.0**, recall and sensitivity of **0.69**, and F1 score of **0.82*.

![image](https://user-images.githubusercontent.com/91766276/156072350-3fb6e39e-a588-4a24-9270-66237ba19dc1.png)

### Cluster Centroids Algorithm

- The accuracy to predict credit risk is **54%**. For High Risk, with a precision score of **0.01**, recall and sensitivity of **0.69**, and F1 score of **0.01** the  model also labeled many Low Risk credits as High Risk. On the other hand, the model was also better at predicting Low Risk credits, with a precision score of **1.0**, recall and sensitivity of **0.40**, and F1 score of **0.57*.

![image](https://user-images.githubusercontent.com/91766276/156073091-b5363ae2-0671-4b77-9d0f-40fcc6700998.png)

### SMOTEENN Algorithm

- The accuracy to predict credit risk is **69%**. For High Risk, with a precision score of **0.01**, recall and sensitivity of **0.80**, and F1 score of **0.02** the  model also labeled many Low Risk credits as High Risk. On the other hand, the model was also better at predicting Low Risk credits, with a precision score of **1.0**, recall and sensitivity of **0.57**, and F1 score of **0.73*.

![image](https://user-images.githubusercontent.com/91766276/156074422-7ad00ea5-c4d3-4b08-b2bf-2b659ecd5844.png)

### Balanced Random Forest Classifier Algorithm

- The accuracy to predict credit risk is **79%**. For High Risk, with a precision score of **0.03**, recall and sensitivity of **0.70**, and F1 score of **0.06** the  model also labeled many Low Risk credits as High Risk. On the other hand, the model was also better at predicting Low Risk credits, with a precision score of **1.0**, recall and sensitivity of **0.87**, and F1 score of **0.93*.

![image](https://user-images.githubusercontent.com/91766276/156075295-bc0fbe97-c83a-4c84-9ffa-82f0178e835f.png)

### Easy Ensemble AdaBoost Classifier Algorithm

- The accuracy to predict credit risk is **93%**. For High Risk, with a precision score of **0.09**, recall and sensitivity of **0.92**, and F1 score of **0.16** the  model also labeled many Low Risk credits as High Risk. On the other hand, the model was also better at predicting Low Risk credits, with a precision score of **1.0**, recall and sensitivity of **0.94**, and F1 score of **0.97*.

![image](https://user-images.githubusercontent.com/91766276/156075808-c1080ee8-18d1-4ec3-8a0a-e662d38e201b.png)

## Summary

All models are not the best to predict High Risk credits beacuse precision for all models was less than **0.04**. This means that all models labeled many Low Risk credits as High Risk. Whereas for Low Risk credits, all models are better at not predicting actual High Risk credits as Low Risk.

Analizing the `Naive Random Oversampling Algorithm`, this model is not be the best one for predicting credit risk because the model's accuracy, **66%**, is low, and the precision and recall are not good enough to state that the model will be good at classifying credit risk. The same hapens with the `SMOTE Algorithm`, one difference is that this model has a higher ability of the classifier to find all the low risk credits. Looking at the `Cluster Centroids Algorithm`, this model is the worst one for this scenario. The model's accuracy is only **54%** and it has the highest number of low risk credits predicted as high risk. The `SMOTEENN Algorithm`, is not the best one for predicting credit risk either, becasue its accuracy is **69%** and the recall for low risk credits is only **0.57** meaning that the model was not successful at finding low risk credits.

On the other hand, `Balanced Random Forest Classifier Algorithm` is better than the previosly mentioned models. Its accuracy is **79%** and the recall is higher than the previous models. However, `Easy Ensemble AdaBoost Classifier Algorithm` is the model with the highest accuracy **(93%)**, Low Risk and High Risk recall and sensitivity is higher than **0.90**.
