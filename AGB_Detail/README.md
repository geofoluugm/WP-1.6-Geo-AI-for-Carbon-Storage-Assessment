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

