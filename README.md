# Titanic Survival Prediction – Logistic Regression

This project uses a logistic regression model to predict passenger survival on the Titanic using engineered and preprocessed features from the original dataset.

>  Internship Project – Data Science @ Coding Samurai  
>  Achieved **80.34% accuracy** on the test set

---

##  Project Overview

This classification problem is based on the famous Titanic dataset, where the goal is to predict survival based on factors like:

- Gender
- Passenger Class
- Age
- Fare
- Family connections onboard
- Extracted Titles (Mr, Miss, etc.)

The model was built using Python, pandas, seaborn, scikit-learn, and visualized with matplotlib.

---

##  Workflow Summary

1. **Data Cleaning**  
   - Dropped `Cabin` column (too many missing values)  
   - Filled missing `Age` values with median  
   - Dropped 2 rows with missing `Embarked`

2. **Feature Engineering**  
   - `FamilySize`: SibSp + Parch + 1  
   - `IsAlone`: 1 if FamilySize == 1  
   - `Title`: extracted from Name column (e.g., Mr, Miss, etc.)

3. **Encoding & Preprocessing**  
   - Categorical features encoded using `LabelEncoder`  
   - Features scaled using `StandardScaler`

4. **Model Building**  
   - Logistic Regression (`sklearn.linear_model.LogisticRegression`)  
   - Accuracy Score: **80.34%**  
   - Confusion matrix and classification report included  
   - Feature coefficients analyzed

---

##  Results & Insights

- **Sex (female)** and **1st class** had the strongest positive impact on survival  
- Passengers **traveling alone** were less likely to survive  
- Feature `Title` helped model capture gender + social context

---

## 🛠️ Tools & Libraries

- Python
- pandas, numpy
- seaborn, matplotlib
- scikit-learn

---

##  Author

**Utsav Thapaliya**  
Data Science Intern – Coding Samurai  
