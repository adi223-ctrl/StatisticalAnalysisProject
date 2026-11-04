# Flight Delay Prediction Using Machine Learning

A machine learning project that analyzes historical US domestic flight data to predict whether a flight will arrive more than 15 minutes late.

The project explores data preprocessing, feature engineering, statistical analysis, classification modelling, and model evaluation. It also includes the development of a Streamlit-based interface concept for making flight delay predictions.

## 1. Project Overview

Flight delays affect passengers, airlines, airport operations, and overall travel efficiency.

The objective of this project is to use historical flight information to identify patterns associated with arrival delays and build a machine learning classification model.

The target variable represents whether a flight arrives more than 15 minutes late.

**Prediction task:** Binary classification

- `1`: Flight arrival delay exceeds 15 minutes.
- `0`: Flight arrival delay does not exceed 15 minutes.

## 2. Project Objectives

- Explore and understand historical flight data.
- Perform data cleaning and preprocessing.
- Handle missing values.
- Apply feature engineering and categorical encoding.
- Train a Logistic Regression classification model.
- Evaluate model performance using classification metrics.
- Explore an interactive interface for flight delay prediction.

## 3. Technologies Used

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Data Analysis | Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Missing Value Imputation | KNN Imputer |
| Feature Engineering | Binary Encoding, One-Hot Encoding |
| Feature Scaling | StandardScaler |
| Model | Logistic Regression |
| Model Evaluation | Confusion Matrix, Classification Report, ROC-AUC |
| Model Serialization | Joblib |
| User Interface | Streamlit |
| Development Environment | Jupyter Notebook |

## 4. Project Structure

```text
StatisticalAnalysisProject/
│
├── pipeline.ipynb
├── app.ipynb
│
├── airlines.csv
├── airports.csv
│
├── confusion_matrix.png
├── Flight_Delay_Prediction_Explained.pdf
│
├── .gitignore
└── README.md
```

### File Descriptions

| File | Description |
|---|---|
| `pipeline.ipynb` | Main notebook for data preprocessing, feature engineering, model training and evaluation. |
| `app.ipynb` | Notebook containing the Streamlit application implementation. |
| `airlines.csv` | Airline reference information. |
| `airports.csv` | Airport reference information. |
| `confusion_matrix.png` | Visualization of classification results. |
| `Flight_Delay_Prediction_Explained.pdf` | Supporting project explanation. |

## 5. Machine Learning Workflow

The project follows these main stages:

1. **Data Collection:** Work with historical US domestic flight data.
2. **Exploratory Data Analysis:** Examine flight characteristics, distributions and delay patterns.
3. **Data Preprocessing:** Handle missing values and prepare features.
4. **Feature Engineering:** Transform categorical variables using encoding techniques.
5. **Feature Scaling:** Apply StandardScaler where required.
6. **Model Training:** Train a Logistic Regression classifier.
7. **Model Evaluation:** Evaluate predictions using classification metrics and ROC-AUC.
8. **Application Development:** Explore a Streamlit interface for user interaction.

## 6. Model Evaluation

The project uses the following evaluation techniques:

- **Confusion Matrix:** Understand correct and incorrect classifications.
- **Precision:** Measure how many predicted delayed flights were actually delayed.
- **Recall:** Measure how many actual delayed flights were correctly identified.
- **F1-Score:** Evaluate the balance between precision and recall.
- **ROC-AUC:** Assess the model's ability to distinguish between the two classes.

The repository includes a confusion matrix visualization.

## 7. How to Run the Project

### Prerequisites

- Python 3.x
- Jupyter Notebook or JupyterLab
- Required Python libraries

### Step 1: Clone the repository

```bash
git clone https://github.com/adi223-ctrl/StatisticalAnalysisProject.git

cd StatisticalAnalysisProject
```

### Step 2: Create a virtual environment

```bash
python -m venv venv
```

Activate it:

**Windows:**
```bash
venv\Scripts\activate
```

**Linux / macOS:**
```bash
source venv/bin/activate
```

### Step 3: Install dependencies

The repository does not currently include a `requirements.txt` file. Install the libraries required by the notebooks, based on their imports.

```bash
pip install pandas numpy matplotlib seaborn scikit-learn category-encoders jupyter streamlit joblib
```

### Step 4: Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `pipeline.ipynb` to explore the data preprocessing and model training workflow.

**Note:** The original training dataset (`flights.csv`) is not currently included in the repository. You will need the corresponding dataset to reproduce the complete training workflow.

The application notebook also references a saved model artifact (`flight_delay_model.pkl`) and an `app.py` file, which are not currently present in the repository. The Streamlit application therefore requires these missing files before it can be launched independently.

## 8. Limitations and Considerations

- The original flight dataset is not included in the repository.
- The trained model artifact is not included.
- The standalone Streamlit application file is not included.
- Model performance should be interpreted in the context of the available features and prediction timing.
- Features such as departure delay, taxi-out time and actual air time may only be available after flight operations have started. Therefore, this model should not be interpreted as a booking-time delay prediction system.
- Further validation is needed before using the model in a real-world operational environment.

## 9. Future Improvements

- Add a complete reproducible training dataset or a documented data-download process.
- Build a complete Scikit-learn preprocessing and modelling pipeline.
- Add a reproducible `requirements.txt`.
- Save and version the trained model.
- Complete the standalone Streamlit application.
- Introduce cross-validation and hyperparameter tuning.
- Evaluate the model on unseen and more recent flight data.
- Explore additional classification algorithms and compare their performance.

## 10. Project Information

**Project:** Flight Delay Prediction Using Machine Learning

**Repository:** [StatisticalAnalysisProject](https://github.com/adi223-ctrl/StatisticalAnalysisProject)

**Domain:** Data Science and Machine Learning

**Problem Type:** Binary Classification

---

*This project demonstrates an end-to-end machine learning workflow, from historical data analysis and preprocessing to classification modelling and evaluation.*
