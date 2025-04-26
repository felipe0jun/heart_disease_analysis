![image](https://github.com/user-attachments/assets/2fd3f23c-7d81-4863-a765-4b45c86b917e)# Heart Disease Prediction Using Data Mining Techniques

Project developed as part of the Data Warehouse and Machine Learning project for the Data Warehouse class at UFSC.

## 📚 About the Project

This project aims to apply data mining techniques to predict the presence of heart disease based on clinical exam data. A complete data pipeline was implemented, including ETL processes, a Data Warehouse, Machine Learning models, and Data Visualization tools.

## 🚀 Technologies Used

- **Python** — for data processing and machine learning model development
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
![image](https://github.com/user-attachments/assets/96540299-4607-4ad6-a31e-0400fa13280c)

- ![image](https://github.com/user-attachments/assets/5daf4f65-398e-4d3d-b601-fcb12724b581)
  <details>
  <summary>Analysis</summary>
  <img src="https://github.com/user-attachments/assets/5daf4f65-398e-4d3d-b601-fcb12724b581" alt="Heat Map"/>
  <img src="https://github.com/user-attachments/assets/96540299-4607-4ad6-a31e-0400fa13280c" alt="Database Diagram"/>
</details>

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
- **Analysis:**
  <details>
  <summary>Analysis</summary>
  <img src="https://github.com/user-attachments/assets/c7083b4a-54ce-4bcc-bdc2-6ccb51fe23cf" alt="Scores for Decision Tree Classifier"/>
  <img src="https://github.com/user-attachments/assets/45f6576e-3f76-4175-92d4-69ea0b4bdcd5" alt="Learning Curve"/>
  <img src="https://github.com/user-attachments/assets/cde64267-d8c6-44a4-9318-c7c6061e5e41" alt="Confusion Matrix"/>
  <img src="https://github.com/user-attachments/assets/bcc848ba-810c-42fe-8610-cbde4772a3c0" alt="Attribute Importance in Decision"/>

</details>

## 📊 Data Visualization

- **Dashboard:** Built with Looker Studio, featuring queries such as:
  - Patient age range and gender analysis
  - Chest pain type analysis by age
  - Correlation between blood pressure, cholesterol levels, and diagnosis
![image](https://github.com/user-attachments/assets/452607fe-219a-4bc5-8ce5-0f0d2d933f54)

- [View the Dashboard here](https://lookerstudio.google.com/reporting/82d12627-2d06-4cc7-ada7-62d438c2d1c9)

## ⚠️ Risks and Considerations

- Small dataset increases the risk of overfitting.
- Medical domain knowledge is important for accurate data interpretation.
- Choosing simple classifiers is crucial when working with limited datasets.

## 👨‍💻 Authors

- Felipe Jun Hatsumura
- Igor Caetano
