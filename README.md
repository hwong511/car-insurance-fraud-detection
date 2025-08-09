# Car Insurance Fraud Detection – Image Classification

## Overview
This project investigates the use of **image-based machine learning models** to detect potential car insurance fraud from damage photographs. The dataset is highly imbalanced, with far fewer fraudulent cases than non-fraudulent ones, making imbalance handling a key challenge.

Two approaches were compared:
1. **Off-the-shelf model** – Based on [ViT Base Patch16-224](https://huggingface.co/google/vit-base-patch16-224) from Hugging Face, using **class weights** to address class imbalance.
2. **Custom-built model** – Designed from scratch in R, using **both class weights and image augmentation** to mitigate imbalance and improve generalization.

This comparison highlights the impact of different imbalance-handling strategies on model performance.

---

## Project Motivation
Insurance fraud costs billions annually, with image evidence often central to investigations. Automating fraud detection can:
- Reduce manual review workload
- Speed up claim processing
- Limit fraudulent payouts
- Support ethical and consistent decision-making

---

## Dataset
Source: [Car Insurance Fraud Detection (Kaggle)](https://www.kaggle.com/datasets/pacificrm/car-insurance-fraud-detection)  

Contents:
- Images of car damage claims
- Labels: `Fraud` or `Non-fraud`
- Separate train and test splits
- Extreme class imbalance, making it a challenging and realistic fraud detection task

---

## Applications
- Automated claim screening for insurance companies
- Research into imaged-based fraud prevention and anomaly detection
- Educational projects in computer vision and AI ethics

---

## Models
- **Off-the-shelf Model (ViT)** – Pretrained Vision Transformer, fine-tuned with class weights for imbalance handling
- **Custom Model** – CNN built in Python, trained with class weights and image augmentation for more robust learning

---

## 📊 Results
| Model                  | Accuracy | Precision | Recall | F1-Score | AUC-ROC |
|------------------------|----------|-----------|--------|----------|---------|
| ViT (Class Weights)    | 98.16%   | 0.9589    | 0.7527 | 0.8434   | 0.9693  |
| Custom CNN (CW + Aug)  | XX.XX%   | 0.XXXX    | 0.XXXX | 0.XXXX   | 0.XXXX  |

---

## Responsible AI Use
- Models are **decision support tools**, not automated claim verdict systems
- Misclassifications could lead to wrongful claim denials or approvals
- Dataset biases should be addressed to avoid unfair treatment across demographics

---

## Potential Future Work
- Use hybrid models combining images with textual claim descriptions
- Explore additional imbalance techniques (SMOTE for images, focal loss)
- Apply explainable AI methods to make fraud decisions interpretable
- Evaluate models in production-like insurance claim workflows

---

## License
This project is for **research and educational purposes** only.  
Refer to the dataset’s [Kaggle license](https://www.kaggle.com/datasets/pacificrm/car-insurance-fraud-detection) before use.

---

## ✏️ Authors
- [Andy Vo]
- [Dusk Zhang]
- [Ho Wong]
