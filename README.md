# 🧠 Employee Attrition Prediction

This project aims to build a machine learning model that predicts whether an employee is likely to leave a company based on HR data. The objective is to not only forecast attrition but also uncover key factors influencing it and provide actionable insights for HR decision-makers.

## 📂 Dataset

- **Source**: IBM HR Analytics Employee Attrition & Performance
- **Dataset Link**: [IBM HR Analytics Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- **Format**: CSV
- **Features**: 35 columns including demographics, work-related factors, and employee satisfaction levels.

## 🔍 Objectives

1. Perform Exploratory Data Analysis (EDA) to understand key patterns and influencing factors.
2. Train a **Logistic Regression** model to predict employee attrition.
3. Use **LIME** for model explainability to interpret why the model predicts attrition for specific employees.
4. Deliver **actionable HR strategies** to reduce future attrition.

## 📊 Exploratory Data Analysis (EDA)

- Visualized attrition distribution, feature correlations, and boxplots.
- Identified key variables such as:
  - Overtime
  - Monthly Income
  - Distance From Home
  - Job Satisfaction
  - Years at Company

## 🧪 Model Training

- **Model**: Logistic Regression
- **Preprocessing**:
  - Label Encoding for binary columns
  - One-Hot Encoding for categorical variables
  - Feature Scaling using `StandardScaler`
- **Evaluation**:
  - Precision, Recall, F1-Score
  - Confusion Matrix

## 🧠 Model Explainability

- **LIME (Local Interpretable Model-Agnostic Explanations)** is used to interpret individual predictions.
- Helps HR teams understand the reasons behind each prediction, improving trust and transparency.

## 📝 Key Results

- Achieved good classification metrics in predicting attrition.
- LIME outputs revealed that overtime and low income are major drivers of attrition.

## 📌 Actionable Insights

1. **Flexible Work Hours**: Minimize overtime to improve retention.
2. **Salary Adjustments**: Consider salary hikes for low-income employees.
3. **Remote Work Opportunities**: Help employees who live far from the workplace.
4. **Mentorship & Onboarding**: Especially for new or short-tenured employees.
5. **Work-Life Balance Programs**: Enhance job satisfaction and reduce burnout.

## 🚀 How to Run the Notebook

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/predict-employee-attrition.git
   cd predict-employee-attrition
   ```

2. **Install Required Packages**
   Make sure you have Python 3.12.8 and Jupyter Notebook installed. You can install the required libraries using pip:

   ```bash
   pip install pandas matplotlib seaborn scikit-learn lime joblib
   ```

3. **Launch the Notebook**
   ```bash
   jupyter notebook main.ipynb
   ```

4. **Explore the Analysis**
   - Follow each step in the notebook to see the data loading, cleaning, visualization, and insights process.

## Conclusion

In this project, we successfully built a machine learning model to predict employee attrition using the IBM HR Analytics dataset. We performed exploratory data analysis (EDA) to identify key factors influencing attrition and visualized the relationships between various features. The logistic regression model was trained and evaluated, achieving good accuracy in predicting whether an employee would leave the company.

Using **LIME** (Local Interpretable Model-agnostic Explanations), we gained valuable insights into how the model makes predictions, allowing for better understanding and trust in the model's decisions. The key features contributing to attrition were identified, and actionable HR retention strategies were provided based on these insights.

### Key Insights:
- Employees with high overtime, low monthly income, long distances from home, short tenure, and low job satisfaction are more likely to leave the company.
- HR strategies like flexible work hours, regular salary reviews, better onboarding, mentorship programs, and prioritizing work-life balance can help reduce attrition.

The model can be further improved with additional data or more complex machine learning algorithms. This project provides a foundation for HR departments to utilize predictive models in making data-driven decisions to enhance employee retention.
