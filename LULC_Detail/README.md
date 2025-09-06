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

## 🛠️ Methods  
- Shallow Learning (Random Forest, SVM, Gradient Boosting)  
- Deep Learning (U-Net)
