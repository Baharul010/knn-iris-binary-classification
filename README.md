# 🌸 KNN Iris Binary Classification with Confusion Matrix GUI

This project implements a **K-Nearest Neighbors (KNN)** model to classify Iris flowers into binary categories. The dataset is loaded directly from an online source and converted into a binary classification problem.

The model performance is evaluated using a **2×2 confusion matrix**, and results are visualized using a **heatmap GUI** built with Matplotlib and Seaborn.

---

## 🚀 Features

* 📥 Load dataset directly from online source
* 🔄 Convert multi-class dataset into binary classification
* 🤖 Train model using K-Nearest Neighbors (KNN)
* 📊 Evaluate model with:

  * Accuracy score
  * Confusion matrix (2×2)
  * Classification report
* 🎨 Visualize confusion matrix using heatmap

---

## 📂 Dataset

* Dataset: Iris Dataset
* Source: GitHub (online CSV)

### Features:

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

### Target Conversion:

* **1 → Iris-setosa**
* **0 → Not Iris-setosa**

---

## 🧠 Algorithm Used

* K-Nearest Neighbors

---

## ⚙️ Installation

Install required libraries:

```bash id="knn1"
pip install pandas numpy scikit-learn matplotlib seaborn
```

---

## ▶️ How to Run

1. Clone the repository:

```bash id="knn2"
git clone https://github.com/your-username/knn-iris-binary-classification.git
cd knn-iris-binary-classification
```

2. Run the Python script:

```bash id="knn3"
python main.py
```

---

## ⚙️ Model Configuration

* Algorithm: K-Nearest Neighbors
* Default k value: **5**
* Distance metric: Euclidean (default)

👉 You can modify:

```python id="knn4"
k = 3  # or 7, 9, etc.
```

---

## 📊 Output

### Console Output:

* Accuracy score
* Confusion matrix (2×2)
* Classification report

### GUI Output:

* Heatmap showing confusion matrix
* Labeled axes (Actual vs Predicted)

---

## 📌 Confusion Matrix Structure

```id="knn5"
        Predicted
         0   1
Actual  --------
   0   | TN  FP
   1   | FN  TP
```

---

## 🎨 Visualization

* Heatmap created using Seaborn
* Blue gradient color scheme
* Helps visually analyze model performance

---

## ⚠️ Important Tip

KNN performs better when features are scaled. You can improve accuracy by adding:

```python id="knn6"
from sklearn.preprocessing import StandardScaler

scaler = StandardScaler()
X_train = scaler.fit_transform(X_train)
X_test = scaler.transform(X_test)
```

---

## 🔮 Future Improvements

* Compare KNN with Naive Bayes
* Tune optimal k value using cross-validation
* Build Streamlit web app
* Add real-time prediction input

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork and submit pull requests.

---

## 📜 License

This project is open-source under the MIT License.

---

## 👨‍💻 Author

Your Name
GitHub: https://github.com/your-username
