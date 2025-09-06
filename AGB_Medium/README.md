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
  - Bands : `'B2', 'B3', 'B4', 'B5', 'B6', 'B7', 'B8', 'B11', 'B12', 'VV', 'VH'`
  - Spatial Resolutions: 20 m (resampled)
  - Filter data: median in 2024

The dataset was processed to produce the final dataset. We extracted Sentinel-1 and Sentinel-2 pixel values with overlap in the GEDI coverage area. Then, we filtered the data and combined everything into a [.csv file](https://drive.google.com/file/d/1540Cgf7UT0HkAtD7fqEGvy2O0HcgkjeI/view?usp=drive_link)

## Methods  
The AGB medium scale model learning process is based on machine learning regression. We tried several regression algorithms classified as shallow learning and deep learning. The details are as follows:
- **Shallow Learning** :
  - Linear Regression,
  - Random Forest,
  - Gradient Boosting, and
  - SVR
- **Deep Learning** :
  - CNN-1D, and
  - CNN-1D-LSTM

## Performance 
- The evaluation of various **shallow and deep learning models** is illustrated by the differences in model performance in predictive performance. The differences in performance can be seen in the following graph:

<img width="450" height="450" alt="Image" src="https://github.com/user-attachments/assets/0289091e-abe4-4337-af53-c89b2b6eb06d" /> <img width="450" height="450" alt="Image" src="https://github.com/user-attachments/assets/ee4a9a7c-115a-4c31-bc0d-69e136e2c908" />

