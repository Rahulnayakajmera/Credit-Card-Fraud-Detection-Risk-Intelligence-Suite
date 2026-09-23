# Credit Card Fraud Detection & Risk Intelligence Suite
**AICTE | IBM SkillsBuild Data Analytics with AI Academic Internship 2026 | BharatCares**

## 📌 Project Overview
The **Credit Card Fraud Detection & Risk Intelligence Suite** is an enterprise-grade analytics and machine learning solution designed to identify unauthorized payment transactions in real time while minimizing false customer denials [cite: 2]. Developed for the **IBM SkillsBuild Data Analytics with AI Academic Internship** by **Ajmera Rahul chatursingh Nayak** from **Visvesvaraya College of Engineering and Technology**, this system combines SQL velocity profiling, RobustScaler normalization, SMOTE balancing, a tuned XGBoost classification pipeline, and an interactive **Streamlit Web Application (`app.py`)** alongside Power BI executive dashboards [cite: 2].

---

## 👨‍🎓 Intern & Academic Information
* **Intern Full Name:** Ajmera Rahul chatursingh Nayak [cite: 2]
* **College / Institution:** Visvesvaraya College of Engineering and Technology, Ibrahimpatnam [cite: 2]
* **Department / Specialization:** Computer Science & Engineering / Data Analytics [cite: 2]
* **Internship Program:** AICTE | IBM SkillsBuild Data Analytics with AI Academic Internship 2026 (BharatCares) [cite: 2]
* **Registered Email:** ajmerarahul112@gmail.com [cite: 2]

---

## 📊 Dataset Architecture
* **Dataset Name:** Credit Card Fraud Detection (`creditcard.csv`) [cite: 2]
* **Dataset Source:** [Kaggle Credit Card Fraud Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) [cite: 2]
* **Record Count:** 284,807 transactions across 31 continuous numerical columns [cite: 2]
* **Target Distribution:** Legitimate: 284,315 (99.828%) | Fraudulent: 492 (0.172%) [cite: 2]
* **Imbalance Treatment:** Stratified 80/20 partitioning with SMOTE (10% ratio) applied strictly on the training partition [cite: 2].

---

## 🛠️ Technology Stack
* **Web App Frontend:** Streamlit (`app.py`)
* **Machine Learning & Analytics:** Python 3.11, Scikit-Learn, Imbalanced-Learn (SMOTE), XGBoost, Pandas, NumPy [cite: 2]
* **Query Layer:** PostgreSQL / SQL Window Functions (Velocity bursts, lag calculations) [cite: 2]
* **Business Intelligence:** Power BI Desktop (IBM Carbon Dark Glassmorphism, 5-Level Hierarchy) [cite: 2]
* **Development Environments:** VS Code, Jupyter Notebook (`.ipynb`) [cite: 2]

---

## 🚀 Installation & Execution Guide

### 1. Clone Repository & Setup
```bash
git clone https://github.com/ajmerarahul112/credit-card-fraud-detection-ibm.git
cd credit-card-fraud-detection-ibm
```

### 2. Create and Activate Virtual Environment
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Linux / macOS
python -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the Streamlit Web Application
To launch the interactive fraud screening web app, run:
```bash
streamlit run app.py
```
*The app will automatically open in your browser at `http://localhost:8501`.*

### 5. Run the Jupyter Notebook Pipeline
```bash
jupyter notebook Ajmera_Rahul_CreditCardFraudDetection.ipynb
```

---

## 📈 Model Performance & Benchmarking

| Algorithm Evaluated | Accuracy | Precision | Recall | PR-AUC | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Logistic Regression** | 99.88% | 82.43% | 62.24% | 0.7312 | Baseline [cite: 2] |
| **Decision Tree (depth=8)** | 99.82% | 74.11% | 76.53% | 0.7584 | Moderate [cite: 2] |
| **Random Forest (200 trees)** | 99.95% | 94.18% | 82.65% | 0.8710 | Near-Production [cite: 2] |
| **Tuned XGBoost (Champion)** | **99.96%** | **94.44%** | **87.21%** | **0.8924** | **🏆 Champion Selected** [cite: 2] |

* **Preserved Capital:** €108,520 intercepted on test holdout with False Positive Rate < 0.05% [cite: 2].
* **Inference Speed:** 1.42 ms per transaction (payment gateway SLA compliant) [cite: 2].

---

## 🏛️ IBM 5-Level Metric Hierarchy (BI Dashboard)
1. **Level 1 (Executive KPIs):** Total Monitored Capital (€28.4M), Losses Prevented (€108.5K), Precision (94.44%) [cite: 2].
2. **Level 2 (Temporal Trends):** Nocturnal fraud surge identified between 01:00 AM – 04:00 AM [cite: 2].
3. **Level 3 (Operational Drivers):** Fraud probability 4x higher in the €500 – €2,000 transaction tier [cite: 2].
4. **Level 4 (Risk Intelligence):** 3-Tier Rule Matrix (`>0.70` Auto-Decline, `0.35–0.70` Step-Up 2FA, `<0.35` Seamless) [cite: 2].
5. **Level 5 (Strategic Actions):** Dynamic nocturnal thresholds projecting €1.2M in annual loss prevention [cite: 2].
