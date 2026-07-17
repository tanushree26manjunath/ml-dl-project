# 📌 Legal Clause-Level Summarization using Deep Learning

## 🧠 Overview

This project focuses on automatically generating concise and legally accurate summaries from lengthy legal documents using Deep Learning techniques. Legal contracts, bills, and statutory documents are often difficult and time-consuming to analyze manually due to their complex language and structure.

The proposed system employs a **Hybrid Sequence-to-Sequence (Seq2Seq) architecture** based on **Gated Recurrent Units (GRU)**, enhanced with an **Attention Mechanism**, **Pointer-Generator Network (PGN)**, and **Coverage Mechanism**. These components enable the model to generate fluent summaries while preserving important legal terminology and minimizing repetition.

---

## 📊 Dataset

* **Dataset:** BillSum Dataset
* Contains U.S. Congressional and California legislative bills paired with expert-written summaries.
* Approximately:

  * **8,000** samples for training
  * **500** samples for evaluation

---

## ⚙️ Methodology

### 🔹 Data Preprocessing

* Text cleaning and normalization
* Lowercase conversion
* Tokenization
* Vocabulary construction
* Padding and sequence encoding
* Input-output sequence preparation

---

### 🔹 Model Architecture

The proposed model consists of:

* Bidirectional **GRU Encoder**
* Attention-based GRU Decoder
* Pointer-Generator Network (PGN)
* Coverage Mechanism
* Beam Search Decoder

The Pointer-Generator Network enables the model to either:

* Generate new words from the vocabulary
* Copy important legal terms directly from the source document

The Coverage Mechanism reduces repetitive phrases during summary generation.

---

### 🔹 Training

* PyTorch implementation
* AdamW Optimizer
* Label Smoothing
* Gradient Clipping
* Scheduled Teacher Forcing
* Coverage-aware Loss
* GPU/CPU compatible training

---

## 📈 Evaluation Metrics

The model was evaluated using:

* **ROUGE-1**
* **ROUGE-2**
* **ROUGE-L**
* **BLEU**
* **METEOR**

These metrics evaluate lexical overlap, semantic similarity, and overall summary quality.

---

## 🚀 Results

| Metric  | Score      |
| ------- | ---------- |
| ROUGE-1 | **0.5040** |
| ROUGE-2 | **0.2851** |
| ROUGE-L | **0.3630** |
| BLEU    | **0.1756** |
| METEOR  | **0.3274** |

The proposed hybrid model effectively preserves important legal information while generating concise, coherent, and factually consistent summaries.

---

## 🛠️ Tech Stack

* Python
* PyTorch
* NumPy
* Pandas
* Matplotlib
* Hugging Face Tokenizers
* Scikit-learn

---

## 📂 Project Structure

```text
legal-clause-summarization/
│── mldl.ipynb          # Main notebook
│── README.md           # Project documentation
│── requirements.txt    # Required packages
```

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone <repository-url>
```

2. Install the required Python libraries:

```bash
pip install torch transformers pandas numpy matplotlib scikit-learn nltk rouge-score sacrebleu
```

3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Open `mldl.ipynb` and run all cells sequentially.

## ✨ Key Features

* Hybrid GRU-based Seq2Seq architecture
* Attention Mechanism
* Pointer-Generator Network
* Coverage Mechanism
* Beam Search Decoding
* Automatic Legal Clause Summarization
* Multiple evaluation metrics
* GPU-compatible implementation

---

## 🔮 Future Improvements

* Fine-tune Transformer-based models such as **T5**, **BART**, and **Longformer**
* Train on larger legal datasets
* Improve factual consistency
* Build a web application for legal professionals
* Support multilingual legal summarization

---

## 📌 Conclusion

This project demonstrates the application of advanced Deep Learning techniques for legal document summarization. By combining GRU-based Seq2Seq learning with Attention, Pointer-Generator Networks, and Coverage Mechanisms, the model generates concise, coherent, and legally faithful summaries while reducing redundancy. The approach provides an efficient solution for legal document analysis and can serve as a foundation for future AI-assisted legal applications.

---

