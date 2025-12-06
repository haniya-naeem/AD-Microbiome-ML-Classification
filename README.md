# AD-Microbiome-ML-Classification
This project proposes a computational, data-driven diagnostic framework for Alzheimer’s disease (AD) by integrating microbiome-derived genome-scale metabolic models (GEMs) and machine learning to accurately predict disease stages from gut microbial activity.

Cognitive State Classification Based on Microbiome Data

This project utilizes two different types of data, referred to as feature sets, to predict cognitive conditions such as Alzheimer's Disease(AD), Mild Cognitive Impairment (MCI), and Healthy through machine learning methods.

- The first feature set consists of Relative Abundance (RA), which includes microbial PCA (principal components analysis) components and top genus abundances.

- The second feature set combines RA with MICOM (Microbiome in Experiments) generated reaction flux and community growth rate estimates resulting in RA + MICOM features.

The analytical pipeline includes: data loading, data cleaning, data merging, data scaling, train/test splitting, cross-validation, hyperparameter tuning, and classification using Support Vector Machine (SVM) and Random Forest (RF).

- The results obtained: The RA only feature set produced moderate test accuracy (approximately 36% to 61%), indicative of the limited predictive power that exists when using only abundance data.

In addition, using the RA + MICOM features increased the predictive performance and achieved 75% test accuracy using the tuned SVM model.  This strongly supports the idea that better predictions can be made by combining microbial composition and metabolic activity. 
