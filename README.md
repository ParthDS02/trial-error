# Classification on Imbalanced Data using Python

## 📜 Overview
This project demonstrates handling imbalanced datasets for classification tasks. Imbalanced datasets often lead to biased model predictions, favoring the majority class. The techniques applied here ensure robust and fair model performance.

---

## 🚀 Technologies Used
- **Jupyter Notebook**: For creating and running the analysis.
- **Python Libraries**:
  - `pandas`: For data manipulation.
  - `numpy`: For numerical computations.
  - `matplotlib` & `seaborn`: For data visualization.
  - `scikit-learn`: For implementing machine learning models and evaluation.

---

## 📊 Dataset
The analysis uses an insurance claims dataset with the following attributes:
- **Size**: 58,592 rows × 41 columns.
- **Target Variable**: `claim_status` (0 = No Claim, 1 = Claim).
- Features include `policy_id`, `vehicle_age`, `customer_age`, `region_density`, and others.

---

## 🌟 Results
### 1. Class Imbalance
- The dataset shows a significant imbalance:
  - Majority Class (No Claim): ~85%
  - Minority Class (Claim): ~15%

### 2. Resampling Techniques
- Applied **oversampling** and **SMOTE** to balance the classes.

### 3. Model Evaluation
| Metric          | Before Resampling | After Resampling |
|------------------|-------------------|------------------|
| **Accuracy**     | 87.5%            | 85.3%            |
| **Precision**    | 63.4%            | 72.1%            |
| **Recall**       | 42.8%            | 74.5%            |
| **F1-Score**     | 51.3%            | 73.3%            |

### 4. Visualization
![Confusion Matrix](images/confusion_matrix.png)
![Precision-Recall Curve](images/precision_recall_curve.png)

---

## ⚔️ Challenges
1. **Severe Class Imbalance**: Skewed data caused the model to favor the majority class.
   - **Solution**: Implemented resampling (Oversampling, SMOTE).
   
2. **Misleading Accuracy**: Accuracy alone was not a reliable metric for evaluating the model.
   - **Solution**: Focused on Precision, Recall, and F1-Score.

3. **High Variance in Features**: Feature scaling and encoding were necessary.
   - **Solution**: Used normalization and encoding techniques.

---

## 📈 Key Learning Outcomes
- Handling class imbalance improves recall for the minority class.
- Metrics like F1-score and Precision-Recall curves are essential for imbalanced datasets.
- Resampling techniques enhance model fairness at the cost of slightly reduced accuracy.

---

## 🛠️ Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/classification-imbalanced-data.git
