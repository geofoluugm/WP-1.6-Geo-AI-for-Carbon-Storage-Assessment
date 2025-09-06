# Medium-scale Above Ground Biomass (AGB) Modeling  

## Description  
This folder contains scripts, models, and results for **Medium-scale AGB estimation**.  
The modeling integrates **UAV LiDAR data** with **forest inventory measurements** to assess biomass at a medium scale.  

## Dataset  
- **Primary Data**: GEDI LiDAR
  - [GEDI L4A Footprint Level Aboveground Biomass Density](https://www.earthdata.nasa.gov/data/catalog/ornl-cloud-gedi-l4a-agb-density-v2-1-2056-2.1)
  - Acquition: 2019 - 2023 (making a full footprint in the study area)
  - We have extracted the footprint GEDI and converted to [shapefile](https://drive.google.com/file/d/1BLQw0BsSjW1_b_8v6tKQBp8gpEAhVNoa/view?usp=drive_link)
- **Supporting Data**: Sentinel-1 & Sentinel-2 imagery  
  

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
