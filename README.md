# 🧴 Body Wash Review Analysis Project  

## 🧠 Brief Description  

This project focuses on analyzing customer reviews for body wash products. It involves processing review data, performing predictive modeling to identify key factors influencing customer satisfaction, and generating insights from the analysis.  

The core task is to predict *Level-1 factors* such as **Fragrance**, **Brand Value**, **Efficacy**, and **Skin Care** from review text using **Natural Language Processing (NLP)** techniques.  

The analysis is conducted using Jupyter notebooks, with datasets for training and testing models. The final results include predicted factors for the test reviews, stored in CSV format.

---

## ⚙️ Process  

### 1️⃣ Data Collection and Preparation  
- **Datasets**:  
  - `datasets/bodywash-train.xlsx` → Training data containing reviews with labeled factors  
  - `datasets/bodywash-test.xlsx` → Unlabeled test data for generating predictions  
- Data preprocessing included text cleaning, handling missing values, and preparing structured input for inference.  

---

### 2️⃣ Model Development and Inference  

#### 💡 LLM Used → Groq Cloud **LLaMA 3.1 – 8B Instant**  
This project uses the **LLaMA 3.1 – 8B Instant** model from **Groq Cloud** for factor prediction.  
It was selected for its **speed, contextual understanding, and free-tier accessibility**.  

**Key Features of LLaMA 3.1 Instant:**  
- 🧩 Large Language Model trained by Meta AI and served on Groq’s ultra-low-latency hardware  
- ⚡ Extremely fast inference (< 1 s per prompt) — ideal for batch text classification  
- 🔁 Supports multi-label NLP tasks (identifying multiple factors from a review)  
- 🧠 Strong semantic reasoning for consumer feedback and sentiment classification  
- 💸 Completely free for moderate usage under Groq Cloud’s public tier  

**Notebook:**  
- `notebook/bodyWash.ipynb` → Contains EDA, model prompt design, Groq API integration, prediction loop (with rate-limit handling), and result generation.  

---

### 3️⃣ Prediction and Evaluation  
- Model queries each review text via the Groq Cloud API and returns a comma-separated list of factors.  
- Predictions are saved to `result/bodywash-test-final.csv`.  
- Evaluation metrics (accuracy, precision, recall) can be computed on the training data for internal validation.  

---

### 4️⃣ Results and Insights  

The final CSV file contains each review and its predicted factors, allowing for quick analysis of themes and sentiment.  

| Review Text | Predicted Factors |
|--------------|------------------|
| “Smells great and foams easily.” | Fragrance, Product Texture |
| “Too harsh on my skin.” | Product Safety, Skin Care |
| “Hard to find locally.” | Accessibility |
| “A bit pricey but amazing scent.” | Price, Fragrance |

---

## 📊 Data Analysis and Visualization  

Exploratory data analysis (EDA) in the notebook includes:  
- Factor frequency distribution  
- Word clouds of review terms  
- Charts showing review lengths and factor occurrences  

---

## 🔍 Key Insights from Reviews  

- **Fragrance** and **Efficacy** are the most common factors.  
- **Skin Care** and **Cleansing** often appear together in positive reviews.  
- **Price** and **Brand Value** influence customer perception strongly.  

---

## 🪄 Getting Started  

1. **Clone the repository**
   ```bash
   git clone https://github.com/Adarsh-Mishra15/MavenMagnet_round_1.git

## 🧩 Dependencies  

```text
Python 3.x  
pandas  
numpy  
matplotlib  
seaborn  
tqdm  
requests  
python-dotenv  
Access to Groq Cloud API (LLaMA 3.1 Instant Model)
