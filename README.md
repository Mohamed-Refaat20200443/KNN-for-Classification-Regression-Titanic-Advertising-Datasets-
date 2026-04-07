# KNN-for-Classification-Regression-Titanic-Advertising-Datasets-
# K-Nearest Neighbors (KNN) - Classification & Regression Project

## 📌 Overview

This project demonstrates the implementation of the **K-Nearest Neighbors (KNN)** algorithm for both **classification** and **regression** tasks. The goal is to understand how distance-based models work and how the same algorithm can be applied to different types of machine learning problems.

The project includes:

* Classification using the **Titanic Dataset**
* Regression using the **Advertising Dataset**

---

## 🧠 Concept

Machine Learning models can be categorized based on how they learn patterns:

* **Linear Models** → تعتمد على المعادلات الخطية (Linear Equations)
* **Distance-Based Models** → تعتمد على المسافات (زي KNN)
* **Tree-Based Models** → زي Decision Trees و Random Forest
* **Probabilistic Models** → زي Naive Bayes

الـ **KNN** هو Distance-Based Algorithm، يعني بيقارن بين البيانات عن طريق حساب المسافات بين النقاط.

---

## 📏 Distance Metrics

اختيار طريقة حساب المسافة بيأثر بشكل كبير على أداء الموديل.

### 1. Euclidean Distance

* المسافة التقليدية (Straight Line)
* مناسبة للـ Low Dimensions

### 2. Manhattan Distance

* مجموع الفروق المطلقة بين القيم
* أفضل في حالة **High Dimensional Data**
* بيقلل تأثير مشكلة **Curse of Dimensionality**

---

## ⚙️ How KNN Works

### 🔹 Classification

1. نحسب المسافة بين الـ Test Point وكل نقاط الـ Training Data
2. نختار أقرب K نقاط (مثلاً K = 5)
3. نعمل **Majority Voting**
4. الكلاس الأكثر تكرارًا هو الناتج النهائي

### 🔹 Regression

1. نحسب المسافة بين النقطة وكل البيانات
2. نختار أقرب K نقاط
3. نحسب **متوسط القيم (Average)**
4. الناتج هو الـ Prediction

---

## 📊 Datasets Used

### 1. Titanic Dataset (Classification)

* الهدف: التنبؤ إذا كان الشخص نجا أم لا
* نوع المشكلة: Classification

### 2. Advertising Dataset (Regression)

* الهدف: التنبؤ بالمبيعات بناءً على الإعلانات
* نوع المشكلة: Regression

---

## 🔧 Hyperparameters

### 🔹 Number of Neighbors (K)

* عدد النقاط المستخدمة في اتخاذ القرار

### 🔹 Weights

* **Uniform** → كل النقاط لها نفس التأثير
* **Distance** → النقاط الأقرب لها تأثير أكبر

---

## ✅ Advantages

* لا يحتاج إلى Training Phase (Lazy Learning)
* سهل الفهم والتطبيق
* فعال مع العلاقات Non-Linear
* متعدد الاستخدامات (Classification, Regression, Imputation)

---

## ❌ Disadvantages

* High Computational Cost مع البيانات الكبيرة
* حساس للـ Noise
* غير مرن مع Outliers
* الأداء بيضعف مع زيادة عدد الـ Features

---

## ⚠️ Important Notes

* لازم نعمل **Feature Scaling** (زي StandardScaler أو RobustScaler)
  لأن KNN بيعتمد على المسافات
* اختيار K المناسب مهم جدًا
* اختيار Distance Metric بيأثر على النتائج

---

## 🚀 Conclusion

KNN من أبسط Algorithms في Machine Learning، لكنه قوي جدًا عند استخدامه بشكل صحيح. مناسب للـ Small to Medium datasets، وبيعتمد بشكل أساسي على جودة البيانات وطرق الـ Preprocessing.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib / Seaborn

---

## 📂 Project Structure

```
KNN-Project/
│
├── data/
│   ├── titanic.csv
│   └── advertising.csv
│
├── notebooks/
│   └── knn_analysis.ipynb
│
├── src/
│   └── knn_model.py
│
└── README.md
```

---

## 👨‍💻 Author

Mohamed Refaat
Computer Engineering Graduate - Cairo University
Interested in Machine Learning & Backend Development

