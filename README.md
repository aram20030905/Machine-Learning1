# Machine-Learning1

# Tips Prediction with Linear Regression

This project uses a dataset of restaurant tips and builds a linear regression model to predict the tip based on the total bill. It also includes data visualization using Plotly and visualizes the results to evaluate the model's performance.

## Libraries Used

- **pandas**: For data manipulation and analysis.
- **numpy**: For numerical operations.
- **plotly.express**: For interactive plots and visualizations.
- **sklearn**: For machine learning tasks such as splitting the data, training the model, and evaluation.
- **matplotlib**: For creating static plots (although only Plotly is used for interactive plots).

## Installation

To run this project, you need to install the required libraries. You can install them using `pip`:

```bash
pip install pandas numpy plotly scikit-learn seaborn matplotlib
Data Description
The dataset used in this project is the Tips dataset. It contains information about restaurant tips, with the following columns:

total_bill: The total bill amount (in dollars) for a meal.
tip: The tip given by the customer (in dollars).
sex: Gender of the customer (Male/Female).
smoker: Whether the customer is a smoker or not (Yes/No).
day: Day of the week when the meal took place.
time: Time of day (Lunch/Dinner).
size: The size of the dining party.
This dataset is often used in regression and classification tasks to understand the relationship between the total bill and the tip.

Project Description
1. Loading the Data:
The dataset is loaded from a CSV file (tips.csv) using pandas.read_csv(). The data is then displayed to help understand the structure and initial values.

2. Visualizations:
Scatter Plot: A scatter plot is created to show the relationship between the total bill and tip using Plotly's scatter() method. This helps visualize any linear relationship between the features.
Pie Chart: A pie chart is displayed showing the proportion of smokers vs non-smokers using Plotly's pie() method.
3. Data Preprocessing:
The data is split into features (X) and the target variable (y). The feature used in this regression model is total_bill, and the target is tip.

4. Splitting the Data:
The dataset is split into training and test sets using train_test_split() from sklearn.model_selection. 80% of the data is used for training, and 20% is used for testing.

5. Training the Model:
The model used is Linear Regression from sklearn.linear_model. The model is trained using the training data (X_train, y_train) to learn the relationship between the total bill and tip.

6. Model Evaluation:
Accuracy (R² Score): The model's accuracy is evaluated using the model.score() method, which calculates the R² score on the test data. This score indicates how well the model fits the test data.
Predictions: The trained model is then used to predict the tips for the test set (X_test).
7. Results Visualization:
The results are displayed in a scatter plot comparing the actual vs predicted tip amounts, using Plotly's scatter() method. This plot helps visually assess the prediction performance.
