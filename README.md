# 🌸 Iris Flower Classification and Analysis

## 📌 Overview

This project explores and analyzes the famous **Iris dataset** using various machine learning algorithms. The dataset contains features like sepal length, sepal width, petal length, and petal width of different iris species (*Setosa*, *Versicolor*, and *Virginica*). The project performs data visualization, classification, regression, clustering, hyperparameter tuning, and even includes an interactive prediction module.

---

## 📂 Project Structure

```bash
├── iris.csv                         # Dataset (if loaded manually)
├── iris_analysis.ipynb             # Full EDA and model building notebook
├── predict_species.py              # Predict flower species via user input
├── README.md                       # This file
```

---

## 🧰 Technologies Used

- Python
- NumPy, Pandas
- Matplotlib, Seaborn
- Scikit-learn
- GridSearchCV, Cross-validation

---

## 📊 Key Features

### 1. Exploratory Data Analysis (EDA)
- Data inspection and statistical summary
- Pie chart for species distribution
- Histograms, boxplots, violin plots, and density plots
- Heatmap for correlation analysis

### 2. Classification Models
- Logistic Regression
- Support Vector Machine (SVM)
- k-Nearest Neighbors (KNN)
- Naive Bayes
- Decision Tree
- Random Forest

### 3. Regression Model
- Linear Regression to predict encoded species values

### 4. Clustering
- KMeans Clustering (unsupervised learning)

### 5. Hyperparameter Tuning
- `GridSearchCV` used to optimize KNN, SVM, Logistic Regression, and Random Forest

### 6. Cross-Validation
- Evaluation of models using 5-fold cross-validation

### 7. Interactive Prediction
- Script to predict species from user input
- Visual feedback with violin plots based on predicted species

---

## 🚀 Getting Started

### Prerequisites

Make sure the following Python libraries are installed:

```bash
pip install numpy pandas seaborn matplotlib scikit-learn
```

### Running the Project

1. **Run the full analysis notebook** (Jupyter Notebook or Python script):
   ```bash
   python iris_analysis.py
   ```

2. **Interactive prediction from terminal**:
   ```bash
   python predict_species.py
   ```

---

## 🎯 Model Accuracy Comparison

| Model               | Accuracy      |
|--------------------|---------------|
| Logistic Regression| **1.00**      |
| SVM                | **1.00**      |
| KNN                | **1.00**      |
| Naive Bayes        | 0.978         |
| Decision Tree      | 1.00          |
| Random Forest      | 1.00          |

**Best Model**: Logistic Regression (based on overall performance)

---

## 🧪 Hyperparameter Tuning Results

| Model              | Best Params                                    | Accuracy |
|-------------------|------------------------------------------------|----------|
| KNN               | `n_neighbors=3`, `metric='euclidean'`          | 1.00     |
| Logistic Regression | `C=100`, `solver='saga'`                     | 1.00     |
| SVM               | `C=10`, `kernel='linear'`, `gamma='scale'`     | 0.978    |
| Random Forest     | `n_estimators=100`, `max_depth=10`             | 1.00     |

---

## 📈 Cross-Validation Scores (5-Fold)

| Model              | CV Accuracy |
|-------------------|-------------|
| KNN               | 0.943       |
| Logistic Regression| 0.886       |
| SVM               | 0.943       |
| Random Forest     | 0.943       |

---

## 🤖 Predict Flower Species (CLI)

```bash
$ python predict_species.py
Enter sepal length (cm): 3
Enter sepal width (cm): 6
Enter petal length (cm): 3
Enter petal width (cm): 9
The predicted flower species is: virginica
```

---

## 📌 Dataset Source

- [UCI Machine Learning Repository - Iris Dataset](https://archive.ics.uci.edu/ml/datasets/iris)

---

## 📜 License

This project is open-source and available under the MIT License.


