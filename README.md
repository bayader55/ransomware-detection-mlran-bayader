# ransomware-detection-mlran-bayader
# Ransomware Detection using Machine Learning — MLRan Dataset

## 📌 Project Overview
Binary classification of software samples as Goodware (0) or Ransomware (1) 
using the MLRan dataset. Four ML models are trained and compared with full 
explainability analysis (SHAP, t-SNE).

## 📊 Dataset
- **MLRan** (Onwuegbuche et al., 2025)
- 483 binary behavioral features (RFE-selected)
- Source: https://github.com/faithfulco/mlran

## 🚀 How to Run
1. Open the notebook in Google Colab: https://colab.research.google.com/drive/1WjJKVPEgTPc8aE-UwJaUBvDAS5Rw_w4E?usp=sharing
2. Run all cells in order (Cell 1 will auto-download the dataset)
3. No manual setup required — all dependencies are pre-installed in Colab

## 📦 Dependencies
scikit-learn, pandas, numpy, matplotlib, seaborn, shap, joblib
## 🗂️ Notebook Structure
| Cell | Description |
|------|-------------|
| 1 | Data Ingestion (Drive + GitHub) |
| 2 | EDA — Textual Report |
| 3 | EDA — 8 Visualization Figures |
| 4 | Preprocessing & Balancing |
| 5 | Model Training & Cross-Validation (4 models) |
| 6 | Final Evaluation on Test Set |
| 7 | Evaluation Figures (6 figures) |
| 8 | XAI — SHAP & Permutation Importance |
| 9 | t-SNE Latent Space Projection |
| 10 | Model Export & Inference Test |

## 📈 Results Summary
 Model                      Acc      F1    Prec     Rec     AUC  ValAcc
  ────────────────────── ─────── ─────── ─────── ─────── ─────── ───────
  Random Forest           0.9679  0.9683  0.9538  0.9840  0.9959  0.9577
  Gradient Boosting       0.9799  0.9799  0.9762  0.9838  0.9959  0.9648
  SVM (RBF)               0.9779  0.9778  0.9724  0.9840  0.9981  0.9648
  MLP Neural Network      0.9618  0.9624  0.9462  0.9799  0.9945  0.9507
  ────────────────────── ─────── ─────── ─────── ─────── ─────── ───────

  🏆 Best model (Val Accuracy): Gradient Boosting (0.9648)

## 👤 Author
Bayader Azabou — 4CS, May 2026
