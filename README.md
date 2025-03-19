# SMS & Email Phishing Detection

## 📌 Project Overview
This project aims to detect phishing attempts in SMS and email messages using **Natural Language Processing (NLP)** and **Machine Learning (ML)**. It leverages **TF-IDF vectorization** for text representation and trains a **Random Forest Classifier** to classify messages as spam (phishing) or ham (legitimate). The model achieves **97% accuracy**, making it highly effective for real-world phishing detection.

## 🗂️ Dataset
The dataset comprises SMS and email messages labeled as **spam (phishing)** or **ham (legitimate)**. The data is preprocessed to remove noise, including:
- **Removing special characters & stopwords**
- **Tokenization & Lemmatization**
- **Converting text into numerical features using TF-IDF**

## 🏗️ Model Architecture
- **Feature Extraction:** TF-IDF vectorization
- **Classifier:** Random Forest Classifier
- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-Score

## 🔧 Installation & Setup
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/SMS-Phishing-Detection.git
cd SMS-Phishing-Detection
```

### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Model
```bash
python train.py
```

## 🎯 Training Process
1. **Data Preprocessing:**
   - Lowercasing, removing stopwords, punctuation, and special characters
   - Tokenization and lemmatization
   - Converting text to numerical features using TF-IDF
2. **Model Training:**
   - Random Forest Classifier trained on TF-IDF features
   - Hyperparameter tuning to optimize performance
3. **Evaluation:**
   - Achieved **97% accuracy** with high precision and recall

## 🚀 Deployment
The trained model is saved using **Joblib** for real-time phishing detection.

### Run the Model for Prediction
```bash
python predict.py --text "Congratulations! You won a free iPhone. Click the link to claim."
```
**Output:** `Spam (Phishing)`

## 📌 Future Improvements
- Experimenting with **Deep Learning models (LSTMs, Transformers)** for better accuracy
- Expanding dataset with real-world phishing emails
- Deploying as a **REST API using Flask or FastAPI**

---
**📩 Contact:** If you have any questions, feel free to reach out or contribute to the project!

