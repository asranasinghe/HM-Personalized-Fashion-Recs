### H&M Personalized Fashion Recommendations
### Last Updated: 6/2/2022

<br>


#### Overview

This repository contained files that were developed as part of the H&M Personalized Fashion Recommendations Competition, hosted by Kaggle (https://www.kaggle.com/c/h-and-m-personalized-fashion-recommendations). The two notebooks provided are described below.

<br>

<ins>preprocessing.ipynb</ins>: 

Prepares data made available from the H&M Personalized Fashion Recommendation Competition (https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/data) for analyses performed in the model_building.ipynb notebook. 

First the transactions_full dataset is split into two dataframes, one comprising of purchases made before 8/1/2020 (named "tx_TrainTest"), and then other on or after 8/1/2020 (named "tx_val"). As the naming suggests, the former file is used for train / test, and the later for validation. These two files are used as the basis for subsequent data processing to prepare for market basket analysis, ALS analysis, and others. 

The note book also contains basic EDA and corresponding graphs.

<br>

<ins>model_building.ipynb</ins>: 

This notebook intakes parquet files created from the "preprocessing.ipynb" notebook and utilizes it for creation of various models for personalized fashion recommendations. The models created are listed below: <br>

(1) Seasonal Model <br>
(2) Trending Product Model <br>
(3) ALS Implicit Model <br>
(4) Market Basket Analysis <br>
(5) Ensemble Model

