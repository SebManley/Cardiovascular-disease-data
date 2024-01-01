# Cardiovascular disease data (2022) <img src="https://media0.giphy.com/media/26BRv0ThflsHCqDrG/giphy.gif?cid=ecf05e4781lacu8c51zi2phdvpeb4k7rehqa3b3x0vxktuxe&ep=v1_gifs_search&rid=giphy.gif&ct=g" width="50" height="50" />

## Project Overview:
This project focused on processing and visualising the data obtained from the Centers for Disease Control and Prevention's 2022 Behavioral Risk Factor Surveillance System (BRFSS) questionnaire performed in all of the states and territories of the United States of America. The questionnaire surveryed 445,000 American citizens on health-related questions, inlcuding health risk behaviors, chronic diseases and conditions, access to health care, and use of preventive health services.

**Project goal:** To process the BRFSS data to a human-readable format and draw insights using visualisations to help understand the lifestyle factors that drive cardiovascular risk, which is the leading cause of global mortality (Roth et al., 2020).

## Data Cleaning and Processing:
* Read the parquet file containing questionnaire responses into a Pandas dataframe.
* Focused the dataframe by creating a CSV file containing the desired SAS column name and using it to select 42 out of the 326 columns  - leaving only the columns that provide the most information in achieving the project goal.
* Created a list of informative column labels to replace the corresponding SAS column names to increase the readability of the columns.
* Removed rows that are missing data on cardiovascular disease.
* Converted numerical values into descriptive values to increase the interpretation of the data.

## Data visualisation:
The primary goal of this project was to help understand the lifestyle factors that influence cardiovascular disease risk in modern day America. This has been achieved through the creation of 6 figures, each of which provide unique insights. The primary metric used as an indicator of cardiovascular disease was the calculated variable 'Had Coronary Artery Disease or Myocardial Infarction' as these events are the most prevalent cardiovascular disease manifestations (Roth et al., 2020).

* **Figure 1:** Relationship between Age and Cardiovascular Disease Risk.

* **Figure 2:** Relationship between Smoking and Cardiovascular Disease Risk.

* **Figure 3:** Relationship between Sex and Cardiovascular Disease Risk.

* **Figure 4:** Relationship between Exercise and Cardiovascular Disease Risk.

* **Figure 5:** Relationship between BMI and Cardiovascular Disease Risk.

* **Figure 6:** Leading Five U.S. States in Cardiovascular Event Frequency.

## Data Source:
The parquet file was acquired from https://github.com/kamilpytlak who extracted the raw questionnaire response data directly from https://www.cdc.gov/brfss/annual_data/annual_2022.html

## Requirements:
* Pandas
* NumPy
* Seaborn
* Matplotlib
* Chardet

**Note: If using the Heart_disease_data Notebook locally, change any file paths to match the actual file path.**
