# Detail-scale Above Ground Biomass (AGB) Modeling  

## Description  
This folder contains scripts, models, and results for **Detail-scale AGB estimation**.  
The modeling integrates **UAV LiDAR data** with **forest inventory measurements** to assess biomass at a detailed scale.  

## Dataset  
- **Primary Data**: UAV LiDAR  
- **Supporting Data**: Field forest inventory  
- **Density Point Cloud**: 100-200 m2  
- **Field Survey & LiDAR Acquition date**: 18 - 21 September 2024  

The dataset was processed to produce the final dataset. The process consisted of data filtering, LiDAR data transformation (DSM, DTM, and CHM), Zonal Statistical, Tree Segmentation, and integration with AGB Field Survey. This final dataset was used in the model training and testing process.   

## Methods  
The AGB LiDAR model learning process is based on machine learning regression. We tried several regression algorithms classified as shallow learning and deep learning. The details are as follows:
- **Shallow Learning** :
  - Random Forest,
  - Gradient Boosting, 
  - Extra Trees,
  - MLP,
  - SVR,
  - LightGBM, and
  - Lasso  
- **Deep Learning** :
  - CNN-1D,
  - CNN-1D-attention,
  - CNN-1D-LSTM,
  - CNN-1D-attention-LSTM,
  - CNN-2D,
  - CNN-2D-attention,
  - CNN-2D-LSTM, and
  - CNN-2D-attention-LSTM  

## Performance 
- The evaluation of various **shallow learning models** is illustrated by the differences in model performance in predictive performance. The differences in performance can be seen in the following graph:
<img width="3580" height="1979" alt="Image" src="https://github.com/user-attachments/assets/b28d794d-bac8-4e30-8506-0c8f995b2333" />

***Note** : MAE and RMSE in Kg/Tree

- The evaluation of various **Deep learning models** is illustrated by the differences in model performance in predictive performance. The differences in performance can be seen in the following graph:
<img width="2480" height="1524" alt="Image" src="https://github.com/user-attachments/assets/3f49b624-cb70-45b7-9fb4-0af5c564294e" />

## Results
The details of the results of this study have been described in detail in our paper **“Comparison of Shallow and Deep Learning Algorithms for Aboveground Biomass Estimation Using LiDAR: Case Study of Eucalyptus Forest in Ibu Kota Nusantara, East Kalimantan Province, Indonesia”** (under review).
