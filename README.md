Alzheimer's Disease Detection Using Brain MRI
> Multi-class MRI classification achieving **97%+ accuracy** across 4 severity stages using fine-tuned EfficientNetB3.
Overview
Deep learning pipeline to classify Alzheimer's progression from brain MRI scans into 4 stages: Non-Demented, Very Mild, Mild, and Moderate Demented — using the OASIS dataset (80,000+ slices).
Results
Metric	Score
Test Accuracy	97%+
Evaluation	Confusion Matrix, ROC-AUC, F1-Score
Interpretability	Grad-CAM activation maps
Tech Stack
Framework: TensorFlow / Keras
Model: EfficientNetB3 (fine-tuned, transfer learning)
Preprocessing: LGG MRI segmentation, data augmentation
Visualization: Grad-CAM, Matplotlib, Seaborn
Key Features
Transfer learning with custom dense head + dropout regularization
LGG segmentation preprocessing to isolate brain ROIs
Grad-CAM maps to validate clinically relevant attention regions
Full evaluation suite: confusion matrix, ROC-AUC curves, F1-score per class
Dataset
OASIS Brain MRI Dataset — 80,000+ MRI slices across 4 Alzheimer's severity classes.
Setup
```bash
git clone https://github.com/harshit-kewalramani/alzheimers-mri-detection
cd alzheimers-mri-detection
pip install -r requirements.txt
jupyter notebook alzheimers_detection.ipynb
```
