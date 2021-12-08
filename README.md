# MSc_Dissertation_Project
## Project Overview
This project is about comparative analysis of different commonly used classifiers for customer churn prediction in banking industries.
### Background
The growth of any organization depends upon their customer base. Organizations are aware of this fact that to sustain and grow in a competitive market they need to focus on customer and their needs. Every organization have a customer relationship management (CRM) team which solely focus on the customer satisfaction and to develop strategies to retain and grow their customer base. Churn is when an existing customer of a company refuse to use the product and services of the company and switch to a different company for their needs. In banking industry prospective, when an existing customer closes all the bank accounts and stops doing banking with the current bank in a given time period. Though the churn rate is low in banking industry, but the losses occurred due to the churn is huge. Banking industry product and services are limited. Most of the customers do not change banks frequently, so most of the profit drives from the existing customers. Existing customers are more likely to avail other new experimental services provided by the bank that will again add to the profit and growth. Having a loyal customer base add advantages to the reputation of the bank which will again attract more new customers. So, it is very crucial for the bank to set up strong customer retention plan and avoid customer churn.

### Dataset
The dataset considered for this experiment contains 10000 records of customers data of a retail bank. The dataset consists of 13 features variable and one target variable.The dataset contains customer demographics data, geographic data, and account related data. The dataset can be found [here](https://www.kaggle.com/mathchi/churn-for-bank-customers?select=churn.csv).

### Classifiers Used
Below 6 machine learning classifiers are used for this paper.
- Logistic Regression
- K-Nearest Neighbor (KNN)
- Support Vector Machine (SVM)
- Decision Tree (CART)
- Random Forest
- Gradient Boost

### Evaluation Metrics
To compare all the model performance, cross validation accuracy, precision and recall taken
as evaluation measure. Accuracy, Precision and Recall can be derived from the confusion
matrix. The confusion matrix consists of 4 components

**Accuracy:** It is the summation of true positive and true negative to the total number of
predictions.

**Precision:** It is the ratio of actual true positive to the total number of positive predictions.
Precision gives us insight about how many correctly predicted churners are actually churners.

**Recall:** It is the ratio of True positive prediction to the total number of True positive and
false negative. Recall gives an insight about how many numbers of actual churner we are able to predict correctly with the model.


### Results
The results can be seen in the below table

| Model | CV Accuracy | Precision | Recall |
| --- | --- | --- | --- |
| Logistic REgression | 84.06% | 76.44% | 38.59% |
| K-Nearest Neighbor | 83.37% | 70.41% | 28.88% |
| Support Vector Machine | 85.33% | 79.70% | 39.08% |
| Decision Tree | 85.51% | 77.97% | 42.96% |
| Random Forest | 86.50% | 77.97% | 44.66% |
| Gradient Boost | 86.08% | 75.57% | 48.06% |

### Conclusion
Almost all classifiers have achieved a good cv accuracy and precision score but
only one evaluation metrics which differentiates the results is recall score. As customer
churn prediction problem is to predict the actual churn customer, in this case the recall score
becomes first priority to consider. By considering the recall score as top priority then precision
and then cv score, gradient boost algorithm will be yielding the best performances among all
models followed by random forest classifier. The gradient boost algorithm can be used in
banking industry for customer churn prediction. From this experiment, we concluded that
ensemble learning based classifiers should be the best choice for customer churn prediction
problem.

# How to Run the File
This code is written in jupiter notebook and can be open and run directly in jupiter notebook.

