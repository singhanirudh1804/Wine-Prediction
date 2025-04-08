# 🍷 Wine Quality Classification & Analysis

This project involves data preprocessing, exploratory data analysis (EDA), classification modeling, and evaluation to classify wine types (Red or White) based on physicochemical features. The model also ranks the quality of the wine and evaluates performance using metrics like accuracy, confusion matrix, ROC-AUC, and learning curves.

## 📌 Dataset

The dataset used is `WineQT.csv`, which contains various chemical properties of wines including:

- Fixed Acidity
- pH
- Alcohol
- Citric Acid
- Quality
- Wine ID

---

## 🧪 Project Workflow

1. **Data Cleaning & Preprocessing**
   - Replaced missing values (`?`) with NaNs
   - Filled missing values using column-wise mean
   - Dropped unnecessary `Id` column

2. **Exploratory Data Analysis (EDA)**
   - Distribution plots for features like fixed acidity, pH, and alcohol
   - Scatter plots to visualize red vs white wine separation
   - Wine quality classification: Low, Medium, High
   - Countplots to analyze quality distribution

3. **Feature Engineering**
   - Created a custom feature `wine_type` based on acidity, pH, and alcohol
   - Derived a `quality_rank` based on the numeric `quality`

4. **Model Training & Evaluation**
   - Used RandomForestClassifier
   - Applied `StandardScaler` for feature normalization
   - Evaluated model with accuracy, classification report, and confusion matrix

5. **Hyperparameter Tuning**
   - Used GridSearchCV for tuning hyperparameters of Random Forest

6. **Performance Metrics**
   - ROC Curve and AUC Score
   - Cross-Validation (5-fold)
   - Feature Importance Visualization
   - Learning Curve for training and test scores

---

## 🔍 Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (sklearn)

---

## 🧠 Model Highlights

- ✅ Achieved effective classification of wine types
- 📈 Analyzed model learning behavior using learning curves
- 🎯 Performed cross-validation to ensure model generalization
- 🔍 Identified most important features influencing the prediction

---

## 📊 Results

- **Best Model**: Random Forest Classifier (after Grid Search)
- **Top Features**: Alcohol, pH, Quality
- **Classification Accuracy**: Evaluated via cross-validation and test data
- **Visualization**: Included histograms, countplots, ROC curves, feature importance bars, and learning curves

---

## 📁 Folder Structure

```bash
wine-quality-analysis/
├── WineQT.csv
├── wine_quality_analysis.ipynb (or .py)
├── README.md
