# Heating and Cooling Load Prediction

This project predicts the heating and cooling load requirements of buildings using various machine learning models. The goal is to predict the energy load for both heating and cooling systems based on building characteristics, helping to optimize energy consumption.

## 📂 Dataset

The dataset used in this project is the **Energy Efficiency** dataset, available from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/242/energy+efficiency). It provides information about building features and their corresponding heating and cooling load requirements. The dataset contains various features that describe the characteristics of a building and its environment, which are used to predict the energy requirements.

## 📊 Dataset Description

The dataset consists of various features such as:

- **X1 to X8**: Features representing building characteristics (e.g., wall area, roof area, temperature)
- **Y1**: Heating Load (target variable)
- **Y2**: Cooling Load (target variable)

## ⚙️ How to Run the Project

1. **Clone this repository**:
    ```bash
    git clone https://github.com/your_username/Heating_and_Cooling_Load_Prediction.git
    ```

2. **Install required libraries** manually:
    ```bash
    pip install pandas numpy matplotlib scikit-learn openpyxl
    ```

3. **Upload the dataset**:  
   Run the `hybridml.py` script. It will prompt you to upload the `ENB2012_data.xlsx` file.

4. **Run the model**:
    ```bash
    python hybridml.py
    ```

5. **View results**:  
   After running the model, the script will output the Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R²) values for various models, including:
   - **Linear Regression (MLR)**
   - **K-Nearest Neighbors (KNN)**
   - **Stacked Model (GradientBoostingRegressor)**

## 📊 Model Evaluation

## Stacked Model Performance

The Stacked Model (GradientBoosting) was evaluated for both Heating Load and Cooling Load prediction tasks. The performance metrics are summarized in the table below:

| Metric   | Heating Load | Cooling Load |
|----------|--------------|--------------|
| **MSE**  | 1.7899       | 2.3248       |
| **RMSE** | 1.3379       | 1.5247       |
| **R²**   | 0.9828       | 0.9749       |

- **MSE** (Mean Squared Error): Measures the average of the squared differences between the predicted and actual values.
- **RMSE** (Root Mean Squared Error): The square root of MSE, giving the error magnitude in the same units as the target variable.
- **R²** (R-Squared): Represents the proportion of variance explained by the model, where a value closer to 1 indicates better model performance.



