# Medium-scale Land Use / Land Cover (LULC) Modeling  

## Description  
This folder contains scripts, models, and results for **Medium-scale LULC classification** using **Benchmark Open Sentinel Map**.  

## Dataset
The OpenSentinelMap dataset contains Sentinel-2 imagery and per-pixel semantic label masks derived from OpenStreetMap. The detail specification of the OpenSentinelMap can you read on their repository [OSM](https://github.com/VisionSystemsInc/open-sentinel-map). 

The specific OSM datasets we have used include: 
- Data key : gsd_10
- Spatial resolution: 10 m
- Bands : B02, B03, B04, B08
- OSM sentinel imagery datasets 2020

We applied several preprocessing steps, such as: 
- Filtering data with a “bad_percent” key below the threshold of 0.05.
- We selected images that only had the ‘wooded’ class label.

Our target mapping only class `wooded` and `non-wooded`. 
We determined this to be in line with our objectives. Furthermore, the proportion of data labels owned by OSM is not balanced between each class. Based on our analysis, in the dataset we used, the ‘wooded’ class had a dominant proportion compared to other classes. 

## 🛠️ Methods  
- Shallow Learning (Random Forest, SVM, Gradient Boosting, Naive Bayes)  
- Deep Learning (U-Net)

## Performance 
- The evaluation of various **Shallow learning models** is illustrated by the differences in model performance in predictive performance. The model's performance evaluated by metrics: Accuracy, Recall, Precision, and F1-Score. The differences in performance can be seen in the following graph:
<img width="500" height="500" alt="Image" src="https://github.com/user-attachments/assets/87c29c09-6d95-4cc0-8cf7-2a6d24740f32" />

- The evaluation of various **Deep learning models** is illustrated by the differences in model performance in predictive performance. The model's performance evaluated by metrics: Accuracy, Loss, and Intersect over Union (IoU). The differences in performance can be seen in the following graph:
<img width="600" height="600" alt="Image" src="https://github.com/user-attachments/assets/3ad5b6b4-9748-4f4b-80d2-8b48348598c4" />

## Results
We have tried applying random forest and gradient boosting model to new data (inference).
<img width="400" height="400" alt="Image" src="https://github.com/user-attachments/assets/68eb4ca7-49b0-4537-8f00-9a78bcd09e51" />
<img width="400" height="400" alt="Image" src="https://github.com/user-attachments/assets/c2c0f2bd-4566-4b98-8c60-95da785e17c1" />
