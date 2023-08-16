# **Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis** 
<b>
<b>
<b>

## **Project Overview:** 

Wastewater is water that has been contaminated by human activities, environmental factors, or industrial processes. Thorough treatment is necessary to ensure safe reclamation or responsible disposal. Decontaminated water from Wastewater Treatment Plants (WWTP) is reintroduced into water bodies and aquifer recharge zones. Each step of the treatment process demands careful attention due to the potential impact on aquatic ecosystems and the risk of biological consequences.

<b>
<b>
<b>

**Data originally sourced from a wastewater treatment plant in Melbourne, Australia.  Atmospheric data compiled by Melbourne weather stations.**

**Original Data link**  https://www.kaggle.com/datasets/d4rklucif3r/full-scale-waste-water-treatment-plant-data

<b>
<b>
<b>

## **Data Dictionary**

<b>
<b>

 - **Average Outflow** (avg_outflow): Treated wastewater released back into the environment.
<b>
<b>

- **Average Inflow** (avg_inflow): Contaminated wastewater entering the treatment plant.
<b>
<b>

- **Energy Consumption** (total_grid): The amount of energy used by the treatment plant, which is influenced by pollutant load, treatment methods, and climate.

<b>
<b>

 - **Ammonia** (A): A critical nutrient in biological wastewater treatment, it is converted by bacteria to break down food or BOD.

<b>
<b>

 - **Biological Oxygen Demand** (BOD): A measure of oxygen required by microorganisms to decompose organic matter in water, indicating the level of organic pollution in wastewater.

<b>
<b>

 - **Chemical Oxygen Demand** (COD): A measure of oxygen needed to oxidize all organic matter in a water sample, indicating organic pollution.

<b>
<b>
 
 - **Total Nitrogen** (TN): The sum of all forms of nitrogen in wastewater, important for treatment and preventing eutrophication.

<b>
<b>

 - **Average Temperature** (T): Influences wastewater treatment processes, with warmer temperatures leading to faster biodegradation and higher oxygen uptake. 

<b>
<b>

 - **Maximum Temperature** (TM) and Minimum Temperature (Tm): Warmest and coldest months, affecting microbial activity and treatment system design.

<b>
<b>

 - **Atmospheric Pressure** (SLP)

<b>
<b>

 - **Average Humidity** (H): Atmospheric conditions affecting the evaporation processes of the plant and overall treatment efficiency.

<b>
<b>

 - **Total Rainfall** (PP): Atmospheric conditions affecting the evaporation processes of the plant and overall treatment efficiency.

<b>
<b>

 - **Average Visibility** (VV): Atmospheric conditions affecting the evaporation processes of the plant and overall treatment efficiency.

<b>
<b>

 - **Average Wind Speed** (VW): Atmospheric conditions affecting the evaporation processes of the plant and overall treatment efficiency.

<b>
<b>

 - **Maximum Wind Speed** (VG): Atmospheric conditions affecting the evaporation processes of the plant and overall treatment efficiency.

<b>
<b>
<b>

## **Goal:**

The project will involve data analysis and building predictive models to estimate the energy consumption of the wastewater treatment plant based on the given atmospheric and biological variables. Machine learning algorithms will be utilized to create the most suitable model, enabling a better understanding and optimization of energy usage in wastewater treatment processes as well as predicting future energy requirements needed to process wastewater for reintroduction to groundwater recharge zones.  
<b>
<b>
<b>

## **Data Preprocessing**

- There are 1382 rows and 20 columns within this data frame.
- Data contains no missing or NaN values.
- No duplicated rows.
- All 20 columns are numeric datatypes.

<b>
<b>
<b>


## **Exploratory Data Analysis (EDA):**


****
<b>
<b>
<b>

