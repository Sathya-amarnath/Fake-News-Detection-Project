The Source code folder having below files
 Scrapping Data Folder
  - NYT_API_Key.txt -> NYT API Key file 
  - Guardian_API.txt -> Guradian API Key file
  - NYT_DB.csv -> NYT dataset 
  - Scraping_NYT_data.ipynb -> code for scrapping data from New York Times 
  - Scraping_Guardian_Data.ipynb -> code for scrapping data from Guradians Post newws i.e Washington DC Newspaper
 
Cleaning data
  -FakeNews_Notebook.ipynb -> code for cleaning Fake news data
  -Guardian_Cleaning.ipynb -> code for cleaning Guardian post data
  -NYT_Cleaning.ipynb -> code for cleaning New York Times data
 
Combining and Modeling
 - Combining and modeling.ipynb -> Code for implementation of models - Logistic regression, Random Forest and XGBoost
 

To execute the code,
First step is to scrape the data from NYT and guardians. Files to execute these are Scraping_NYT_data.ipynb and Scraping_Guardian_Data.ipynb
After scraping NYT data, we will get data into mongodb collection and export using mongoexport into NYT_DB.csv file.
After scraping data from Guradian post, we will get data in .json files.

Second step is to execute files in Cleaning data folder.
 - Execute FakeNews_Notebook.ipynb to clean the fakenews data
 - Execute NYT_Cleaning.ipynb to clean New York Times data. Input to this code will be NYT_DB.csv file
 - Execute Guardian_Cleaning.ipynb to clean Guardians data. Input to this code should be set of all json files that we collected from Scraping_Guardian_Data.ipynb

After cleaning all the three data, we will get FakeNews_Clean_All.csv, NYT_final.csv and Clean_TheGuardian_Combined_No_Slash.csv files.

Third step is to execute file from Combining and Modeling folder.
 - Execute Combining and modeling.ipynb file for combining the three datasets and training the models.
 The combined datasets are in file Complete_DataSet_Clean.csv file. This csv file will be input for training the classifiers.

  