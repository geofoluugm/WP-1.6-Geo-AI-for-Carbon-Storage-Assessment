# Detail-scale Land Use / Land Cover (LULC) Modeling  

## Description  
This folder contains scripts, models, and results for **Detail-scale LULC classification** using **PlanetScope imagery**.  

## Dataset
We have created a data benchmark for land cover and land use. The benchmark consists of image pairs and labels measuring 256*256 pixels. The metadata of the benchmark is as follows:
- **Primary Data**: PlanetScope imagery  
- **Spatial Resolution**: ~3 m  
- **Temporal Coverage**: 2024-04-03, 2024-03-18, and 2020-11-07  
- **Classes**: There are 13 classes:
  - Bareland
  - Cloud
  - Dryland Farming and Agriculture
  - Forest Regrowth
  - Grassland and Shrubland
  - Individual/Clustered Tree
  - Mangrove Forest and Swamp Forest
  - Natural Primary/Secondary Forest
  - Oil Palm Plantation
  - Other Tree Plantation
  - Road and Built-up
  - Shadow
  - Swamp
  - Water Body   

Preview benchmark:

<img width="600" height="600" alt="Image" src="https://github.com/user-attachments/assets/6232fb6d-877f-4e8c-b4ec-0e70b3df87b8" />

## 🛠️ Methods  
- Shallow Learning (Random Forest, SVM, Gradient Boosting)  
- Deep Learning (U-Net)
