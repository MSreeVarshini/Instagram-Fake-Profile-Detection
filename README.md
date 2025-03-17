# 🚀 **Instagram Fake Profile Detection using Machine Learning**  

A **machine learning-driven approach** to detect fake Instagram profiles using **XGBoost** and **data analysis techniques**. This project employs **feature engineering, exploratory data analysis (EDA), model training, and evaluation** to build a high-performing classifier for distinguishing between real and fake accounts.  

---

## 📌 **Project Overview**  

Social media platforms like Instagram are flooded with **fake profiles**, often used for spam, scams, and misinformation. This project leverages **data-driven techniques** to analyze Instagram account characteristics and build a **predictive model** to classify profiles as **real or fake**.  

### ✨ **Key Highlights**  

✔ **Dataset Exploration & Cleaning** – Handling missing values, renaming columns, and preparing data.  
✔ **Feature Analysis & Visualization** – Distributions, correlations, and fake-vs-real comparisons.  
✔ **Machine Learning Model** – **XGBoost classifier** for high-accuracy detection.  
✔ **Evaluation Metrics** – Accuracy, Precision, Recall, F1-score, ROC-AUC, Log Loss, MCC.  
✔ **Model Reliability Check** – **Calibration Curve & Confusion Matrix** for performance validation.  

---

## 🔧 **Installation & Setup**  

### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/msreevarshini/Fake-Instagram-Profile-Detection.git
cd Fake-Instagram-Profile-Detection
```

### 2️⃣ Install Dependencies  
```bash
pip install -r requirements.txt
```

### 3️⃣ Run Jupyter Notebook  
```bash
jupyter notebook
```

---

## 📊 **Data Analysis & Key Insights**  

### **📌 Feature Exploration**  
We analyze key attributes of Instagram accounts using **histograms, KDE plots, and boxplots**.  

🔹 **Username & Name Patterns:** Fake accounts often have **more numerical characters** in usernames.  
🔹 **Profile Picture Usage:** Many fake profiles lack a profile picture.  
🔹 **Follower-Following Ratio:** Fake accounts have **low follower count** but follow many profiles.  
🔹 **Engagement Metrics:** Fake profiles tend to have **fewer posts** and shorter bio descriptions.  

### **📌 Correlation Analysis**  
The **correlation heatmap** reveals relationships between features:  
✔ **Fake accounts tend to have higher numbers in usernames.**  
✔ **Lower post counts are correlated with fake profiles.**  

### **📌 Real vs. Fake Profile Comparisons**  
Using **violin plots and bar charts**, we compare feature distributions for **real vs. fake** accounts:  
✔ Fake accounts often have **higher numerical density** in usernames.  
✔ Many fake profiles **lack external links** or have **short descriptions**.  

---

## 🚀 **Machine Learning Model**  

We use **XGBoost**, a powerful gradient boosting algorithm, to classify Instagram accounts.  

✅ **Hyperparameters Used:**  
- **n_estimators:** 200  
- **learning_rate:** 0.1  
- **eval_metric:** logloss  
- **random_state:** 42  

✅ **Training Process:**  
- **Train-Test Split:** 80% training, 20% testing  
- **XGBoost Model Fitting**  

✅ **Predictions:**  
- We generate **class predictions** and **probabilities** for fake account detection.  

---

## 📊 **Model Evaluation**  

### **📌 Performance Metrics**  
✔ **Accuracy:** Measures overall correctness.  
✔ **Precision:** How many predicted fake accounts are actually fake?  
✔ **Recall:** How many actual fake accounts were correctly identified?  
✔ **F1-Score:** Balance between Precision & Recall.  
✔ **ROC-AUC Score:** Measures the model’s ability to distinguish between real & fake profiles.  
✔ **Log Loss:** Measures prediction uncertainty.  
✔ **MCC (Matthews Correlation Coefficient):** Evaluates model quality.  

📌 **Best Performing Model Achieved:**  
- **Accuracy:** **99%**  
- **F1-Score:** **0.99**  
- **ROC-AUC Score:** **0.99**  

### **📌 Confusion Matrix**  
The **heatmap visualization** of the **Confusion Matrix** helps identify misclassifications.  

✔ **High True Positives & True Negatives** → Strong classification performance.  
✔ **Minimal False Positives & False Negatives** → Model reliability.  

### **📌 Model Calibration Curve**  
- Evaluates how well the predicted probabilities align with actual probabilities.  
- The closer the curve follows the **diagonal reference line**, the more reliable the model is.  

---

## 📜 **License**  

This project is licensed under the **MIT License** – feel free to use and modify it for research and educational purposes.  

---

## 🤝 **Contributions & Support**  

💡 **Contributions are welcome!**  
If you want to improve the model, fix issues, or add new features, feel free to submit a **pull request**.  

📩 **For any questions, contact:** msreevarshini@ieee.org  

📌 **Give this project a ⭐ if you found it useful!** 🚀
