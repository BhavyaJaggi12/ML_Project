# Student Performance Prediction Model

This project is a regression-based machine learning application designed to predict students' academic performance. It leverages multiple regression algorithms and is deployed on AWS Elastic Beanstalk for scalable and reliable access.

## 🚀 Features

- **Regression Algorithms Used**:
  - Linear Regression
  - Ridge Regression
  - Random Forest Regressor
  - XGBoost Regressor
- **Dimensionality Reduction**: PCA (Principal Component Analysis) used for transforming input data.
- **Performance Metrics**:
  - Achieved **R² Score of 0.9762** with Random Forest
  - Achieved **R² Score of 0.9955** with XGBoost
- **Deployment**:
  - Hosted on **AWS Elastic Beanstalk**
  - Built with scalable architecture and production-ready deployment pipeline

## 🧠 Model Pipeline

1. **Data Preprocessing**:
   - Handled missing values and categorical encoding
   - Balanced the dataset using appropriate techniques (if needed)
   - Applied **PCA** for feature reduction

2. **Model Training**:
   - Trained multiple regressors using cross-validation
   - Fine-tuned hyperparameters for optimal performance

3. **Evaluation**:
   - Compared models using **R² score** and **Mean Squared Error (MSE)**
   - Selected best-performing model for deployment

4. **Deployment**:
   - Flask/FastAPI-based backend (optional)
   - Packaged and deployed on **AWS Elastic Beanstalk**


## 🛠 Tech Stack

- **Python**, **scikit-learn**, **XGBoost**
- **Pandas**, **NumPy**, **Matplotlib**
- **Flask**/**FastAPI** (for serving the model)
- **AWS Elastic Beanstalk** (for deployment)

## 📊 Results

| Model              | R² Score |
|-------------------|----------|
| Linear Regression | ~0.85    |
| Ridge Regression  | ~0.88    |
| **Random Forest** | **0.9762** |
| **XGBoost**       | **0.9955** |

## 🌐 Deployment

To deploy locally:

```bash
cd app
pip install -r requirements.txt
python app.py

To deploy on AWS Elastic Beanstalk:

1.Zip the project directory

2.Create a new Elastic Beanstalk environment

3.Upload the zipped package via the AWS Console or CLI

