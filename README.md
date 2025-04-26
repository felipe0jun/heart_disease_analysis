# Heart Disease Prediction Using Data Mining Techniques

Project developed as part of the Data Warehouse and Machine Learning studies in the Control and Automation Engineering program at UFSC.

## 📚 About the Project

This project aims to apply data mining techniques to predict the presence of heart disease based on clinical exam data. A complete data pipeline was implemented, including ETL processes, a Data Warehouse, Machine Learning models, and Data Visualization tools.

## 🚀 Technologies Used

- **Python** — for data processing and machine learning model development
- **Google Colab** — environment for running the scripts
- **Pandas, Scikit-learn** — data manipulation and machine learning libraries
- **Google BigQuery** — data storage (Back Room)
- **Looker Studio** — dashboard creation (Front Room)
- **Docker (basic knowledge)** — for environment isolation support

## 🩺 Dataset

- **Source:** [Heart Disease - UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/45/heart+disease)
- **Instances:**  
  - 900 total
  - 300 after preprocessing
- **Features:** 13 independent variables + 1 target variable (`target`)

## 🔧 ETL Process

- **Extract:**  
  - Extract the original dataset in CSV format.
- **Transform:**  
  - Clean missing and inconsistent data.
  - Standardize data types and perform categorical encoding.
  - Create patient ID keys and dimensional tables.
- **Load:**  
  - Upload the cleaned dataset and tables to BigQuery.

## 🧠 Machine Learning

- **Model:** Decision Tree Classifier
- **Validation:** K-Fold Cross Validation (7 folds)
- **Transformations:**  
  - One Hot Encoding for categorical variables  
  - Z-score normalization
- **Results:**  
  - Training accuracy: 80%  
  - Testing accuracy: 100%  
  *(Overfitting detected due to small dataset size)*

## 📊 Data Visualization

- **Dashboard:** Built with Looker Studio, featuring queries such as:
  - Patient age range and gender analysis
  - Chest pain type analysis by age
  - Correlation between blood pressure, cholesterol levels, and diagnosis

- [View the Dashboard here](https://lookerstudio.google.com/reporting/82d12627-2d06-4cc7-ada7-62d438c2d1c9)

## ⚠️ Risks and Considerations

- Small dataset increases the risk of overfitting.
- Medical domain knowledge is important for accurate data interpretation.
- Choosing simple classifiers is crucial when working with limited datasets.

## 👨‍💻 Authors

- Felipe Jun Hatsumura
- Igor Caetano
