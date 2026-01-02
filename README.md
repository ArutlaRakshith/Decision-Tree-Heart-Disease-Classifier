# Decision-Tree-Heart-Disease-Classifier
Heart disease prediction using Decision Tree classification. Includes EDA, preprocessing, 80/20 evaluation, accuracy, confusion matrix insights, tree depth analysis, and manual tuning with Gini, Entropy, and min_samples_leaf.

````
# Decision-Tree-Heart-Disease-Classifier

A simple ML project that predicts heart disease using a Decision Tree classifier trained on 205+ patient records.

---

## Project Overview
- **Model used:** Decision Tree Classifier
- **Task:** Binary Classification (0 = No Disease, 1 = Disease)
- **Best model (max_depth=None):**
  - Train Accuracy: **100%**
  - Test Accuracy: **98.5%**
- Model shows strong learning and reliable prediction on unseen patient data.

---

## Notebook Outcomes
| Parameter | Result |
|---|---|
| Best max_depth | None (Deep Tree) |
| Train Accuracy | 1.0 |
| Test Accuracy | 0.985 |
| Precision (0) | 0.97 |
| Recall (0) | 1.00 |
| F1 (0) | 0.99 |
| Precision (1) | 1.00 |
| Recall (1) | 0.97 |
| F1 (1) | 0.99 |
| Fit Analysis | Good Fit, Mild Overfitting, Strong Generalization |

---

## Depth Analysis (Manual Experiment)
| Model | max_depth | Train Acc | Test Acc |
|---|---|---|---|
| 1 | 2 | 0.769 | 0.678 |
| 2 | 5 | 0.929 | 0.843 |
| 3 | None | 1.0 | 0.985 |

- **Shallow tree (2):** Too simple, misses multi-factor disease logic → underfits.
- **Medium tree (5):** Learns better but test score moderate → balanced learning.
- **Deep tree (None):** Best test accuracy, learned most patterns but created very specific rules → mild overfit risk.

---

## Why Decision Tree Works on This Data
- Accepts both numeric and category features
- Finds important medical signals by splitting
- No heavy computation needed
- Decisions can be traced like doctor questions

**Example rule learned by model:**  
If **heart rate < 120** and **sugar level high** → more chance of disease.

---

## Conclusion
The model predicts heart disease effectively using learned decision rules. Controlling depth and leaf size improves stability. Multi-tree methods like Random Forest and Boosting use Decision Trees because combining trees reduces errors and gives better real-world results.

---

**Author:** Arutla Rakshith (Fresher, B.Tech CSE – AI & Data Science)


