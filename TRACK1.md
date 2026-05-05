Imagine Decoding Challenge

Track 1: Kaggle Competition

Group Members: Athirah, Heidi and Izzah

1. Project Overview

   This project focuses on the Imagine Decoding Challenge, where the objective is to predict 10 object categories from MEG brain activity (306 channels × 121          timepoints). This task involves processing high-dimensional time-series data with a low signal-to-noise ratio.

2. Methodology & Preprocessing

   To improve model performance, we implemented the following pipeline:

   I) Standardization: Applied StandardScaler across MEG channels to normalize the signals.  
   II) Data Augmentation: Combined data from multiple subjects to increase the training sample size.  
   III) Stratified Splitting: Used stratified shuffling to maintain class balance during validation.

3. Iterative Model Development (Assessment 2)

   We conducted experiments to compare a baseline approach against an improved architecture
   
| Version |       Model       |        Technique          | Val Accuracy |       Notes           |
|---------|-------------------|---------------------------|--------------|-----------------------|
|    v1   |    Simple CNN     |        Baseline           |    ~10%      |    No preprocessing   |
|    v2   | EEGNet + Ensemble | BN, Dropout, LR Scheduler |    ~TBD      | Improved architecture |



4. Key Insights

   a) Class Distribution: Our Exploratory Data Analysis (EDA) confirmed a balanced distribution across all 10 labels.  

   b) Model Bias: The confusion matrix for the improved model indicates a bias toward Class 9, suggesting that the model is struggling to differentiate specific    high-frequency features in the MEG signals.  

   c) Signal Variance: Most of the variance is concentrated in the early channel indices, requiring precise feature scaling.
