Assignment 8 — Evaluating Fine-Tuned LLM Performance
**Name:** Asma Begum
**Course:** AD331
**Model:** BERT-base-uncased (Fine-Tuned)
**Task:** Sentiment Classification (Negative / Neutral / Positive)
Overview
This repository contains the full evaluation of a fine-tuned Large Language Model (LLM) trained for a supervised sentiment-classification task. The evaluation includes metric computation, confusion matrix visualization, worst-class identification, and misclassification analysis.
Repository Structure
.
├── evaluation_notebook.ipynb
├── confusion_matrix_normalized.png
└── README.md
Evaluation Metrics
Metric	Value
Accuracy	0.88
Precision (Macro)	0.87
Recall (Macro)	0.86
F1-Score (Macro)	0.86
Why Macro-F1?
Macro-F1 is preferred over Accuracy because it treats all classes equally, regardless of class imbalance. Accuracy can remain high even when minority classes perform poorly. Macro-F1 evaluates precision and recall independently for each class and averages them fairly, providing a more balanced representation of performance.
Confusion Matrix
A normalized confusion matrix was generated and saved as 'confusion_matrix_normalized.png'. Rows represent true labels, while columns represent predicted labels. Diagonal values indicate correct predictions, and off-diagonal values represent misclassifications.
Error Analysis
**Worst-Performing Class:** Negative
**F1-Score:** 0.79

**Misclassified Example 1:**
Text: "The update didn’t fix anything, but whatever I guess it’s fine."
Reason: Subtle negativity disguised with neutral phrasing, making the sentiment difficult to detect.
**Misclassified Example 2:**
Text: "Great, another feature that breaks everything… wonderful."
Reason: Sarcasm. The presence of positive keywords misleads the model into predicting a positive label.
Video Demonstration
The accompanying video presentation includes:
- An explanation of all evaluation metrics (Accuracy, Precision, Recall, F1)
- A walkthrough of the normalized confusion matrix and its interpretation
- Identification and discussion of the worst-performing class
- Analysis of two misclassified examples, including likely technical reasons for each
- A justification for using Macro-F1 as the primary evaluation metric
- A screen-and-webcam view, with clear audio, within the required 5–7 minute duration
Conclusion
This document provides the full evaluation write-up for Assignment 8, including the model’s metrics, confusion matrix interpretation, and error analysis. The results offer insight into the performance and limitations of the fine-tuned LLM.

