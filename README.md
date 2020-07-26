# lifespan

### prediction human's life expectancy
* **data description**  
The Global Health Observatory (GHO) data repository under World Health Organization (WHO) keeps track of the health status as well as many other related factors for all countries The datasets are made available to public for the purpose of health data analysis. The dataset related to life expectancy, health factors for 193 countries has been collected from the same WHO data repository website and its corresponding economic data was collected from United Nation website. Among all categories of health-related factors only those critical factors were chosen which are more representative. It has been observed that in the past 15 years , there has been a huge development in health sector resulting in improvement of human mortality rates especially in the developing nations in comparison to the past 30 years. Therefore, in this project we have considered data from year 2000-2015 for 193 countries for further analysis. The individual data files have been merged together into a single dataset. On initial visual inspection of the data showed some missing values. As the datasets were from WHO, we found no evident errors. Missing data was handled in R software by using Missmap command. The result indicated that most of the missing data was for population, Hepatitis B and GDP. The missing data were from less known countries like Vanuatu, Tonga, Togo,Cabo Verde etc. Finding all data for these countries was difficult and hence, it was decided that we exclude these countries from the final model dataset. The final merged file(final dataset) consists of 22 Columns and 2938 rows which meant 20 predicting variables. All predicting variables was then divided into several broad categories:​Immunization related factors, Mortality factors, Economical factors and Social factors.
  
* **purpose**  
  1) Predict human life expectancy according to whether or not it is advanced => **purpose1_complete.ipynb**   
  2) Analyzing factors affecting human life expectancy in Asian countries => **purpose2_complete.ipynb**
  
* **Analytical methods**  
First, the data is preprocessed by checking the missing values and outliers. After that, the relationship between life expectancy and explanatory variables, which are response variables, is identified through data EDA. In this process, a simple linear regression model is constructed and evaluated by selecting one explanatory variable that has the highest relationship with the response variable. Then, based on the variable selection method and regression model evaluation, a multilinear regression model is constructed to predict the life expectancy more accurately.  
In addition, we build a second regression model that predicts life expectancy only for countries in the Asian continent to which Korea belongs. As a result, identify factors affecting life expectancy in Asian countries and compare the results with the results of the variable importance assessment of the randomforest model.
#
###### *final_report.pdf file is analysis results report*
###### *data sources are: https://www.kaggle.com/kumarajarshi/life-expectancy-who*
###### *This team project was conducted at the Dongguk University Regression Analysis Lecture*