![Heatmap of Variables](https://github.com/combechelsey/Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis/assets/132314345/02ae96a6-141c-4e6d-9c52-3e9c7e72f2c2)

### **We can observe from this correlation map that temperature, along with TM and Tm (maximum and minimum temperature), has the most significant negative correlation with the plant's energy consumption. As temperatures decrease, energy consumption rises. The month of the year also appears to be correlated with energy consumption, likely influenced by seasonal average temperatures. We also note weak negative correlations with nitrogen and ammonia content, as well as the required Biological Oxygen Demand of the contaminated water. The strongest positive correlations, albeit weak, with our target variable are associated with year, humidity, average inflow, and average outflow.**
 


<b>
<b>
<b>

![Temperature and Energy Consumption](https://github.com/combechelsey/Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis/assets/132314345/094c54ae-b689-4ee9-ae62-d7e117df7e1f)


### **Climate and temperature appear to significantly influence the overall energy consumption of the plant. As temperatures rise, there is an observable trend of decreased energy consumption averages. This occurrence is likely attributed to the increased availability of biological components present for waste breakdown when temperatures are elevated.**  

<b>
<b>
<b>

![Energy trends over time](https://github.com/combechelsey/Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis/assets/132314345/b6abf503-99d5-441f-a6b9-fc73436741ae)


### **The figure above depicts the energy consumption pattern for powering the wastewater treatment facility. Notably, there has been a pronounced upward trend in energy demand over time. Moreover, post-2016, the seasonal fluctuations in energy requirements have significantly diminished, indicating a more consistent energy consumption pattern. This further underscores the critical role of energy infrastructure and planning in the operations of the plant**
<b>
<b>
<b>

![Inflow over time](https://github.com/combechelsey/Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis/assets/132314345/e6dbc465-d419-4854-9db4-4638f47a0784)


### **Over time, there has been a consistent upward trend in the average inflow to the wastewater plant. The rates have nearly doubled from their levels in 2014 to those observed in 2019. Additionally, there is an observable increase in the occurrence of larger influxes of heightened inflow.**


<b>
<b>
<b>

![Precipitation averages by month](https://github.com/combechelsey/Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis/assets/132314345/bbde284b-6d9a-4f69-a8ab-4859df93f5fd)


### **April exhibits the highest amount of rainfall, closely followed by September and October. On the other hand, November and May experience the least amount of precipitation. Notably, increases in inflow are unlikely to be attributed to groundwater runoff resulting from precipitation. To delve deeper into the relationship between inflow and other factors, such as temperature, warrants exploration.**


<b>
<b>
<b>

![Temperature and inflow averages](https://github.com/combechelsey/Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis/assets/132314345/05bce61d-d13d-4bcf-bf14-67665dd59bc8)


### **Temperature is strongly correlated with monthly inflow averages suggesting that the extra inflow during warmer months of the year may be a result of groundwater runoff caused by non-atmospheric conditions.  Perhaps the result of irrigation of crops or farmland or landscape watering in urban areas.  This may be the cause of the dilution of wastewater and thus the reduction of energy expenditure at times of increased inflow.**

<b>
<b>
<b>

![Nitrogen Levels and Energy Use](https://github.com/combechelsey/Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis/assets/132314345/e64eb440-7367-488e-bc99-d61cf3e79e07)


### **As the levels of total nitrogen increase, there is a corresponding reduction in the treatment facility's reliance on the energy grid.**


<b>
<b>
<b>

![Biological Oxygen Demand and Energy Use](https://github.com/combechelsey/Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis/assets/132314345/868c2c4a-de64-4d91-9423-7382c6e4dc66)

### **A negative correlation exists between Biological Oxygen Demand and energy consumption.**


<b>
<b>
<b>

![Temperature and Energy Consumption](https://github.com/combechelsey/Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis/assets/132314345/701bcc99-1327-4791-92f4-9bbfe41e682d)


### **There is a negative correlation between atmospheric temperature and energy consumption.**



<b>
<b>
<b>

![Humidity and Energy Use](https://github.com/combechelsey/Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis/assets/132314345/5c500da7-f009-489c-9654-0a12b72e2cf7)


###**There is a weak positive correlation between Humidity and energy use.**



<b>
<b>
<b>

## **Modeling Preprocessing**


To prepare the data for modeling, we will take the following steps:

- Remove columns that are constant or quasi-constant, such as Atmospheric Pressure (SLP).
- Drop the "Maximum Wind Gust" column to reduce noise as we are more interested in the average wind speed data.
- Exclude the "day" column to concentrate on broader trends within the data.
- Combine the "Month" and "Year" columns into a single datetime column, allowing for modeling of long-term trends.
- Since there are no missing values, there is no need for imputation.
- Scale the numeric columns.
- There are no ordinal or nominal columns requiring processing through the pipeline.

<b>
<b>
<b>

## **Modeling Result Metrics:**


<img width="179" alt="Modeling Metrics" src="https://github.com/combechelsey/Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis/assets/132314345/bb335908-f181-4440-a38a-2fb5baaf7fa2">

<b>
<b>
<b>

## **Model Evaluation:**

**After an evaluation of twenty different models, we have determined that the Extreme Gradient Boosting Tuned model is the highest ranking model of those we trained. WIth an R2 score of 18.7% on the testing data and an MAE of 32091, the model is able to explain just under 19 peercent of the variance in our dataset as it currently is. While is is important to note a large degree of overfitting in this model, the XGBoost approach gave an average error of 32091 energy units and further exploration of this model may provide a promising pathway for predictive accuracy of the future energy requirements of Wastewater Treatment Facilities.**


<b>
<b>
<b>

## **Dependencies:**

### Imported libraries:

import pandas as pd

import numpy as np

import matplotlib.pyplot as plt

import seaborn as sns

### Preprocessing Imports:

from sklearn.model_selection import train_test_split, GridSearchCV

from sklearn.compose import make_column_selector

from sklearn.preprocessing import StandardScaler

from sklearn.pipeline import make_pipeline

from sklearn.compose import make_column_transformer

from sklearn.impute import SimpleImputer

from sklearn.compose import ColumnTransformer



### Modeling Imports:

from sklearn.dummy import DummyRegressor

from sklearn.tree import DecisionTreeRegressor

from sklearn.ensemble import RandomForestRegressor

from sklearn.ensemble import GradientBoostingRegressor

from sklearn.decomposition import PCA

from sklearn.svm import SVR

import xgboost as xgb

import lightgbm as lgb


<b>
<b>
<b>

## **Contact Information:**

**Author:  Chelsey Combe**
- email combechelsey@gmail.com

- github  https://github.com/combechelsey


<b>
<b>
<b>

## **Acknowledgments:**

Data was originally sourced from Arsh Anwar on Kaggle. 

Original Data Notebook by Lucifer ML on Kaggle: 
 https://www.kaggle.com/code/d4rklucif3r/waste-water-treatment-plant-luciferml-viz

License:  CC BY-SA 4.0

Scientific Article referenced for information:  https://www.sciencedirect.com/science/article/abs/pii/S0957582021004663?via%3Dihub



