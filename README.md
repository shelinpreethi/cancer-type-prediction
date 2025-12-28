# 🧬 Cancer Type Prediction from Gene Expression Data

Machine Learning • Cancer Genomics • TCGA • Bioinformatics

> End-to-end bioinformatics project demonstrating how gene expression signatures can be used to accurately classify cancer types using machine learning.

# 🚀 Project Snapshot (TL;DR)
- **Problem**: Can gene expression profiles reliably predict cancer type?
- **Data**: TCGA Pan-Cancer RNA-Seq + clinical phenotype metadata
- **Approach**: Feature selection → class balancing → Random Forest classification
- **Outcome**: High-accuracy multi-class cancer prediction using transcriptomic data
- **Skills**: Bioinformatics, ML, data preprocessing, genomics, model evaluation

# 🧠 Why This Project Matters
Cancer diagnosis and research increasingly rely on molecular signatures rather than only histology.
This project demonstrates how high-dimensional RNA-Seq data can be transformed into a predictive model that captures biologically meaningful cancer-type patterns.


# 🧪 Dataset
**Source**: TCGA Pan-Cancer Atlas
|Data|Type Description|
|---|---|
|Gene Expression|Normalized RNA-Seq expression values (HiSeqV2)|
|Clinical Data|Cancer histological types per sample|

> Samples were carefully aligned between molecular and clinical datasets to ensure label integrity.

# 🔄 Workflow Overview
```bash
Raw RNA-Seq Data
        ↓
Data Cleaning & Transposition
        ↓
Clinical Data Integration
        ↓
Feature Selection (Variance Filtering)
        ↓
Class Imbalance Handling
        ↓
Random Forest Model Training
        ↓
Evaluation & Interpretation
```

# ⚙️ Tech Stack
**Languages**: Python
**Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
**ML Model**: Random Forest Classifier
**Domain**: Cancer Genomics, Transcriptomics

# 🔍 Key Methodology Highlights
## 🧹 Data Preprocessing
- Transposed gene expression matrix to ML-friendly format
- Removed samples with missing clinical annotations
- Ensured one-to-one alignment between features and labels

## 🎯 Feature Selection
- Removed low-variance genes to reduce noise
- Addressed high dimensionality common in omics data

## ⚖️ Class Balancing
- Filtered cancer types with insufficient sample sizes
- Improved model robustness and statistical reliability

## 🤖 Machine Learning
- Stratified train-test split
- Random Forest chosen for non-linear pattern learning
- Multi-class classification across major cancer types

## 📊 Model Evaluation
- Accuracy
- Precision / Recall / F1-Score
- Confusion Matrix Visualization
> Misclassifications often occurred between biologically related cancers, reinforcing the model’s biological relevance.

## 📈 Results (Summary)
✔ Strong predictive performance across major cancer types
✔ Demonstrates cancer-specific transcriptomic signatures
✔ Validates machine learning applicability in genomics
![Confusion Matrix: Predicted Cancer Types]([/assets/myplot.jpg](https://github.com/shelinpreethi/cancer-type-prediction/blob/main/assets/myplot.jpg))

▶️ How to Run
```bash
git clone <repository-url>
cd CancerTypePrediction
pip install -r requirements.txt
jupyter notebook CancerTypePredictionFromGeneExpresionSignatures.ipynb
```
> Place TCGA expression and clinical files in the project directory before running.
# 🔮 Future Enhancements
- Hyperparameter optimization
- Feature importance & biomarker discovery
- Model comparison (SVM, XGBoost)
- External dataset validation
- Dimensionality reduction (PCA / Autoencoders)

# 👤 Author
**Shelinpreethi**
Aspiring Bioinformatics Analyst
Interests: Cancer Genomics • Machine Learning • Drug Discovery
LinkedIn: [[https://www.linkedin.com/in/shelinpreethi/]]

📌 Actively seeking roles in Bioinformatics / Data Analysis
