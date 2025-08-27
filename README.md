## 🔍 Project Activities & Workflow

This project followed a structured machine learning pipeline to predict heart disease using patient health metrics. 
Below is a detailed breakdown of the activities carried out:

## 📊 Dataset Overview

The dataset contains 303 rows and 14 columns, each representing a patient record. The features include:

| Feature     | Description |
|------------|-------------|
| `age`       | Age of the patient |
| `sex`       | Gender (1 = male, 0 = female) |
| `cp`        | Chest pain type (0–3) |
| `trtbps`    | Resting blood pressure (in mm Hg) |
| `chol`      | Serum cholesterol (in mg/dl) |
| `fbs`       | Fasting blood sugar > 120 mg/dl (1 = true, 0 = false) |
| `restecg`   | Resting electrocardiographic results (0–2) |
| `thalachh`  | Maximum heart rate achieved |
| `exng`      | Exercise-induced angina (1 = yes, 0 = no) |
| `oldpeak`   | ST depression induced by exercise |
| `slp`       | Slope of the peak exercise ST segment |
| `caa`       | Number of major vessels (0–3) colored by fluoroscopy |
| `thall`     | Thalassemia (0 = normal, 1 = fixed defect, 2 = reversible defect) |
| `output`    | Target variable (1 = heart disease, 0 = no heart disease) |


### 1. 📦 Data Preparation
- Loaded the dataset (`heart.csv`) and inspected its structure.
- Handled missing values and outliers to ensure data quality.
- Encoded categorical variables and normalized numerical features where necessary.

### 2. 📊 Exploratory Data Analysis (EDA)
- Conducted univariate analysis:
  - Used **Distplots** to visualize distributions of numerical features.
  - Used **Pie Charts** to explore proportions of categorical variables.
- Conducted bivariate analysis:
  - Explored relationships between features using:
    - `FacetGrid`
    - `Count Plot`
    - `Pair Plot`
    - `Swarm Plot`
    - `Box Plot`
    - `Heatmap` (for correlation analysis)

### 3. 🧠 Model Building
We trained and evaluated four different classification algorithms:

| Model                     | Accuracy | AUC Score |
|--------------------------|----------|-----------|
| Logistic Regression      | 87%      | 88%       |
| Decision Tree Classifier | 83%      | 85%       |
| Support Vector Classifier| 83%      | 89%       |
| Random Forest Classifier | 90.3%    | 93%       |

### 4. ✅ Model Selection
After comparing performance metrics, we selected the **Random Forest Classifier** as the final model due to its superior accuracy and AUC score.

---

## 🏁 Conclusion

This project demonstrates the effectiveness of machine learning in predicting heart disease from clinical data. The Random Forest model achieved the best results and can be considered a strong candidate for deployment in a real-world diagnostic setting.

Thanks for following along — see you in the next project!

---

Would you like help formatting this into your actual `README.md` file or adding visuals like charts or model comparison plots?
