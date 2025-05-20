# 📘 SVM Optimization on Multi-Class UCI Dataset

This project focuses on optimizing Support Vector Machine (SVM) parameters for a multi-class classification problem using the **Letter Recognition** dataset from the UCI Machine Learning Repository.

---

## 📌 Objective

- Select a UCI multi-class dataset (5k–30k rows).
- Split it into 10 different 70-30 train-test splits.
- Optimize SVM parameters (kernel, C, gamma) over 20 iterations.
- Record the best accuracy and parameters per sample.
- Plot the convergence graph (accuracy vs. iteration) for the best-performing sample.
- Perform basic data analytics and upload all results to GitHub.

---

## 📊 Dataset: Letter Recognition

- 🔗 Source: [UCI Letter Recognition Dataset](https://archive.ics.uci.edu/ml/datasets/letter+recognition)
- 🧮 Samples Used: 5,000 (subset for speed)
- 📈 Classes: 26 capital letters (A–Z)
- 🔠 Target Variable: `letter` (encoded to 0–25)
- 📌 Features: 16 numerical attributes based on character image statistics

---

## 🧪 Methodology

1. Sampled 5,000 rows from the dataset.
2. Performed 10 random 70-30 train-test splits.
3. For each split:
   - Randomly selected SVM parameters over 100 iterations.
   - Trained and evaluated SVM classifier.
   - Logged best accuracy and corresponding parameters.
4. Generated convergence graph for the best-performing sample.
5. Exported results to CSV and plot as PNG.

---

## ✅ Results

| Sample | Best Accuracy | Best SVM Parameters |
|--------|----------------|---------------------|
| S1     | 0.9742         | `{'kernel': 'rbf', 'C': 10.0, 'gamma': 'auto'}` |
| S2     | 0.9758         | `{'kernel': 'rbf', 'C': 10.0, 'gamma': 'auto'}` |
| S3     | 0.9782         | `{'kernel': 'rbf', 'C': 7.8, 'gamma': 'auto'}`  |
| S4     | 0.9713         | `{'kernel': 'rbf', 'C': 3.4, 'gamma': 'auto'}`  |
| S5     | 0.9792         | `{'kernel': 'rbf', 'C': 3.4, 'gamma': 'auto'}`  |
| S6     | 0.9748         | `{'kernel': 'rbf', 'C': 7.8, 'gamma': 'auto'}`  |
| S7     | 0.9763         | `{'kernel': 'rbf', 'C': 3.4, 'gamma': 'auto'}`  |
| S8     | 0.9752         | `{'kernel': 'rbf', 'C': 8.9, 'gamma': 'auto'}`  |
| S9     | 0.9763         | `{'kernel': 'rbf', 'C': 8.9, 'gamma': 'auto'}`  |
| S10    | 0.9683         | `{'kernel': 'rbf', 'C': 4.5, 'gamma': 'auto'}`  |

📈 A convergence graph (`convergence_plot.png`) shows how the accuracy improved over iterations for the best sample.

---

## 📂 Files Included

| File Name               | Description                                         |
|------------------------|-----------------------------------------------------|
| `Parameter_Optimization_of_SVM_Assignment_5.ipynb`  | Main Python script for data loading, training, optimization |
| `convergence_plot.png` | Accuracy vs. Iteration plot for the top-performing sample |
| `README.md`            | Project documentation                              |

---

## ▶️ How to Run

1. **Install requirements:**
   ```bash
   pip install numpy pandas scikit-learn matplotlib seaborn
   ```

2. **Run the script:**
   ```bash
   python svm_optimization.py
   ```

3. **Check outputs:**
   - `svm_results.csv` – performance table
   - `convergence_plot.png` – accuracy graph

---

## 📊 Sample Analytics

- Class Distribution: Balanced among all 26 letters.
- Feature stats (mean, std, etc.) shown in terminal at runtime.

---

## 🧠 Author

Arshiya Jain – B.Tech, 3rd Year  
This project is part of an SVM optimization assignment under academic coursework of UCS654.

---

## 📌 License

This project is for academic and educational purposes only.
