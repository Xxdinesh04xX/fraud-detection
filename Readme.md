# Fraud Detection with Machine Learning On Banksim Data

Fraud is a major issue in industries like e-commerce, healthcare, and banking, costing businesses millions annually. Automated fraud detection can be done using rule-based methods or machine learning, with this repository focusing on the latter for classifying fraudulent transactions.

The dataset used here is synthetically generated, containing payments from various customers made at different times and amounts. For more details on the dataset, check the "Dataset" section for the link and the original paper under "Original Paper."

If you prefer not to run the script, here's a quick summary of the classification results from the machine learning models:

Update: These results are without the SMOTE oversampling technique. I've added a Jupyter notebook with more insights and included SMOTE to balance the dataset. The updated results are better, and you can check them in the "Fraud Detection on Bank Payments.ipynb" file in the repo.

<br/>Classification Report for K-Nearest Neighbours (1:fraudulent,0:non-fraudulent) :

|class | precision | recall | f1-score | support|
| ---- | --------- | ------ | -------- | -------|        
|  0   |   1.00    |   1.00 |  1.00    | 176233 |
|  1   |   0.83    |   0.61 |  0.70    |  2160  |
           
Confusion Matrix of K-Nearest Neigbours:
<br/> [175962    271]
<br/> [   845   1315] 



<br/>Classification Report for XGBoost : 

class | precision | recall | f1-score | support|
| ---- | --------- | ------ | -------- | -------|        
|  0   |   1.00    |   1.00 |  1.00    | 176233 |
|  1   |   0.89    |   0.76 |  0.82    |  2160  |
           
           
Confusion Matrix of XGBoost: 
<br/> [176029    204] 
<br/> [   529   1631] 




<br/>Classification Report for Random Forest Classifier : 

class | precision | recall | f1-score | support|
| ---- | --------- | ------ | -------- | -------|        
|  0   |   1.00    |   0.96 |  0.98    | 176233 |
|  1   |   0.24    |   0.98 |  0.82    |  2160  |
           
         
 Confusion Matrix of Random Forest Classifier: 
<br/> [169552   6681]
<br/> [    39   2121]



<br/>Classification Report for Ensembled Models(RandomForest+KNN+XGBoost) : 

class | precision | recall | f1-score | support|
| ---- | --------- | ------ | -------- | -------|        
|  0   |   1.00    |   1.00 |  1.00    | 176233 |
|  1   |   0.73    |   0.81 |  0.77    |  2160  |
           

Confusion Matrix of Ensembled Models: 
<br/> [175604    629]
<br/> [   417   1743]


## Dataset
https://www.kaggle.com/ntnu-testimon/banksim1
