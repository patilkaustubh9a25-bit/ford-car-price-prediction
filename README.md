# Ford Car Price Prediction Using Machine Learning

## Project Overview

This project focuses on analyzing Ford used-car data and building machine learning models to predict the prices of used Ford cars using Python.

The project uses two different categorical encoding techniques — **One-Hot Encoding** and **Label Encoding** — to prepare the data and build Linear Regression prediction models. The results of both approaches are evaluated and compared to understand how the encoding techniques affect model performance.

## Project Objectives

* Perform Exploratory Data Analysis (EDA) on the Ford car dataset.
* Understand the relationships between car features and prices.
* Visualize data patterns and feature relationships using graphs and charts.
* Preprocess the data using categorical encoding and feature scaling.
* Build a car price prediction model using Linear Regression.
* Compare model performance using One-Hot Encoding and Label Encoding.
* Evaluate the models using R² and Adjusted R² scores.

## Dataset

The project uses the `ford.csv` dataset, which contains information about used Ford cars and their features.

The dataset is used for data exploration, visualization, preprocessing, model training, and price prediction.

**Dataset file:** `ford.csv`

## Technologies and Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## Project Workflow

1. Import the required Python libraries.
2. Load and explore the Ford car dataset.
3. Perform data cleaning and Exploratory Data Analysis (EDA).
4. Visualize relationships between car features and prices.
5. Preprocess categorical and numerical features.
6. Apply two different categorical encoding techniques.
7. Build Linear Regression models using both approaches.
8. Evaluate and compare model performance.

## Machine Learning Approaches

### 1. Linear Regression with One-Hot Encoding

One-Hot Encoding converts categorical features into separate binary columns. This approach allows the model to use categorical information without assigning an artificial numerical order to categories.

A Linear Regression model is trained using the preprocessed data to predict used-car prices.

### 2. Linear Regression with Label Encoding

Label Encoding converts categorical values into numerical labels. These encoded features are then used to train another Linear Regression model for price prediction.

This approach is compared with One-Hot Encoding to examine the impact of different encoding methods on prediction performance.

## Model Evaluation and Results

The two models are evaluated using the following metrics:

* **R² Score:** Measures how well the model explains the variation in car prices.
* **Adjusted R² Score:** Measures model fit while accounting for the number of predictors.

Based on the saved outputs in the notebook, the results are approximately:

| Encoding Technique | Model             | R² Score | Adjusted R² Score |
| ------------------ | ----------------- | -------: | ----------------: |
| One-Hot Encoding   | Linear Regression |   0.8397 |            0.8387 |
| Label Encoding     | Linear Regression |   0.7310 |            0.7307 |

The One-Hot Encoding approach achieved a higher R² score than the Label Encoding approach in the saved notebook results. This suggests that One-Hot Encoding performed better on the evaluated test split.

*Note: These scores are taken from the notebook's saved outputs and have not been independently reproduced.*

## Project Structure

```text
ford-car-price-prediction/
│
├── Ford_Car_Price_Prediction.ipynb
├── ford.csv
└── README.md
```

* `Ford_Car_Price_Prediction.ipynb` — Contains data analysis, visualizations, preprocessing, model training, and evaluation.
* `ford.csv` — Dataset used for training and evaluating the prediction models.
* `README.md` — Project documentation.

## How to Run the Project

1. Clone or download this repository.
2. Install Python and the required libraries.
3. Open the notebook using Jupyter Notebook or Google Colab.
4. Ensure `ford.csv` is available in the location expected by the notebook.
5. Run the notebook cells in order to perform the analysis and build the models.

Install the main dependencies with:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## Conclusion

This project demonstrates how machine learning can be applied to used-car price prediction using Linear Regression. Two approaches were implemented and evaluated: One-Hot Encoding and Label Encoding.

Based on the saved evaluation results, One-Hot Encoding achieved better predictive performance than Label Encoding for this dataset and test split. The project also provides practical experience in data analysis, visualization, preprocessing, feature encoding, model training, and evaluation.

## Disclaimer

This project is intended for educational purposes. The predictions are estimates based on the available dataset and model assumptions and may not reflect actual used-car market prices.


