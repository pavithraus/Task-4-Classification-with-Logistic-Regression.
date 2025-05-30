# Task-4 : Classification with Logistic Regression


##  Objective

Build a binary classifier using Logistic Regression to predict whether a tumor is malignant or benign using diagnostic features. The task includes model training, evaluation, threshold tuning, and visualizing the underlying mechanics.

---

##  Project Contents

- `data.csv` — https://github.com/pavithraus/Task-4-Classification-with-Logistic-Regression./blob/main/Breast_cancer_wisconsin.csv
- `logistic_classifier.py` — Python script for preprocessing, model training, evaluation, and visualizations
- `Visual Outputs/` — Folder containing all visual plots
- `README.md` — Project documentation

---

##  Dataset

- **Dataset**: Breast Cancer Wisconsin Diagnostic Dataset
- **Target Column**: `diagnosis`
  - `M` → Malignant (1)
  - `B` → Benign (0)

---

## 🛠 Tools & Libraries

- **Python 3.x**
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical computations
- **Matplotlib & Seaborn** — Data visualization
- **Scikit-learn** — Machine learning model building and evaluation

---

##  Workflow

1. **Data Loading & Cleaning**
   - Load the dataset from `data.csv`
   - Drop unnecessary columns (e.g., ID columns)
   - Encode categorical target variable (`diagnosis`) to numerical

2. **Exploratory Data Analysis (EDA)**
   - Visualize class distribution
   - Generate correlation heatmap
   - Plot distributions of key features

3. **Data Preprocessing**
   - Split data into training and testing sets
   - Standardize features using `StandardScaler`

4. **Model Training**
   - Train a Logistic Regression model on the training data

5. **Model Evaluation**
   - Predict on test data
   - Evaluate using:
     - Classification report (precision, recall, F1-score)
     - Confusion matrix
     - ROC curve and AUC score

6. **Threshold Tuning**
   - Adjust decision threshold (e.g., from 0.5 to 0.6)
   - Observe changes in evaluation metrics

7. **Sigmoid Function Visualization**
   - Plot the sigmoid function to understand logistic regression behavior

---

##  Results

- **Classification Report**: Provides precision, recall, F1-score for each class
- **Confusion Matrix**: Shows true vs. predicted classifications
- **ROC Curve**: Illustrates the trade-off between true positive rate and false positive rate
- **AUC Score**: Measures the area under the ROC curve

---

##  Visual Outputs

All visualizations generated during the workflow are saved in the `Visual Outputs/` directory, including:

- Class distribution plot
- ![class distribution](https://github.com/user-attachments/assets/278e433a-2d22-48f2-932d-b9e880f600c6)
- Feature correlation heatmap
- ![Feature correlation Heatmap](https://github.com/user-attachments/assets/840cfc58-325d-4117-9be6-8f9743cc9046)

- Feature distribution histograms
- ![Feature Distribution](https://github.com/user-attachments/assets/8564de2f-8d75-4c99-a56f-6b99b3f7304f)

- ROC curve
- ![ROC Curve](https://github.com/user-attachments/assets/dbe23552-3642-4c80-a0a6-f7aa40e5ba7b)

- Sigmoid function plot
- ![Sigmoid function](https://github.com/user-attachments/assets/640cf59e-b6c3-427c-b025-d121c7091a5c)


---

##  Conclusion

This project demonstrates the application of Logistic Regression for binary classification tasks, emphasizing the importance of data preprocessing, model evaluation, and threshold tuning to optimize performance.

---


