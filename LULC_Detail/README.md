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
- Shallow Learning (Random Forest, SVM, Gradient Boosting, Naive Bayes)  
- Deep Learning (U-Net)

## Performance 
- The evaluation of various **Shallow learning models** is illustrated by the differences in model performance in predictive performance. The model's performance evaluated by metrics: Accuracy, Recall, Precision, and F1-Score. The differences in performance can be seen in the following graph:
<img width="400" height="400" alt="Image" src="https://github.com/user-attachments/assets/20212a39-4a52-4719-82aa-ca3998a0df10" />

- The evaluation of various **Deep learning models** is illustrated by the differences in model performance in predictive performance. The model's performance evaluated by metrics: Accuracy, Loss, and Intersect over Union (IoU). The differences in performance can be seen in the following graph:
<img width="600" height="600" alt="Image" src="https://github.com/user-attachments/assets/77ec7ffc-f8d0-4a3a-83ce-bd595603191e" />


## Results
We have tried applying the U-Net model to new data (inference).
<img width="600" height="600" alt="Image" src="https://github.com/user-attachments/assets/c141db5c-b857-4f34-b557-5b8357cd6ccc" />
