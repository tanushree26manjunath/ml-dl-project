# 📌 Legal Clause Summarization using Machine Learning & Deep Learning

## 🧠 Overview

This project focuses on automatically summarizing complex legal clauses into concise and meaningful text using Machine Learning and Deep Learning techniques.

The system leverages transformer-based models such as **T5 (Text-to-Text Transfer Transformer)** along with sequence-to-sequence architectures to generate high-quality summaries.

---

## 📊 Dataset

* Dataset used: **BillSum Dataset (Legal/Text Summarization)**
* Contains legal documents and their corresponding summaries
* Used for training and evaluation of the model

---

## ⚙️ Approach

### 🔹 Data Preprocessing

* Text cleaning and normalization
* Tokenization using Hugging Face tokenizer
* Input-output sequence preparation

### 🔹 Models Used

* **T5-small (Transformer-based Seq2Seq model)**
* Custom **Seq2Seq architecture (PyTorch-based)**

### 🔹 Training

* Fine-tuning of pre-trained transformer model
* Batch processing using DataLoader
* GPU/CPU compatible training

---

## 📈 Evaluation Metrics

The model performance is evaluated using:

* **ROUGE Score** (for summarization quality)
* **BERTScore** (semantic similarity)
* **SacreBLEU** (text generation evaluation)

---

## 🚀 Results

* Efficient summarization of legal clauses
* Generates concise and meaningful summaries
* Supports real-world legal text processing use cases

*(You can add your actual scores here if available)*

---

## 🛠️ Tech Stack

* Python
* PyTorch
* Hugging Face Transformers
* NumPy, Pandas
* Matplotlib, Seaborn

---

## ▶️ How to Run

1. Clone the repository from GitHub
2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Open the notebook:

```bash
jupyter notebook
```

4. Run all cells step by step

---

## 📁 Project Structure

```
legal-clause-summarization/
│── mldl(1).ipynb   # Main notebook
│── README.md       # Project documentation
```

---

## 📌 Key Features

* Transformer-based summarization (T5)
* Custom Seq2Seq implementation
* Multiple evaluation metrics
* Visualization of training performance

---

## 🔮 Future Improvements

* Use larger transformer models (T5-large, BART)
* Deploy as a web application
* Improve accuracy with more legal datasets

---

## 📌 Conclusion

This project demonstrates how deep learning models can be applied to automate the summarization of complex legal documents, improving readability and saving time in legal analysis.

---
