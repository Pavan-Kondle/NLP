# Multi-Model Approach for Disease Detection Using Text Analysis

## 1. What is the research about?

- **Core Focus**: Applying **Natural Language Processing (NLP)** and **machine learning** on pharmaceutical reviews to detect early signs of diseases caused by medications.  
- **Healthcare Relevance**: Improves **personalized treatment recommendations** and preventive healthcare.  
- **Sentiment & Context Analysis**: Classifies reviews into **positive, negative, neutral** while considering context and nuances.  
- **Integration of Knowledge**: Incorporates external medical knowledge (side effects, drug interactions, conditions) to improve accuracy.  
- **Deployment Goal**: User-friendly system for **healthcare professionals and patients**, providing insights, visualizations, and alerts for early disease identification.  

---

## 2. Research Problem and Solution

### Problem
- Pharmaceutical reviews contain **technical jargon, subjective opinions, and nuanced sentiment**, making automated analysis difficult.  
- Existing sentiment analysis in healthcare struggles with **low accuracy, poor contextual awareness, and lack of medical knowledge integration**.  

### Solution
- **Sentiment Analysis Models**: Classify drug reviews (positive/negative/neutral).  
- **Disease Detection Models**: Deep learning (CNN, RNN, BiLSTM) to detect patterns between drugs, symptoms, and conditions.  
- **Feature Engineering & Embeddings**: Use n-grams, TF-IDF, and embeddings to capture semantic meaning.  
- **Medical Knowledge Integration**: Add data on side effects, drug interactions, and known conditions.  
- **Trust & Credibility Modeling**: Filter unreliable reviews by weighting reviewer reliability and consistency.  
- **End-to-End Pipeline**: Preprocessing → feature extraction → model training → evaluation → deployment.  

---

## 3. Contributions

- ✅ **Framework**: Supervised learning framework for **context-aware sentiment analysis** of drug reviews.  
- ✅ **Text Summarization**: Extracts short, usable insights from long reviews.  
- ✅ **Dependency Parsing & Clustering**: Improves accuracy by capturing long- and short-range text dependencies.  
- ✅ **Knowledge Integration**: Adds medical domain knowledge for reliable disease detection.  
- ✅ **Model Comparison**: Benchmarks Naive Bayes vs BiLSTM for text classification tasks.  
- ✅ **Practical Impact**: Designed for **healthcare professionals and patients** to improve treatment decision-making.  

---

## 4. Results

- 📊 **Metrics Used**: Accuracy, Precision, Recall, F1-score, ROC-AUC.  
- 🚀 **Improved Accuracy**: Embeddings + medical knowledge integration improved disease detection vs baselines.  
- 🧠 **Best Performing Model**: BiLSTM outperformed Naive Bayes in contextual sentiment/disease detection.  
- ⚡ **Scalability & Usability**: Efficient for large datasets, ready for real-world healthcare use.  
- 💻 **Deployment**: Integrated into a **user-friendly interface** with alerts, summaries, and actionable insights.  

---

## 5. Comprehensive Error Analysis Report

### Overview
This report provides a detailed analysis of the performance of **LSTM**, **CNN**, and **BiLSTM** models for the classification task. Models were evaluated using **accuracy, precision, recall, F1-score, and confusion matrices** to identify strengths, weaknesses, and areas for improvement.

---

### LSTM Model
- **Accuracy**: ~93.32%  
- **Precision**: 0.83 – 0.99 (high precision in most classes)  
- **Recall**: 0.77 – 0.98 (variation across classes)  
- **F1-score**: 0.80 – 0.99 (balanced performance)  
- **Confusion Matrix**:  
  - Misclassifications concentrated in **classes 1, 5, and 11**  
  - Class 1 (P=0.83, R=0.77) and Class 5 (P=0.85, R=0.88) showed weaker performance  

---

### CNN Model
- **Accuracy**: ~93.52%  
- **Precision**: 0.84 – 0.99  
- **Recall**: 0.81 – 0.96  
- **F1-score**: 0.83 – 0.99  
- **Confusion Matrix**:  
  - Errors mostly between **classes 1, 5, and 11**  
  - Class 1 (P=0.84, R=0.81) and Class 5 (P=0.86, R=0.89) weaker  

---

### BiLSTM Model
- **Accuracy**: ~93.35%  
- **Precision**: 0.82 – 0.99  
- **Recall**: 0.81 – 0.94  
- **F1-score**: 0.81 – 0.99  
- **Confusion Matrix**:  
  - Similar error patterns in **classes 1, 5, and 11**  
  - Class 1 (P=0.82, R=0.81) and Class 5 (P=0.85, R=0.87) weaker  

---

### General Observations
- 🔁 **Consistent Errors**: All models misclassify between classes 1, 5, and 11 → indicates intrinsic overlap in features.  
- ⚖️ **Performance Discrepancies**: While overall accuracy is high (>93%), some classes consistently underperform.  
- 🧩 **Model Consistency**: Different architectures (LSTM, CNN, BiLSTM) exhibit similar weaknesses, suggesting **class-level difficulty** rather than model-specific flaws.  

---

### Conclusion
- All three models (**LSTM, CNN, BiLSTM**) show **high accuracy (93%+)** with strong precision, recall, and F1-scores.  
- Common **misclassification patterns** highlight areas for targeted dataset refinement or hybrid modeling.  
- Future work should focus on **enhancing robustness** and **reducing overlap between challenging classes** (1, 5, 11).  

---



