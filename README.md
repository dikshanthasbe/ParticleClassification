
## 🌌 Particle Classification using Random Forest (Internship Project)

Welcome to the repository for our internship project on **cosmic ray particle classification** using supervised machine learning. This work is inspired by the research paper:  
📄 [Composition Classification of Ultra-High Energy Cosmic Rays](https://www.mdpi.com/1099-4300/22/9/998) (Entropy, 2020)

The goal of this project is to build a machine learning model that can accurately classify **ultra-high energy primary particles** based on features simulated through the **CORSIKA Monte Carlo tool**.

---

## 🚀 Project Highlights

- 🧪 Dataset based on **simulated cosmic ray events** (proton, helium, nitrogen, iron nuclei)
- 🔬 Five input features: `MUTotal`, `ELTotal`, `Energy`, `Zenith angle`, and `NAllParticles`
- 🧠 **Random Forest Classifier** used with extensive **hyperparameter tuning** via `RandomizedSearchCV`
- 📈 Achieved **96% validation accuracy** and **93% test accuracy**
- 📊 Clear evaluation using **classification reports** and accuracy metrics
- ⏱️ Trained with 20 randomized tuning loops (each with 5-fold cross-validation)

---

## 📁 Repository Structure

```bash
├── train_val.csv       # training and validation dataset
├── test.csv            # final testing dataset
├── particlclassification.ipynb  # Final Jupyter notebook with all training and evaluation steps
├── README.md                   # Project overview and instructions
```

---

## 🧠 Model Summary

The model is based on **RandomForestClassifier** from `scikit-learn`, with parameters tuned over:

- `n_estimators`: Number of decision trees
- `max_depth`: Maximum depth of trees
- `min_samples_split`, `min_samples_leaf`: For pruning
- `bootstrap`: Sampling strategy

Validation and testing were done with stratified splits to preserve class balance. The model was evaluated using `accuracy_score` and `classification_report`.

---

## 📦 Dependencies

- Python 3.x
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`

## 📊 Sample Output

```
Validation Accuracy: 96.88%
Test Accuracy: 96.64%

Precision, Recall, F1-Score: High across all 5 particle classes
```

---

## ✍️ Author

- 👨‍💻 **Dikshant Hasbe**


---

## 📚 Reference

> Herrera, L.J., et al. (2020). *Composition Classification of Ultra-High Energy Cosmic Rays*. Entropy, 22(9), 998.  
> [Paper Link](https://www.mdpi.com/1099-4300/22/9/998)

---
