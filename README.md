# Bulldozer Price Prediction using Machine Learning

## 📋 Project Overview
This project predicts the sale price of bulldozers using machine learning algorithms. The goal is to build a regression model that can accurately estimate bulldozer prices based on their characteristics and historical sales data.

## 🎯 Problem Statement
How well can we predict the future sale price of a bulldozer, given its characteristics and previous examples of how much similar bulldozers have been sold for?

## 📊 Dataset
- **Source**: Kaggle Bluebook for Bulldozers Competition
- **Training Data**: Data through the end of 2011
- **Validation Data**: January 1, 2012 - April 30, 2012
- **Features**: 53 different attributes including machine specifications, usage patterns, and sale information

## 🛠️ Technologies Used
- **Python 3.x**
- **pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **scikit-learn** - Machine learning algorithms and tools
- **XGBoost** - Gradient boosting framework
- **CatBoost** - Gradient boosting library
- **Matplotlib** - Data visualization

## 🔄 Project Workflow

### 1. Data Collection & Preparation
- Extract data from ZIP archive
- Parse date columns and create time-based features
- Handle missing values using median/mode imputation
- Convert categorical variables to numerical format

### 2. Feature Engineering
- Create date-related features (year, month, day of week, etc.)
- Handle categorical variables with label encoding
- Create missing value indicator features

### 3. Model Development
- **Random Forest Regressor**: Ensemble method using multiple decision trees
- **XGBoost**: Gradient boosting with advanced optimization
- **CatBoost**: Gradient boosting optimized for categorical features

### 4. Model Evaluation
- Primary metric: **Root Mean Squared Log Error (RMSLE)**
- Secondary metrics: Mean Absolute Error (MAE) and R-squared (R²)

## 📈 Results

| Model | RMSLE | MAE | R² Score |
|-------|-------|-----|----------|
| Random Forest | 0.2085 | 4,499.58 | 0.8980 |
| **XGBoost** | **0.2073** | **4,411.32** | **0.9070** |
| CatBoost | 0.2205 | 4,746.61 | 0.8922 |

**Best performing model**: XGBoost with RMSLE of 0.2073 and R² of 0.9070

## 🚀 Getting Started

### Prerequisites

### Running the Project
1. Clone this repository
2. Download the dataset from [Kaggle Bluebook for Bulldozers](https://www.kaggle.com/c/bluebook-for-bulldozers/data)
3. Open `Bulldozer_price_prediction.ipynb` in Jupyter Notebook
4. Run all cells to reproduce the results

## 📁 Project Structure

## 📝 Key Insights
- XGBoost performed best with the lowest RMSLE of 0.2073
- Feature engineering, especially date-related features, significantly improved model performance
- Proper handling of missing values was crucial for model accuracy
- Ensemble methods outperformed individual algorithms

## 🔮 Future Improvements
- Hyperparameter tuning for better performance
- Feature selection to reduce overfitting
- Cross-validation for more robust evaluation
- Deploy model as a web application

## 🤝 Contributing
Feel free to fork this project and submit pull requests for any improvements.

## 📄 License
This project is open source and available under the [MIT License](LICENSE).

## 📧 Contact
**Raj** - 25f1001478@ds.study.iitm.ac.in
Project Link: https://github.com/pattern-finder-Raj/Bulldozer-price-prediction
