# Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis

**Data originally sourced from a wastewater treatment plant in Melbourne, Australia.  Atmospheric data compiled by Melbourne weather stations.**

**Original Data link**  https://www.kaggle.com/datasets/d4rklucif3r/full-scale-waste-water-treatment-plant-data

## Data Dictionary
Average Outflow (avg_outflow): Treated wastewater released back into the environment.

Average Inflow (avg_inflow): Contaminated wastewater entering the treatment plant.

Energy Consumption (total_grid): The amount of energy used by the treatment plant, which is influenced by pollutant load, treatment methods, and climate.

Ammonia (A): A critical nutrient in biological wastewater treatment, it is converted by bacteria to break down food or BOD.

Biological Oxygen Demand (BOD): A measure of oxygen required by microorganisms to decompose organic matter in water, indicating the level of organic pollution in wastewater.

Chemical Oxygen Demand (COD): A measure of oxygen needed to oxidize all organic matter in a water sample, indicating organic pollution.

Total Nitrogen (TN): The sum of all forms of nitrogen in wastewater, important for treatment and preventing eutrophication.

Average Temperature (T): Influences wastewater treatment processes, with warmer temperatures leading to faster biodegradation and higher oxygen uptake.

Maximum Temperature (TM) and Minimum Temperature (Tm): Warmest and coldest months, affecting microbial activity and treatment system design.

Atmospheric Pressure (SLP), Average Humidity (H), Total Rainfall (PP), Average Visibility (VV), Average Wind Speed (VW), and Maximum Wind Speed (VG): Atmospheric conditions affecting the evaporation processes of the plant and overall treatment efficiency.

##**Goal:**

The project will involve data analysis and building predictive models to estimate the energy consumption of the wastewater treatment plant based on the given atmospheric and biologic variables. Machine learning algorithms will be utilized to create the most suitable model, enabling better understanding and optimization of energy usage in wastewater treatment processes as well as predict future energy requirements needed to process wastewater for reintroduction to groundwater recharge zones.  

##**Methods**
- .
- .
- .
- .

##**Results**
![image](https://github.com/combechelsey/Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis/assets/132314345/256d8259-471c-4908-9d9c-934984ea26dd)
###Analyzing Inflow rate vs Outflow rate paired with the mean Energy Consumption of the plant.

![image](https://github.com/combechelsey/Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis/assets/132314345/738441f6-cba3-4217-97de-19c1c2b98315)
###Climate and temperature play a big part in the total energy consumption of the plant.  As temperatures increase, energy consumption averages tend to decrease.  This likely has to do with the increase of available biologic components present to breakdown waste when temperatures rise.  

![image](https://github.com/combechelsey/Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis/assets/132314345/5bc41c49-eaac-4efb-910b-ed161c97928a)
###We can see here that Ammonia and Total Nitrogen have a negative corralation with the energy consumption of the wastewater plant.  

![image](https://github.com/combechelsey/Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis/assets/132314345/472a0141-a597-4e89-ab93-a7f6d9e50c05)
###SImilar to above, bilogical and chemical oxygen demand are commonly used to determine the degree of contamination of the incon=ming wastewater and have a negative corralation with the energy consumption of the wastewater plant.

![image](https://github.com/combechelsey/Full-Scale-Waste-Water-Treatment-Plant-Data-Analysis/assets/132314345/06858249-3cf7-4799-9206-ede0346c918b)

