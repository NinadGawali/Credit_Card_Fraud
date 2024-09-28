# Credit_Card_Fraud
This is a project on Credit-card-fraud
Dataset Overview
Context:
This dataset contains credit card transaction data from European cardholders in September 2013, aimed at identifying fraudulent transactions. Credit card companies need to recognize such frauds to prevent unauthorized charges to customers.

Content:

Total Transactions: 284,807
Fraudulent Transactions: 492 (0.172% of total)
Class Imbalance: Highly unbalanced dataset
Key Features
Time

Description: The number of seconds elapsed from the first transaction in the dataset.
Type: Continuous numerical variable.
Amount

Description: The transaction amount. This feature is crucial for cost-sensitive learning and can be used to weigh transactions differently during model training.
Type: Continuous numerical variable.
V1, V2, ..., V28

Description: Principal components derived from PCA (Principal Component Analysis) transformation of the original features. These components capture the variance in the dataset while preserving confidentiality.
Type: Continuous numerical variables.
Class

Description: The response variable indicating whether a transaction is fraudulent (1) or not (0).
Type: Categorical variable (binary).
Explanation of Features
The dataset consists solely of numerical input variables. The use of PCA has transformed the original features for confidentiality, leading to 28 principal components (V1-V28) that provide insights into transaction patterns without revealing sensitive information.
The Time feature provides a temporal aspect to the transactions, which can be important for understanding patterns in fraudulent behavior.
The Amount feature allows for differentiation in learning based on the transaction value, potentially influencing the cost of false positives and negatives in fraud detection.
The Class variable is essential for supervised learning tasks, serving as the target for classification models.
Recommended Evaluation Metric
Due to the high class imbalance, it is recommended to measure model performance using the Area Under the Precision-Recall Curve (AUPRC) instead of traditional accuracy metrics, as the latter can be misleading in unbalanced datasets.
Acknowledgements
This dataset was collected and analyzed through a collaboration between Worldline and the Machine Learning Group at Université Libre de Bruxelles (ULB). It is part of ongoing research into big data mining and fraud detection methodologies.

References for Citing the Dataset
Dal Pozzolo, Andrea, et al. "Calibrating Probability with Undersampling for Unbalanced Classification." IEEE, 2015.
Other references related to fraud detection methodologies can be found in the publications listed in the original dataset description.
