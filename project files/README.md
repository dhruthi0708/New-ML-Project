# 🚗 SmartPark AI

### Parking Space Availability Prediction Using Random Forest and Time-Series Models

## 📌 Project Overview

SmartPark AI is a machine learning project that predicts parking space availability using historical parking data. It combines data analysis, machine learning, and time-series forecasting to identify parking patterns and estimate future parking availability.

The project is developed using Python and can be executed in Visual Studio Code (VS Code). It aims to support smarter parking management by analyzing historical trends and generating data-driven predictions.

## 🎯 Project Objectives

* Analyze historical parking availability data.
* Perform Exploratory Data Analysis (EDA).
* Identify peak parking hours and availability patterns.
* Develop a Random Forest model for parking availability prediction.
* Apply time-series forecasting techniques.
* Evaluate model performance using appropriate metrics.
* Build a foundation for a future smart parking application.

## 🛠️ Technologies Used

| Technology         | Purpose                               |
| ------------------ | ------------------------------------- |
| Python             | Programming language                  |
| Pandas             | Data manipulation and analysis        |
| NumPy              | Numerical computations                |
| Matplotlib         | Data visualization                    |
| Seaborn            | Statistical visualization             |
| Scikit-learn       | Machine learning and model evaluation |
| Statsmodels        | Time-series forecasting               |
| Visual Studio Code | Development environment               |

## 🤖 Machine Learning Models

### 1. Random Forest

Random Forest is a supervised machine learning algorithm used to predict parking availability based on relevant features in the dataset.

**Applications:**

* Learning patterns from historical parking data.
* Predicting parking availability.
* Evaluating prediction accuracy.

### 2. Holt–Winters Exponential Smoothing

Holt–Winters is a time-series forecasting technique that models the level, trend, and seasonality of historical observations.

**Applications:**

* Identifying seasonal parking patterns.
* Forecasting future parking availability.
* Analyzing recurring changes in parking demand.

### 3. SARIMA

Seasonal Autoregressive Integrated Moving Average (SARIMA) is a statistical forecasting model that considers temporal patterns and seasonality.

The project explores the configuration:

`SARIMA(1,0,1)(1,0,1,48)`

The seasonal period of 48 is appropriate only when it matches the dataset's sampling frequency and observed seasonal cycle.

## 📊 Exploratory Data Analysis (EDA)

EDA is performed to understand the dataset before model training.

It may include:

* Inspecting dataset dimensions and data types.
* Checking missing values and duplicate records.
* Analyzing parking availability distributions.
* Visualizing trends over time.
* Identifying peak and off-peak periods.
* Examining relationships between input features.
* Preparing suitable features for machine learning.

## ⚙️ Project Workflow

1. **Data Collection:** Load the parking dataset.
2. **Data Preprocessing:** Clean the data and handle missing values.
3. **EDA:** Explore trends, distributions, and patterns.
4. **Feature Engineering:** Prepare relevant features for prediction.
5. **Model Training:** Train the Random Forest model.
6. **Time-Series Forecasting:** Apply Holt–Winters and SARIMA where appropriate.
7. **Model Evaluation:** Compare predictions with actual observations.
8. **Result Visualization:** Display important patterns and prediction results.

## 📁 Project Structure

The project can be organized in VS Code as follows:

```text
SmartPark_AI/
│
├── data/
│   └── parking_dataset.csv
│
├── notebooks/
│   └── SmartPark_AI.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── eda.py
│   ├── random_forest.py
│   └── time_series.py
│
├── models/
│
├── visualizations/
│
├── requirements.txt
├── README.md
└── .gitignore
```

*Note: This is a suggested structure. The actual files and folders may differ in your project.*

## 💻 Installation and Setup in VS Code

### Prerequisites

Install the following:

* Python 3.10 or a compatible version supported by your dependencies.
* Visual Studio Code.
* The Python extension for VS Code.
* The Jupyter extension if you are using notebooks.

### Step 1: Clone the Repository

Open the VS Code terminal and run:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your actual repository URL.

Alternatively, download the repository as a ZIP file and extract it.

### Step 2: Open the Project

Open VS Code and select:

**File → Open Folder → SmartPark_AI**

### Step 3: Create a Virtual Environment

Run the following command in the VS Code terminal:

```bash
python -m venv .venv
```

Activate it on Windows:

```powershell
.venv\Scripts\Activate.ps1
```

If you are using Command Prompt instead of PowerShell:

```cmd
.venv\Scripts\activate.bat
```

### Step 4: Install Dependencies

If a `requirements.txt` file is available, run:

```bash
python -m pip install -r requirements.txt
```

Otherwise, install the libraries required by your code:

```bash
python -m pip install pandas numpy matplotlib seaborn scikit-learn statsmodels jupyter
```

### Step 5: Run the Project

For a Python script:

```bash
python src/random_forest.py
```

For a Jupyter Notebook:

1. Open the `.ipynb` file in VS Code.
2. Select the Python kernel associated with your environment.
3. Run the notebook cells in the correct order.

Use the actual script or notebook filename from your repository.

## 📈 Model Evaluation

Model performance should be evaluated using metrics appropriate to the prediction task.

Possible metrics include:

* **MAE:** Mean Absolute Error.
* **RMSE:** Root Mean Squared Error.
* **R² Score:** Coefficient of determination for suitable regression tasks.
* **MAPE:** Mean Absolute Percentage Error, when appropriate for the data.

For classification tasks, metrics such as accuracy, precision, recall, and F1-score may be more suitable.

The final evaluation metrics should be added after running the models on the project dataset.

## 🔮 Future Enhancements

* Develop a web interface to display parking predictions.
* Integrate real-time parking occupancy data.
* Add interactive dashboards and visualizations.
* Provide location-based parking recommendations.
* Deploy the trained model as an API.
* Integrate the system with smart parking infrastructure.

## 👥 Project Information

**Project Title:** Parking Space Availability Prediction Using Random Forest and Time-Series Models

**Team:** Team-17

**Project Domain:** Machine Learning and Smart Parking

**Development Environment:** Visual Studio Code

## 📄 License

This project is developed for academic and educational purposes.
