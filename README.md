# Project Summary: From-Scratch Car Price Prediction

## 📌 Overview
A machine learning project that **manually implements** core algorithms to predict car prices (MSRP) without relying on scikit-learn's pre-built functions. All components including data preprocessing, model training, and evaluation were built from scratch.

## 🔧 Key Components
| Component               | Implementation Details                          |
|-------------------------|-----------------------------------------------|
| **Data Processing**     | Manual one-hot encoding, outlier handling      |
| **Model Architecture**  | Linear Regression (OLS) implemented manually  |
| **Dataset Splitting**   | Custom train/val/test split (60/20/20)        |
| **Feature Engineering** | Log transformation of target variable         |

## 📊 Performance Results
- Achieved **RMSE score of 0.46** on validation set
- Achieved **RMSE score of 0.47** on test set
## 📂 Project Structure
car-price-prediction/  
│
├── data/  
│   ├── processed/  
│   │   ├── df_test.pkl        # Test set features (processed)  
│   │   ├── df_train.pkl       # Training set features (processed)  
│   │   ├── df_val.pkl         # Validation set features (processed)  
│   │   ├── y_test.pkl         # Test set target (MSRP)  
│   │   ├── y_train.pkl        # Training set target (MSRP)  
│   │   ├── y_val.pkl          # Validation set target (MSRP)  
│   │   └── car_prices.csv     # Raw dataset (before preprocessing)  
│
├── plots/  
│   ├── log(1+msrp).png                     # Log-transformed MSRP distribution  
│   ├── msrp_distribution_less_100k$.png     # MSRP distribution (<$100k)  
│   ├── msrp_distribution.png                # Original MSRP distribution  
│   ├── predictions_vs_actual_distribution(5 features).png    # Model performance (5 features)  
│   └── predictions_vs_actual_distribution(more features).png # Model performance (more features)  
│
├── src/  
│   ├── __init__.py          # Python package initialization  
│   ├── EDA.ipynb            # Exploratory Data Analysis (Jupyter Notebook)  
│   └── Training.ipynb       # Model training & evaluation (Jupyter Notebook)  
│
├── venv/                    # Python virtual environment  
├── .gitignore               # Files/folders excluded from Git  
├── README.md                # Project overview & setup guide  
├── requirements.txt         # Python dependencies  
└── setup.py                 # Project setup script (if applicable)  
