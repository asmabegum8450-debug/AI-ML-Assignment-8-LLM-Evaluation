# Assignment 8 — Evaluating Fine-Tuned LLM Performance

**Name:** [YOUR NAME]  
**Course:** [COURSE NAME]  
**Model:** [Your Fine-Tuned Model Name]  
**Task:** [Sentiment / Topic Classification]

---

## 📌 Overview
This repository contains the complete evaluation of a fine‑tuned Large Language Model (LLM) for a supervised text‑classification task.  
The evaluation includes metric computation, confusion matrix generation, and detailed error analysis.

---

## 📂 Repository Structure
```
.
├── evaluation_notebook.ipynb
├── confusion_matrix_normalized.png
└── README.md
```

---

## 📊 Evaluation Metrics
The following metrics are computed using the held‑out test set:

| Metric | Value |
|--------|--------|
| Accuracy | [FILL] |
| Precision (Macro) | [FILL] |
| Recall (Macro) | [FILL] |
| F1-Score (Macro) | [FILL] |

---

## ⭐ Why Macro-F1?
Macro‑F1 is preferred over Accuracy because it treats each class equally, making it more reliable in imbalanced datasets.  
Accuracy can remain high even when minority classes are misclassified.  
Macro‑F1 evaluates both precision and recall per class and averages them fairly.

---

## 📉 Confusion Matrix
A normalized confusion matrix is generated to visualize classification patterns.  
Rows represent **true** labels; columns represent **predicted** labels.

The matrix is saved as:
```
confusion_matrix_normalized.png
```

---

## 🔍 Error Analysis
The notebook identifies and displays:

- The **worst‑performing class** (lowest F1)
- Two misclassified samples from that class
- A technical explanation for why the model failed on each example

---

## 🎥 Video Demonstration
Your recorded video should include:
- Metric explanation (Accuracy, Precision, Recall, F1)
- Confusion matrix interpretation
- Worst‑class analysis
- Demonstration of misclassified samples
- Justification for using Macro‑F1

---

## ✅ Conclusion
This repository provides a complete evaluation pipeline for analyzing LLM classification performance.
