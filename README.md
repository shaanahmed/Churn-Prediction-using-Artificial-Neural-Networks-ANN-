Title : Churn Prediction using Artificial Neural Networks (ANN)


Objective:
The goal of this project is to predict customer churn using an Artificial Neural Network (ANN) model. Customer churn refers to the scenario where customers stop doing business with a company. By predicting churn, businesses can proactively address issues and retain customers.

Dataset Details:
Dataset Used: Churn_Modelling.csv
Number of Records: 10,000
Number of Features: 14
Features Description:
Demographic Information: Geography, Gender, Age
Customer Information: Credit Score, Balance, Tenure, Number of Products
Account Activity: Has Credit Card, Is Active Member
Estimated Salary: Estimated monthly earnings
Churn Label: Whether the customer exited (1) or not (0)
Data Preprocessing:
Importing Libraries:
Libraries such as NumPy, Pandas, and Matplotlib were used for data manipulation and visualization.
Loading Data:
The dataset was loaded using Pandas.
Exploratory Data Analysis:
Summary statistics (mean, median, mode) and data shape were analyzed.
Insights like geographic distribution of customers and credit score variations were explored.
Data Cleaning:
Columns like RowNumber, CustomerId, and Surname were removed as they are irrelevant to prediction.
Encoding Categorical Variables:
Categorical columns (Geography and Gender) were one-hot encoded.
Feature Scaling:
StandardScaler was used to scale features for better ANN performance.
Modeling:
Data Splitting:
Dataset split into training (80%) and testing (20%) sets.
Model Architecture:
Framework: TensorFlow/Keras
Sequential model with:
Input Layer: 11 input features.
Hidden Layers:
Two layers with 13 nodes each, using Sigmoid and ReLU activation functions.
Batch normalization applied after each layer for stability.
Output Layer: Single neuron with Sigmoid activation for binary classification.
Model Compilation:
Optimizer: Adam
Loss Function: Binary Crossentropy
Metrics: Accuracy
Training:
Epochs: 30
Validation split: 20% of training data
Model Summary:

Total Parameters: 456

Evaluation:
Training Results:
Accuracy during training reached approximately 82.45%.

]Validation accuracy and loss were plotted.
Testing Results:Achieved a test accuracy of 79.75%.

Visualization:Loss and accuracy trends during training were visualized for better understanding of model performance.

Key Insights:
The model performs reasonably well in predicting churn, with further potential for improvement through hyperparameter tuning and feature engineering.
Future Improvements:
Experimenting with deeper networks or alternative activation functions.
Incorporating additional customer data for better feature representation.
Using advanced optimization techniques like learning rate schedulers.
