# Daegu Apartment Prediction Analysis

**project status : On Hold**

## Project Domain

Daegu, as one of the largest cities in South Korea, has significant economic potential and development. With a rich history and strategic geographical position, Daegu becomes a center of economic, cultural, and educational activities. The growth of urbanization and industrial development in the city has created an increasing need for property information, especially regarding apartment sale prices. The increased demand for property market information in Daegu reflects the community’s need for clarity in making property purchase decisions. In an ever-changing environment, potential buyers or sellers of apartments require a deep understanding of price trends, factors influencing property value, and indications of investment prospects.

Human assessment is often limited in analyzing the complexity of various factors that affect apartment sale prices. Factors such as market trends, economic conditions, nearby infrastructure, and other local factors can be difficult to measure manually. This is the point where the presence of machine learning solutions becomes crucial. By using this technology, we can process and analyze data on a larger scale and objectively, providing deep insights into the dynamics of Daegu’s property market and overcoming the limitations of human assessment.

## Business Understanding
- In analyzing the property market needs of Daegu, it is important to understand market demand, including the type of properties most sought after, the level of availability, and location preferences. This information provides an overview of what potential buyers or renters want, and can help developers and investors direct their investments in a way that better aligns with the needs of the local community.

- The factors that influence the selling price of apartments in Daegu involve complex aspects such as location, nearby facilities, economic conditions, and infrastructure development. A thorough analysis of historical price data can help identify certain patterns and market trends. By understanding these factors, stakeholders can take strategic steps in determining a competitive selling price that aligns with market value

### Problem Statements

Based on the description above, the problems that need to be addressed are:
- How can we predict the selling price of apartments in Daegu?
- What are the most significant factors in determining the selling price of apartments?

### Goals

Based on the problem statemnts, the solutions that can be implemented include:
- Developing a machine learning model to predict the selling price of apartments. The machine learning model that can be implemented is a regression model for predicting numerical values such as the price of an apartment.
- Identifying factors that have a significant impact on apartment prices. This can be obtained by performing feature analysis to determine the variables that most affect the price.

## Data Understanding

Source of data [here](). The data has 4123 observations and 11 features. The features or columns of this dataset have the following meanings:

- **HallwayType** : Apartment Entrance Room Type.
- **TimeToSubway** : Time Required from Apartment to Subway Station (Categorical).
- **SubwayStation** : Underground station name near Apartment.
- **N_FacilitiesNearBy(ETC)** : Number of public facilities near apartments such as hotels and special schools.
- **N_FacilitiesNearBy(PublicOffice)** : Number of Public Offices Near the Apartment.
- **N_SchoolNearBy(University)** : Number of University Near the Apartment.
- **N_Parkinglot(Basement)** : Number of parking spaces in the basement.
- **YearBuilt** 
- **N_FacilitiesInApt** : The number of facilities for residents, such as swimming pools, gyms, and playgrounds.
- **Size(sqf)** : Apartment Size in Square Feet.
- **SalePrice** : Price in US$ (target).

### Data Analysis



## Data Preparation 

step by step data preparation:
- Remove Duplicate Data.
- Binning.
- Handling Cardinality.
- Handling Outlier wit Transformation.
- Handling Missing Value.

step by step feature engineering:
- Binning
- MinMaxScaling
- StandardScaling
- RareLabel Encoding
- OneHotEncoding

## Modeling

There are seven models used for making predictions. all these models use default parameters as a benchmark. the following are each model and the results from cross-validation

## Conclusion

- Based on the modeling that has been done, the features that most influence the selling price of the apartment in order are the size of the apartment, whether the type of entrance room of the apartment is a terrace, the number of facilities in the apartment, the number of parking spaces in the basement, and whether the time to the subway is fast or not.

- Considering the size of the MAPE (Mean Absolute Percentage Error) which is ~1.5%, we can conclude that the model we created when predicting prices for new data with the note that the range of values is the same as the training data values, then the average estimate will be off by approximately 1.5% from the actual price.