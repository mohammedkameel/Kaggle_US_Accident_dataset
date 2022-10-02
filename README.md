## Kaggle_US_Accident_dataset

This is the main read me file which contains all the information about the countrywide car accident dataset, which covers 49 states of the USA. The accident data are collected from February 2016 to Dec 2021, using multiple APIs that provide streaming traffic incident (or event) data. I have done EDA on the same.

**Currently, there are about 2.8 million accident records in this dataset.**

[Project - Kaggele - Countrywide Traffic Accident Dataset (2016 - 2021) EDA](https://mohammedkameel.github.io/Kaggle_US_Accident_dataset/)

- EDA on US countrywide car accident dataset, which covers 49 states of the USA.
- Used Pandas and Seaborn libabry 
***************************************************************************

#### We have use open datasets to load kaggale data into jupyter and import 
-> pip install opendatasets --upgrade --quiet 

-> import opendatasets as od -- hit

    **dataset_url = 'https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents'**
    **od.download('https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents')** 
    
 #### Saving file as data_filename variable 
     data_filename = './us-accidents/US_Accidents_Dec21_updated.csv'
     
 #### Information about below records
      df.tail() 
  
  ![imagetail](https://user-images.githubusercontent.com/56510494/192331993-41024bf8-1d45-4062-b59e-ea98d3748f09.PNG)

     
###   Plotting section
#### Cities by accident 
     cities_by_accident[:10].plot(kind ="barh")
     
 ![cities buy accident](https://user-images.githubusercontent.com/56510494/192334023-68f6144c-7036-48e8-bb97-ba5f52cacb2b.PNG)
 
 #### USA Population by cities 2022
 ![populationusa](https://user-images.githubusercontent.com/56510494/192597038-64306646-357b-4837-85ac-edb14b23c47b.PNG)
      
 #### What are the most populated states vs cities in the United States? Here is a list of the top ten most populated states in the country:

   1. California (Population: 39,613,493) <> City Los Angeles (Population: 3,971,883)(3.9 Million) 
   
   2. Texas (Population: 29,730,311) <> City: Houston (Population: 2,307,345)(2.9 Million), Dallas (Population : 1,308,814)(1.3 Milion)
   
   3. Florida (Population: 21,944,577) <> City Miami (Population: 441,003)(4 Lakhs) <> Orlando (Population: 309,154)(3 Lakhs)
   
   4. New York (Population: 19,299,981)  
   
   5. Pennsylvania (Population: 12,804,123)  
   
  

 
### Observation


NewYork being highest population there are no records. Miami has highest accidents however population is 4 lakhs as compare to Los Angeles population of 3Million in Califonia.
Orlando(Population: 3Lakhs), Dallas(Texas), Houston(Texas) at second and 3rd place. 

##### Now to see cities where accidents is more than 1000 compare to low cities with accidents and check them with distplot/histplot also with log scale. 

    high_accident_cities = cities_by_accident[cities_by_accident >= 1000]
  
  
    less_accident_cities = cities_by_accident[cities_by_accident < 1000]

#### Total count of cities having high accidents(<1000) 

     len(high_accident_cities) is 496



#### Less than 5% of cities have yearly 1000 accidents yearly. 

     len(high_accident_cities)/len(cities) 
   
   
   
   

#### Plotting for High accident cities 

     sns.distplot(high_accident_cities) 
     
![high accident](https://user-images.githubusercontent.com/56510494/193461929-4a218889-b473-4f98-8190-083e0e0feb73.PNG)

     sns.distplot(less_accident_cities) 
     
![low accident](https://user-images.githubusercontent.com/56510494/193461963-ca939a3a-f673-4ec4-98bb-ab43052fbf6a.PNG)


     sns.histplot(cities_by_accident, log_scale = True) 
     
![logscale](https://user-images.githubusercontent.com/56510494/193462011-7733ddd6-5c2f-42b5-b42d-f99033258fd5.PNG)

  




