# Wine Quality Prediction using Machine Learning

---

##  Objective
This project performs **multi-class classification** of wine quality (Good, Average, Bad).  
The goal is to **predict the quality of wine based on its chemical properties** using machine learning models.  
This eliminates the need for subjective manual wine tasting and provides a **faster, more consistent, and unbiased** evaluation method.

---

##  Problem Statement
Traditionally, wine quality is judged by human tasters, which can be:

- **Slow** – manual tasting takes time  
- **Costly** – requires experts  
- **Biased** – different tasters may give different results  

However, wine producers already measure chemical properties in laboratories.  
This project leverages these measurable features to **automatically classify wines** into three categories:

-  **Good**  
-  **Average**  
-  **Bad**  

---

##  Approach
1. **Data Preprocessing**  
   - Loaded the dataset and classified wine quality into Good, Average, and Bad categories  
   - Balanced the dataset using **SMOTE** to handle class imbalance  
   - Scaled features using **StandardScaler**

2. **Feature Selection**  
   - Applied **Recursive Feature Elimination (RFE)** with Random Forest to select the top features  

3. **Model Building**  
   - Trained **Random Forest** and **Gradient Boosting** classifiers  
   - Used **GridSearchCV** with Stratified K-Fold cross-validation for hyperparameter tuning  
   - Combined models using **weighted probabilities** for robust predictions  

4. **Evaluation**  
   - Achieved **99.71% accuracy** with strong precision, recall, and F1-scores across all classes  
   - Metrics used: **Confusion Matrix**, **Classification Report**

---

##  Impact / Why Useful
- Eliminates dependency on manual tasters  
- Reduces human bias  
- Provides faster and consistent results  
- Scalable to apps for **wine producers & consumers**  

---

##  Example Workflow
- **Input**: Chemical properties of a wine sample  
- **Output**: Prediction of quality → Good / Average / Bad  

Prediction also includes **class probabilities** from:  
- Random Forest  
- Gradient Boosting  
- Combined Model  

---

##  Tech Stack
- **Python**  
- **Pandas, NumPy** – Data Handling  
- **Seaborn, Matplotlib** – Visualization  
- **Scikit-learn** – ML Models, Feature Selection, Evaluation  
- **Imbalanced-learn (SMOTE)** – Data Balancing  
- **Joblib** – Model Saving & Loading  

---

##  Future Work
- Deploy the model as a **Flask/Django web app**  
- Build a **mobile app** for real-time predictions  
- Integrate **cloud storage** for large datasets  

---

##  Author
 R Rithanya  
 ravirithanya1@gmail.com  
*Wine Quality Prediction Project | Machine Learning Enthusiast*  

If this project added value to your learning or work, I’d really appreciate your support by giving it a ⭐ on GitHub.

---


