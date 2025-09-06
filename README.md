# Indonesia’s FOLU Net Sink 2030 – WP 1.6: Geo-AI for Carbon Storage Assessment

## Project Description

This project is part of Indonesia’s FOLU Net Sink 2030 – IP UGM WP 2.6, focusing on Geo-AI Development and Use-case for Carbon Storage Assessment.
We develop a Geo-AI modeling system to support carbon stock assessment, following the IPCC Tier 2 and Tier 3 standards (medium and detail scale).

The study area is located in Sepaku Watershed, East Kalimantan, with a specific focus on Wanagama Forest in IKN (Nusantara Capital City).

## Objectives

- Develop models for Above Ground Biomass (AGB) and Land Use/Land Cover (LULC) at both medium and detail scales.
- Integrate remote sensing data (LiDAR, Sentinel, PlanetScope) with field forest inventory.
- Produce models using shallow learning and deep learning for carbon stock analysis.

## Dataset Modelling Summary
| Product| Scale  |  Primary Dataset  |	Additional Data Integration |             Methods               | 
|--------|--------|-------------------|-----------------------------|-----------------------------------|
|  AGB   | Detail |	   UAV LiDAR	    |   Forest inventory data     | Shallow Learning & Deep Learning  |
|  AGB	 | Medium |	   LiDAR GEDI	    |   Sentinel-1 & Sentinel-2   | Shallow Learning & Deep Learning  |
|  LULC	 | Detail |	   PlanetScope	  |             -               | Shallow Learning & Deep Learning  |
|  LULC	 | Medium |	Open Sentinel Map	|             -               | Shallow Learning & Deep Learning  |

## Methodology
All sub-activities apply a combination of Shallow Learning and Deep Learning approaches, including:
- Shallow learning algorithms (e.g., Random Forest, SVM, etc.).
- Deep learning architectures (e.g., CNN, U-Net, or other variations depending on the product).

***Note**: Detailed dataset metadata and methodology will be provided in each product folder. 

## Outputs
- Trained models in .pth and .joblib formats.
- Model performance evaluation (accuracy, confusion matrix, etc.).
- Spatial prediction products (Inference).

## License
- This dataset is made available under the Apache license. Freely available for both academic and commercial use, but protected by intellectual property rights. See the [LICENSE](./LICENSE) file for details.
- Access to Sentinel data is free, full and open for the broad Regional, National, European and International user community. View [Terms and Conditions](https://scihub.copernicus.eu/twiki/do/view/SciHubWebPortal/TermsConditions).
- Access to Planet data is restricted. View [Terms of Use](https://www.planet.com/terms-of-use/).
- The EULA for Pleiades imagery includes restrictions on how the imagery can be used. View [Terms and Conditions](https://space-solutions.airbus.com/legal/terms-and-conditions/)
- Access to GEDI LiDAR data is free. View [Terms and Conditions](https://gedi.umd.edu/data/products/)
- Access to Open Sentinel Map is free. This benchmark data was developed by Johnson (2022). View [Metadata](https://github.com/VisionSystemsInc/open-sentinel-map)

## Publication 
We are currently writing an article titled **“Comparison of Shallow and Deep Learning Algorithms for Aboveground Biomass Estimation Using LiDAR: Case Study of Eucalyptus Forest in Ibu Kota Nusantara, East Kalimantan Province, Indonesia”** (Under review). We will share the citation for this article once it has been published.

## Research Team
This project is developed by IP UGM – WP 1.6 Team in Indonesia’s FOLU Net Sink 2030. The authors for this project are: Sanjiwana Arjasakusuma, Projo Danoedoro, Danang Sri Hadmoko, Marzuki, Muhammad Arrafi, Yanuar Vira Febiyanti, Putri Laila Kartika Ningrum, Nur Laila Eka Utami, Aning Andita, Francisca Nova Puspatiyaningrum, and Ariseto Basworo from Department of Geographic Information Science, Faculty of Geography, Universitas Gadjah Mada.

## Acknowledge
The authors also would like to acknowledge the funding given under the scheme of FOLU NET SINK 2030 that has been granted to the Faculty of Geography, Universitas Gadjah Mada.
