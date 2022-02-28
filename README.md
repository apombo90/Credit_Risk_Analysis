# Credit_Risk_Analysis

## Project overview

Analyzing Amazon reviews written by members of the paid Amazon Vine program, which is a service that allows manufacturers and publishers to receive reviews for their products, members that are enrolled in the program receive free products for publishing reviews. The main idea of the project is to use PySpark to perform an ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Finally, use Pandas determine if there is any bias toward favorable reviews from Vine members in the dataset.

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

- 

![image](https://user-images.githubusercontent.com/91766276/156073091-b5363ae2-0671-4b77-9d0f-40fcc6700998.png)

