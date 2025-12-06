Machine Learning Analysis: Gut Microbiome Classification

This notebook exhibits the machine-learning application of determining the patients’ gut microbiome samples classified into three different clinical states: Healthy State, Mild Cognitive Impairment (MCI), and Alzheimer’s Disease (AD). The classification is based on taxonomic features (relative abundances) and the metabolic features predict by MICOM.

Project Structure: 
- ML Visualizations.ipynb – The purpose of the notebook is to provide visual representations of how well the models performed and how to explore individual features.
- ML_Figures.ipynb – This notebook contains the code necessary to create various types of visual summaries (confusion matrices, metrics tables, etc.).
- Machine_Learning_Analysis.ipynb – This notebook is the primary notebook for the project; it includes tasks such as data preprocessing and merging features, training the model, and an analysis of the model.


Features and Dataset
- Relative Abundance Features: The relative abundance is actually PCA Component Scores as well as Genera of Microbial Species that are found in each patient sample.
- MICOM Features: The predicted metabolic flux and predicted growth rate of the microbial community.
- The merged dataset contains both Relative Abundances and MICOM features to be used to train the model.


Machine Learning Models
- Model A: Support Vector Machine (SVM) using Relative Abundance Only
- Model B: Random Forest using Relative Abundance Only
- Model C: SVM using Relative Abundance + MICOM

For all models, the training/testing split was completed, the models/rfs were evaluated using Cross Validation, and all were analyzed using precision, recall, and F1-Scores as well as confusion matrices to aid in understanding the results.
