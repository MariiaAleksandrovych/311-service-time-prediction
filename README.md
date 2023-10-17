#  311 Service Time Prediction Agencies in New York City 

We aim to test out three different models — a linear regression, a neural network, and a decision tree — to determine if we can predict how long it takes to resolve 311 calls. We anticipate that significant features could be the particular city agency responding, such as the Sanitation Department or the NYPD, the location of the caller, and the problem described by the caller. By analyzing these features, we aim to employ various models to predict the time it takes to resolve these service requests. Linear regression will serve as our baseline model, while decision trees and neural networks will be implemented to explore different modeling techniques. This project's objective is to evaluate and identify the most effective model for predicting the resolution time of service requests within New York City's agencies.

## Data Availability Statement

The dataset used in this project, "311 Service Requests from 2010 to Present," is publicly available through the City of New York's official data portal at the following URL: [Link to Dataset](https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9). This dataset provides several variables that could be used as features, including agency, complaint type, descriptor, location type, zip code, and borough. Below, we provide the screenshot of the data set we are using. 


Table 1. A sample from the dataset “311 Service Requests from 2010 to Present”
![Alt text](images/table-data-sample.png "A sample from the dataset “311 Service Requests from 2010 to Present")
Some features, such as agency name and agency, exhibit a linear correlation and can easily be dropped. Location is a critical feature, especially amid concerns that city agencies may service wealthier, more privileged neighborhoods faster and more efficiently than others. Another valuable feature could be the distance from the agency's location to the neighborhood of the request — though this would require more investigation and may not be that predictive, depending on whether the agency has field offices. This feature could be calculated using the request's location (x, y coordinates).  Complaint type could also be valuable, as it might be easier to remove a “Derelict Vehicle” than a “Rodent Infestation.” 

## Citations
City of New York. 311 Service Requests from 2010 to Present. [Data set]. Data source URL: [Link to Dataset](https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9)
