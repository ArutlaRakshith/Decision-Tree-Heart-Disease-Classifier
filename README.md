# Decision-Tree-Heart-Disease-Classifier
Heart disease prediction using Decision Tree classification. Includes EDA, preprocessing, 80/20 evaluation, accuracy, confusion matrix insights, tree depth analysis, and manual tuning with Gini, Entropy, and min_samples_leaf.

````
# Heart Disease Prediction using Decision Tree

This project uses a **Decision Tree Machine Learning model** to predict whether a patient has heart disease (**Disease / No Disease**) using real medical data.

---

## 📌 Project Overview
- Model used: **Decision Tree Classifier**
- Task: **Binary Classification (0 = No Disease, 1 = Disease)**
- Dataset: 205+ patient health records
- Best model result:  
  - **Training Accuracy: 100%**
  - **Testing Accuracy: ~98.5%**
  - This shows the model learned medical patterns well and predicts unseen data reliably.

---

## 📊 Notebook Outcomes Summary
| Parameter | Result |
|---|---|
| Best `max_depth` | **None (Deep Tree)** |
| Train Accuracy | **1.0 (100%)** |
| Test Accuracy | **0.985 (98.5%)** |
| Precision (Class 0) | **0.97** |
| Recall (Class 0) | **1.00** |
| F1 (Class 0) | **0.99** |
| Precision (Class 1) | **1.00** |
| Recall (Class 1) | **0.97** |
| F1 (Class 1) | **0.99** |
| Fit Analysis | **Good Fit, Mild Overfitting but Generalizes Strongly** |

🔍 *Interpretation:*  
The model predicts both classes very well. **Class 0 has perfect recall**, meaning all healthy patients were identified correctly. **Class 1 also performs strong**, missing only a few cases.

---

## 🧠 How Decision Tree Makes Predictions (Simple Example)
The tree learns rules like:
- **Is blood pressure high?**
- **Is sugar level abnormal?**
- **Is heart rate low or high?**

Using these conditions, it moves through the tree and predicts:
```
New Patient Record → Disease (1) or No Disease (0)
```

---

## ⚙️ Hyperparameter Tuning Done
- Compared **Gini vs Entropy** split criteria
- Tried **min_samples_leaf (2 & 5)** manually to reduce noise
- Analyzed tree depth impact to avoid underfitting
- Visualized the best performing tree with features and class labels

---

## ✨ Conclusion
Decision Trees are fast, easy to interpret, and work well for medical datasets. The best model here shows high test accuracy and strong classification scores, making it reliable for heart disease prediction tasks.

---

## 🚀 How to Use
1. Open the notebook
2. Run all cells from top to bottom
3. The model will train and predict results
4. You can also test with new patient values using `model.predict()`

