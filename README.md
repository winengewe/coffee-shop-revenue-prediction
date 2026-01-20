# Coffee Shop Revenue Prediction ☕📊

This project analyzes the factors influencing daily revenue for a coffee shop and builds a Linear Regression model to predict revenue based on key performance metrics.

## 📌 Project Overview
The goal of this exercise is to understand what drives shop revenue and to create a predictive model that can aid in business decisions, such as analyzing the impact of increasing customer footfall.

## 📂 Dataset
The analysis uses a dataset (`coffee_shop_revenue.csv`) containing the following features:
* **Number_of_Customers_Per_Day**: Daily customer count.
* **Average_Order_Value**: Average value of an order.
* **Operating_Hours_Per_Day**: Hours the shop is open.
* **Number_of_Employees**: Staff count.
* **Marketing_Spend_Per_Day**: Daily marketing budget.
* **Location_Foot_Traffic**: Pedestrian traffic in the area.
* **Daily_Revenue**: Total revenue for the day (Target Variable).

## 🛠️ Technologies Used
* **Python 3**
* **Pandas**: For data manipulation and analysis.
* **NumPy**: For numerical operations.
* **Matplotlib**: For data visualization.
* **Scikit-Learn**: For building the Linear Regression model.

## ⚙️ Analysis Workflow
1.  **Data Loading & Inspection**: 
    * Loaded the dataset and inspected it using `.info()` and `.describe()` to understand distributions and data types.
2.  **Data Cleaning**: 
    * Checked for missing values and removed incomplete rows to ensure data quality.
3.  **Correlation Analysis**: 
    * Generated a correlation matrix to identify relationships between variables.
    * **Key Finding**: A strong positive correlation (approx. 0.74) was observed between `Number_of_Customers_Per_Day` and `Daily_Revenue`.
4.  **Visualization**: 
    * Created scatter charts to visualize the linear relationship between customer count and revenue.
5.  **Modeling**:
    * Split the data into training (70%) and testing (30%) sets.
    * Trained a **Linear Regression** model using the training data.
    * Generated predictions on the test set for evaluation.

## 🚀 How to Run
1.  Clone this repository.
2.  Ensure you have the required libraries installed:
    ```bash
    pip install pandas numpy matplotlib scikit-learn
    ```
3.  Open the notebook `coffee-shop-revenue-prediction.ipynb` in Jupyter Notebook or Google Colab.
4.  Run the cells to reproduce the analysis and model predictions.

## 📈 Results
The analysis highlights that the **Number of Customers Per Day** is a significant predictor of Daily Revenue. The Linear Regression model leverages this relationship to forecast future revenue based on expected customer traffic.
