# Phone Purchase Prediction using Machine Learning

## Project Overview

This project uses Machine Learning to predict whether a customer will buy a phone based on their Age and Estimated Salary.

A Logistic Regression classification model is trained using customer data. After training, the model predicts the purchasing decision of a new customer.

## Project Objective

The main objective is to build a classification model that predicts a customer's buying behavior using two features:

- Age
- Estimated Salary

The target variable is `Buy`:

- `1` = Customer will buy
- `0` = Customer will not buy

## Technologies and Libraries

- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab / Jupyter Notebook

## Dataset

The project uses a CSV file named:

`Social_Network_Ads_Practice.csv`

The dataset contains the following columns:

| Column | Description |
|---|---|
| Age | Customer's age |
| Salary | Customer's estimated salary |
| Buy | Whether the customer purchases the phone (1 or 0) |

### Dataset Upload Instructions

Upload the CSV dataset to the same GitHub repository as the notebook.

1. Open your GitHub repository.
2. Click **Add file** and select **Upload files**.
3. Select `Social_Network_Ads_Practice.csv` from your computer.
4. Keep the CSV file in the main repository folder.
5. Click **Commit changes**.

Your repository should look like this:

```text
Phone-Purchase-Prediction/
│
├── README.md
├── Model_Train_BuyPhone.ipynb
└── Social_Network_Ads_Practice.csv
```

## Project Workflow

1. Import the required libraries.
2. Load the CSV dataset.
3. Explore the dataset using `head()`, `tail()`, `describe()`, `info()`, and `shape`.
4. Check for missing values.
5. Fill missing values in Age and Salary with their respective column means.
6. Separate input features (X) and target variable (Y).
7. Split the dataset into training and testing sets using a 75:25 ratio.
8. Apply StandardScaler for feature scaling.
9. Train the Logistic Regression model.
10. Make predictions using the test dataset.
11. Evaluate the model using a Confusion Matrix and Accuracy Score.
12. Predict the purchasing decision of a new customer.

## Machine Learning Model

**Algorithm:** Logistic Regression

The model uses Age and Estimated Salary as input features to predict customer purchase decisions.

The model is evaluated using:

- Confusion Matrix
- Accuracy Score

## How to Run the Project

### Using Google Colab

1. Open Google Colab.
2. Upload the Jupyter Notebook.
3. Upload the CSV dataset to the Colab environment.
4. Make sure the dataset path is correct.
5. Run all notebook cells in order.
6. Enter a new customer's age and salary when prompted.

### Using Jupyter Notebook

1. Install Python.
2. Install the required libraries:

```bash
pip install pandas matplotlib seaborn scikit-learn
```

3. Keep the notebook and CSV file in the same folder.
4. Load the dataset using:

```python
df = pd.read_csv("Social_Network_Ads_Practice.csv")
```

5. Run all notebook cells.

## Example Prediction

The notebook asks the user to enter:

```text
Enter New Customer Age:
Enter New Customer Salary:
```

The prediction result will be:

```text
Customer will Buy
```

or

```text
Customer won't Buy
```

## Notes

- This is a Machine Learning practice project.
- The prediction is based on Age and Estimated Salary.
- Missing values are handled using mean imputation.
- StandardScaler is used for feature scaling.
- Logistic Regression is used for classification.
- Predictions are estimates and do not guarantee actual customer behavior.

## Author

**Somaya Akter**
