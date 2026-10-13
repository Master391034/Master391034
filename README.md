## Hi there 👋
My name is Ivan, I'm a biologist-turned-ML-engineer with a passion for applying data science to medicine, biology and agriculture.
I hold a Master's degree from the Faculty of Soil Science of Lomonosov Moscow State University, and I'm currently looking for a junior ML/DS position or internship in the agrotech / biotech domain.

## Core competences

- **Machine Learning & Deep Learning:** supervised learning, transfer learning, autoencoders, model interpretation (SHAP, Grad-CAM)
- **Computer vision:** semantic segmentation (U-Net / U-Net++, EfficientNet encoders), ensembling, TTA, classical CV for measurement tasks (OpenCV)
- **Multi-omics integration:** bulk RNA-seq, scRNA-seq, methylation, miRNA; MOFA, PCA, UMAP, custom autoencoders
- **Bioinformatics:** genome assembly (Illumina + Nanopore), metagenomics (16S, DADA2, PiCRUST, Kraken2), alignment, variant calling
- **Validation discipline:** leakage-free cross-validation by group, blind ground-truth annotation, controls that fail loudly, domain-shift awareness
- **Tools & Languages:** Python (pandas, scikit-learn, PyTorch, CatBoost, OpenCV), R, Bash, Git, Docker.
- **Soft skills:** project documentation, reproducible research, clear visualizations

## Projects

### [Multi-omics survival prediction for breast cancer (TCGA-BRCA)]
Integration of expression, methylation and miRNA data with autoencoders, MOFA, PCA and UMAP.  
- Cross‑validated comparison of 6 methods; final model – Autoencoder 2 + CatBoost (C‑index = 0.626)  
- Biological interpretation of latent factors (apoptosis, proliferation, methylation, motility)  
- Clean notebook, production‑ready model saving, full documentation

### [FTU segmentation] — 2nd place, OpenBio competition

Segmentation of functional tissue units in five organs (kidney, prostate, large intestine, lung, spleen), 1744 train images, metric: mean IoU. Final score **0.7588**.
- Ensemble of 5 CNN segmentation models (U-Net / U-Net++ with EfficientNet encoders), 8-fold TTA, per-organ thresholds, GroupKFold by patient
- **Geometric-mean ensembling** instead of arithmetic: acts as an agreement filter — a single confident "background" vote suppresses the pixel. 
- **Entropy gating for lung:** alveoli are nearly indistinguishable from background by brightness (Δ5 px), but differ in texture entropy (4.21 vs 2.95). Switching from segmentation to tile-level detection of FTU presence gave +0.19 IoU on validation and +0.007 LB
  
### [Breast Cancer Wisconsin – interpretable ML]
Complete ML pipeline on tabular data: EDA, cross‑validation of 7 classifiers, Optuna hyperparameter tuning, SHAP analysis.  
- XGBoost selected as final model; threshold analysis and production saving without scaler

## 🎓 Education
- **Master’s degree** – Faculty of Soil Science, Lomonosov Moscow State University  
- **Bioinformatics & Data Science** – multiple specialized courses and workshops (Blasteam, faculty of AI MSU, OpenBio, Positive Technologies)

## 📫 Contact
- Email: [stata-boss88@mail.ru]  
- Telegram: @Master21003 

*Open to internships and junior positions in biomedical ML / data science – feel free to reach out!*
