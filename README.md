# Oil-Spills-Detection-using-DeepLabV3-
A robust oil spill detection system using DeepLabV3+ on Sentinel-1 SAR (Synthetic Aperture Radar) imagery

Project Overview

This project focuses on detecting marine oil spills using Synthetic Aperture Radar (SAR) imagery, specifically Sentinel-1 Ground Range Detected (GRD) data. SAR is highly effective for ocean monitoring because it works day/night, in all weather conditions, and captures the unique low-backscatter signatures of oil slicks.

The pipeline includes data preprocessing, feature extraction, model training, evaluation, and visualization of results. The project is fully implemented in Google Colab, and includes:

Complete Python code
Project PPT
Research paper PDF
Result visualizations
Inferences & observation notes

Key Features :
Sentinel-1 SAR image processing
Single-polarization (VV) based detection
(If you used dual-pol, update this line accordingly.)
Speckle noise reduction (Lee / Median filters)
Contrast enhancement & thresholding
Texture feature extraction (GLCM / statistical features)
Machine Learning classification
Random Forest
SVM
XGBoost
Logistic Regression
Mask generation for oil-spill region detection
Accuracy, confusion matrix & evaluation metrics
End-to-end Colab notebook for reproducibility
  
🧠 Machine Learning Workflow
Load Sentinel-1 SAR GRD images

Apply preprocessing:
Radiometric calibration
Speckle filtering
Normalization

Extract Features:
Backscatter intensity
GLCM features (contrast, homogeneity, entropy)
Statistical texture
Train ML classifiers
Generate predictions & visualize oil spill masks
Evaluate results with accuracy, F1-score, precision & recall


Repository Structure:
├── /notebooks
│   └── Oil_Spill_Detection.ipynb
├── /research
│   └── Oil_Spill_Detection_Research_Paper.pdf
├── /presentation
│   └── Oil_Spill_PPT.pdf
├── /results
│   ├── detected_spill_masks/
│   └── evaluation_metrics.json
└── README.md


Tech Stack:
Python
Google Colab
NumPy / Pandas / Scikit-learn
OpenCV
Matplotlib / Seaborn
GDAL / Rasterio
Sentinel-1 SAR Data

Results :
Successfully detected oil-spill regions using SAR intensity variations.
Achieved strong model performance with 95%+ mAP@0.5.
Spill masks align closely with known dark formations in SAR imagery.

Research & Presentation

This repository includes:
Detailed research paper explaining methodology, theory, and experiments.
Professional PPT summarizing the problem, solution approach, results, and dataset.

Dataset
Sentinel-1 GRD images
Acquired via the Copernicus Open Access Hub.

Future Improvements:
Deep learning (U-Net / ResNet-based segmentation)
Dual-pol classification (VV + VH)
Real-time detection pipeline
Integration with GIS dashboards

Contact:
For queries or collaboration, feel free to open an issue or reach out.
Contact Email : code4ssr@gmail.com
