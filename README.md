# 🛍️ Shopping Habits Predictor with ML
## Project Overview
This project presents a simple machine learning approach to predicting the shopping habits based on age and gender. Trained on a labeled dataset, the model is designed to make predictions for previously unseen demographic combinations. The project is built using the <code style="color : name_color">pandas</code>  and <code style="color : name_color">scikit-learn</code> libraries.

### Data Sources
The dataset used for model training was created by the author. It includes synthetic entries with age, gender, and corresponding shopping preferences.

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
The dataset was split into training and test sets using <code style="color : name_color">train_test_split</code>. To evaluate the model’s performance, we used the <code style="color : name_color">accuracy_score</code> function from <code style="color : name_color">sklearn.metrics</code>. The accuracy score may vary slightly with each execution, as the data is randomly split by default.

### Persisting the Model
The trained model was saved using the <code style="color : name_color">joblib</code> library for future use. This step allows us to make predictions without retraining the model.
### Visualizing the Desicion Tree
The structure of the trained decision tree was visualized using VSC with Graphviz Interactive Preview extension <img width="541" height="148" alt="Screenshot 2025-07-19 at 3 14 31 PM" src="https://github.com/user-attachments/assets/4d92f215-372c-418a-b015-36b2aa4c025d" />

This visualization illustrates the decision-making process of the model. The tree asks a question based on the input features (in our case, age or gender). If the condition is true, the model follows one branch, if false, it follows the other. The process continues until the model reaches a leaf node, or, in other words, the final predicted outcome.

## Final Result
![DecisionTree](https://github.com/user-attachments/assets/01ecf529-c81d-46f5-a3a4-0acb789a93f9)
