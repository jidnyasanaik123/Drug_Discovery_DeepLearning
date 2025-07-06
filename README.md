# AI-Powered Drug Discovery using Deep Learning 🧬💊

This project demonstrates a deep learning-based pipeline for predicting IC50 values in drug-target interactions using publicly available datasets.

## 📌 Project Overview
Drug discovery is a complex and expensive process. This project leverages deep learning to predict drug-protein binding strength (IC50) using molecular fingerprints and one-hot encoded targets.

## 📁 Dataset
- **Source**: [Therapeutics Data Commons (TDC)](https://tdcommons.ai/)
- **Dataset Used**: `bindingdb_ic50`
- **Type**: Drug-target interaction data with IC50 values

## ⚙️ Methodology
1. **Data Preprocessing**:
   - Convert SMILES strings to Morgan fingerprints using RDKit.
   - One-hot encode target protein names.
2. **Model Architecture**:
   - Two input branches: Drug and Target
   - Each branch contains fully connected layers with ReLU
   - Concatenate both embeddings → Dense output layer (regression)
3. **Training**:
   - 5-Fold Cross-Validation
   - Loss Function: Mean Squared Error (MSE)
   - Optimizer: Adam

## 📊 Evaluation
- Metric: Root Mean Squared Error (RMSE)
- Results plotted as RMSE vs Fold to visualize performance.

## 🧠 Requirements
```bash
pip install pytdc rdkit-pypi torch-geometric torch pandas matplotlib seaborn scikit-learn plotly
```

## 📈 Outputs
- RMSE scores for each fold
- IC50 prediction performance graph
- Draft paper with architecture diagram
- Code explanation video

## 📂 Deliverables
- `Research_Report_AI_Drug_Discovery.docx`
- `Drug_Discovery_DeepLearning.ipynb`
- `Draft_Paper_With_Diagram.docx`
- Code explanation script/video

## 🤝 Contributors
- [Jidnyasa Naik]

---
© 2025 • AI for Drug Discovery | Educational Use Only
