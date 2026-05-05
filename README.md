Imagine Decoding Challenge

Track 1: Kaggle Competition

Group Members: Athirah, Heidi and Izzah

1. Project Overview

This project focuses on the Imagine Decoding Challenge, where the objective is to predict 10 object categories from MEG brain activity (306 channels × 121     timepoints). This task involves processing high-dimensional time-series data with a low signal-to-noise ratio.

3. Methodology & Preprocessing

   To improve model performance, we implemented the following pipeline:

   I) Standardization: Applied StandardScaler across MEG channels to normalize the signals.  
   II) Data Augmentation: Combined data from multiple subjects to increase the training sample size.  
   III) Stratified Splitting: Used stratified shuffling to maintain class balance during validation.

4. Iterative Model Development (Assessment 2)

   We conducted experiments to compare a baseline approach against an improved architecture
