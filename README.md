# 🍔 Food Delivery Time Prediction using Random Forest

## 📌 Project Overview

This project uses **Machine Learning to predict food delivery time** based on factors such as delivery distance, weather conditions, traffic level, time of day, vehicle type, food preparation time, and courier experience.

The main goal is to build a reliable regression model that estimates delivery time in minutes. A Decision Tree Regressor is also considered for comparison with the Random Forest model.

## 🎯 Objectives

- Analyze and understand the food delivery dataset.
- Handle missing values and preprocess categorical and numerical features.
- Apply a machine learning pipeline for data preprocessing and model training.
- Compare Decision Tree and Random Forest regression models.
- Predict delivery time for new orders.
- Save the trained pipeline for future use.

## 🛠️ Technologies Used

- **Python** — Programming language
- **Pandas & NumPy** — Data manipulation and numerical operations
- **Matplotlib & Seaborn** — Data visualization
- **Scikit-learn** — Data preprocessing, pipelines, model training, and evaluation
- **Jupyter Notebook** — Development environment

## 📂 Dataset

The project uses `Food_Delivery_Times.csv`.

The dataset contains features related to food delivery, including:

| Feature | Description |
|---|---|
| `Distance_km` | Delivery distance in kilometers |
| `Weather` | Weather conditions |
| `Traffic_Level` | Traffic conditions |
| `Time_of_Day` | Time of the delivery |
| `Vehicle_Type` | Type of delivery vehicle |
| `Preparation_Time_min` | Food preparation time |
| `Courier_Experience_yrs` | Courier's experience in years |
| `Delivery_Time_min` | Target variable to predict |

`Order_ID` is removed before model training because it is an identifier rather than a useful delivery-time feature.

## ⚙️ Project Workflow

1. **Data Loading:** Import the dataset using Pandas.
2. **Exploratory Data Analysis:** Inspect the dataset, identify missing values, and analyze the target variable's distribution.
3. **Data Transformation:** Apply a logarithmic transformation to the target variable to reduce its skewness.
4. **Train-Test Split:** Divide the dataset into training and testing sets using an 80:20 split.
5. **Data Preprocessing:** Use `SimpleImputer` to handle missing values and `OneHotEncoder` to encode categorical features.
6. **Pipeline Creation:** Combine preprocessing and model training into a Scikit-learn pipeline.
7. **Model Training:** Train a Decision Tree Regressor and a Random Forest Regressor.
8. **Model Evaluation:** Compare model performance on training and testing data.
9. **Prediction:** Compare actual and predicted delivery times and test predictions on a new order.
10. **Model Saving:** Save the complete pipeline for potential future use.

## 🌳 Why Random Forest?

Random Forest is an ensemble learning algorithm that combines multiple decision trees to make predictions.

Instead of relying on a single decision tree, it combines predictions from many trees. This can improve generalization and help reduce overfitting compared with an individual tree.

In this project, the Random Forest model uses **100 decision trees**, as described in the notebook.

## 📊 Key Concepts Learned

- Regression and supervised machine learning
- Exploratory data analysis
- Target-variable transformation
- Handling missing data
- Categorical feature encoding
- `Pipeline` and `ColumnTransformer`
- Decision Tree vs. Random Forest
- Model evaluation and prediction
- Saving a trained machine learning pipeline

## 🚀 How to Run the Project

1. Clone or download this repository.
2. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

3. Place `Food_Delivery_Times.csv` in the appropriate project directory.
4. Open `Random_Forest.ipynb` in Jupyter Notebook or Google Colab.
5. Run the notebook cells in order.

## 🔮 Future Improvements

- Evaluate performance using MAE, RMSE, and R².
- Tune Random Forest hyperparameters to improve predictions.
- Visualize feature importance.
- Build a simple web application for delivery-time predictions.
- Deploy the trained model using Streamlit or FastAPI.

## 👩‍💻 Author

**Jyotsana Tripathi**

Aspiring Data Scientist | Machine Learning Enthusiast

---

⭐ If you find this project interesting, feel free to explore the repository and share your feedback.
