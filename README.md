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
   
   6. Illinois (Population: 12,569,321)  
   
   7. Ohio (Population: 11,714,618)  
   
   8. Georgia (Population: 10,830,007)  
   
   9. North Carolina (Population: 10,701,022)  
   
   10. Michigan (Population: 9,992,427)

 

     

  




