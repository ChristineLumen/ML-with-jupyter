# 🛍️ Shopping Habits Predictor with ML
## Project Overview
This project presents a simple machine learning approach to predicting the shopping habits based on age and gender. Trained on a labeled dataset, the model is designed to make predictions for previously unseen demographic combinations. The project is built using the pandas and scikit-learn libraries. 

### Data Sources
The dataset used for model training was created by the author. It includes synthetic entries with age, gender, and corresponding music genre preferences.

### Tools
- Jupyter Notebook
- Python 
  - pandas - Data Analysis
  - sklearn - Model training/testing, prediction and basic visualization
 
### Data Cleaning
As the dataset was synthetically created by the author with a limited number of rows and columns, no additional data cleaning was necessary.

## Machine Learning
### Creating Model
A Decision Tree Classifier from scikit-learn was used to train the model on a labeled dataset. The input features were age and gender, while the target (output) was shopping habits. Since the dataset does not include every possible age and gender combination, we use the trained model to predict shopping habits for new, unseen inputs.
### Measure Model Accuracy
The dataset was split into training and test sets using train_test_split. To evaluate the model’s performance, we used the accuracy_score function from sklearn.metrics. The accuracy score may vary slightly with each execution, as the data is randomly split by default.
### Persisting the Model
The trained model was saved using the <code style="color : name_color">joblib</code> library for future use, allowing for fast loading and prediction without retraining.
### Visualizing the Desicion Tree
