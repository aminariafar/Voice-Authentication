This project implements a **Voice Authentication system** that leverages **audio preprocessing, feature extraction, and machine learning models** to classify both **speaker gender** and **identity**, and to perform **clustering analysis** for grouping similar voices.  


## Project Overview
- **Audio Preprocessing**: 
  - Applied spectral subtraction for noise removal.
  - Extracted consistent middle segments with padding.
- **Feature Extraction**:  
  Extracted multiple audio features using `librosa`:
  - MFCC  
  - Spectral Bandwidth  
  - Spectral Centroid  
  - Mel Spectrogram  
  - Spectral Contrast  
  - Zero-Crossing Rate  

- **Classification**:
  1. **Gender Classification**  
     - Logistic Regression, KNN, XGBoost, and MLP.  
     - Best accuracy: **80.5% (MLP)**.  

  2. **Identity Classification (multi-class)**  
     - KNN, XGBoost, and MLP tested on subsets of students.  
     - XGBoost and MLP achieved best performance.  

- **Clustering**:
  - **KMeans**: Optimal clusters identified with Elbow and Silhouette methods.  
  - **DBSCAN**: Density-based clustering for alternative grouping.  
