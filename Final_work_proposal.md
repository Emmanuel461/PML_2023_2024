# Project Proposal

## Project Title
Soil Salinity Mapping with Remote Sensing and Convolutional Neural Networks

## Project Category
Regression

## Team Members
- Emmanuel Jesús Céspedes Rivera (Student ID: 28066)

## Description
The research focuses on the problem of soil salinity in rice production areas within mangroves, specifically in Guinea-Bissau, West Africa. This issue is of paramount importance due to the vital role of rice in the local diet and the significant impact of soil salinity on agricultural productivity in the region ([Balasubramanian et al., 2007](https://doi.org/10.1016/S0065-2113(06)94002-4); [Food and Agriculture Organization of the United Nations, 2018](https://www.fao.org/markets-and-trade/commodities/rice/rmm/en/)). Compounded by unpredictable rainfall patterns and inadequate diagnostic methods, the management of soil salinity poses a considerable challenge, underscoring the urgent need for innovative approaches ([Mendes and Fragoso, 2023](https://doi.org/10.3390/geosciences13020025); [Garbanzo et al., 2024](https://doi.org/10.3390/agronomy14020335)). Leveraging satellite imagery and machine learning algorithms offers a promising solution to address this complex issue and enhance agricultural practices in rice production ([Chuvieco, 2020](https://doi.org/10.1201/9780429506482); [Wu et al., 2018](https://doi.org/10.1002/ldr.3148)).

## Challenges
The research confronts several challenges:

- **Data Preparation:** Efficient extraction, access to satellite data, and selecting appropriate indices for salinity modeling pose significant challenges.
- **Identification of Optimal Indices:** Determining the most suitable indices for modeling salinity, considering the specific soil texture characteristics of the study area, is essential for accurate results.
- **Hyperparameter Optimization:** Attaining optimal hyperparameters is crucial to achieving high accuracy in the model predictions.
- **Integration of Diverse Data Types:** Integrating soil texture data with satellite imagery presents a unique challenge in ensuring seamless compatibility and meaningful interpretation.
- **Access to the data:** The work will include access to the data using the Google Earth Engine repository and using the library of GeeMap ([Geemap](https://geemap.org/)). 

## Dataset
The dataset comprises 183 soil samples collected from the village of Cafine, Guinea-Bissau, along with accompanying soil texture (Clay, Silt, and Sand) data and Sodium Absorption Ratio (SAR) measurements. The soil texture data is already interpolated with ordinary kriging and using the procedure of the work [Garbanzo et al., 2024](https://doi.org/10.3390/agronomy14020335). 

The satellite image will be from a PlanetScope (PS) sensor with a 3x3m spatial resolution. For more details visit ([PlanetScope Bands](https://developers.planet.com/docs/apis/data/sensors/)). The image will correspond to the month of soil sampling (March 2022). The date of acquisition of the image is 2022-05-28. 

## Method
The proposed approach utilizes Convolutional Neural Networks 1-D (CNN-1D) to address these challenges. By employing a buffer to extract satellite data and transforming it into a tabular format for modeling, the method has an important component of soil texture and satellite imagery data.

## Evaluation
Performance evaluation will be conducted using global model accuracy, root mean square error, mean absolute error, linear regression (observed vs predicted), and Pearson correlation coefficient metrics. These metrics will provide comprehensive insights into the effectiveness of the proposed model in accurately predicting soil salinity levels.
