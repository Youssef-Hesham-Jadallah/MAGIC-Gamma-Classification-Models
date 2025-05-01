# MAGIC Gamma Classification Models 🚀

This project presents a full machine learning workflow for classifying high-energy gamma-ray events using the MAGIC Gamma Telescope dataset. It compares the performance of four classification models using parameter tuning and cross-validation.

---

## 📊 Objective
To classify events as **gamma (signal)** or **hadron (background)** using:
- Decision Tree
- Naïve Bayes
- Random Forest *(with tuning)*
- AdaBoost *(with tuning)*

And to compare their performance using evaluation metrics.

---

## 📁 Dataset
- Source: [UCI MAGIC Gamma Telescope Dataset](https://archive.ics.uci.edu/ml/datasets/MAGIC+Gamma+Telescope)
- Format: CSV (no headers)
- Features: 10 numerical attributes
- Labels: `g` (gamma) or `h` (hadron)

### ⚠️ Class Imbalance
Gamma events > Hadron events. Solution: Undersample gamma events to balance the dataset.

---

## 🧠 Models Used
| Model            | Tuning Parameter(s)   | Description                                |
|------------------|------------------------|--------------------------------------------|
| Decision Tree    | None                   | Simple tree-based classifier               |
| Naïve Bayes      | None                   | Probabilistic model                        |
| Random Forest    | `n_estimators`         | Ensemble of decision trees                 |
| AdaBoost         | `n_estimators`         | Adaptive boosting over weak learners       |

---

## ⚙️ Project Structure
```
MAGIC-Gamma-Classification-Models/
│
├── data/                  # Dataset (magic04.data)
├── notebook.ipynb         # Main Jupyter Notebook
├── requirements.txt       # Python dependencies
├── README.md              # This file
└── results/               # Optional: Plots, confusion matrices
```

---

## 📈 Evaluation Metrics
Each model is evaluated using:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

---

## 🚀 How to Run
1. Clone the repository:
```bash
git clone https://github.com/your-username/MAGIC-Gamma-Classification-Models.git
```
2. Install requirements:
```bash
pip install -r requirements.txt
```
3. Download the dataset from [here](https://archive.ics.uci.edu/ml/machine-learning-databases/magic/magic04.data) and place it in the `data/` folder.
4. Open and run `notebook.ipynb`

---

## ✅ Conclusion
This project offers a clean comparison between different classification algorithms applied to an imbalanced scientific dataset. It highlights the importance of:
- Data preprocessing (balancing)
- Model selection
- Hyperparameter tuning
- Evaluation based on multiple metrics

> Great for students learning supervised classification and model comparison.

---

**Author:** *Your Name*  
**Course:** Introduction to Machine Learning, Alexandria National University

