# Coursera_Capstone
This repository will contain assignment information on the capstone. 

Seattle Car Accident Severity

# Introduction: 

For the capstone project, we want to analyze the accident “severity” in of how bad an accident impacts in the city of Seattle and how to prevent future accidents. The data was collected by Seattle SPOT Traffic Management Division which  dataset is updated weekly and is from 2004 to present. It contains information such as severity code, location, weather, road conditions, collusion types , address type, speeding, many other attributes.

# Background:

Death and injuries caused by road collisions leave a long-lasting impact on millions across the world. In Seattle, 20 people’s lives are lost each year on average, and another 150 people are hospitalized with severe injuries from traffic crashes. Every one of these deaths and serious injuries affect not just the people directly involved but their family, friends, and communities. These accidents can be can prevented.  

The Seattle government is attempting to prevent avoidable car accidents. In most cases, accidents occur due to not paying enough attention while driving, abusing drugs and alcohol or speeding are the main causes of occurring accidents that can be prevented by enacting harsher regulations. Other reasons they play a part are issues with visibility caused by the weather and road conditions. 

The target audience of the project is local Seattle government, police, rescue groups, and car insurance companies. The model and its results are going to provide some advice for the target audience to make insightful decisions for reducing the number of accidents and injuries for the city of Seattle.

# Data

There are 194,673 observations and 38 variables in this data set. Since we would like to identify the factors that cause the accident and the level of severity, we will use SEVERITYCODE as our dependent variable Y, and try different combinations of independent variables X to get the result. Since the observations are large, we may need to remove the missing values and delete any unrelated columns first. Then we can select the factor which may have more impact on the accidents, such as address type, weather, road condition, and light condition.

The target Data to be predicted under (SEVERITYCODE 1-prop damage 2-injury) label.

*Severity codes are as follows:*

0: Little to no Probability (Clear Conditions)

1: Very Low Probability — Chance or Property Damage

2: Low Probability — Chance of Injury

3: Mild Probability — Chance of Serious Injury

4: High Probability — Chance of Fatality

*Other important variables include:*

• ADDRTYPE: Collision address type: Alley, Block, Intersection

• LOCATION: Description of the general location of the collision

• PERSONCOUNT: The total number of people involved in the collision helps identify severity involved

• PEDCOUNT: The number of pedestrians involved in the collision helps identify severity involved

• PEDCYLCOUNT: The number of bicycles involved in the collision helps identify severity involved

• VEHCOUNT: The number of vehicles involved in the collision identify severity involved

• JUNCTIONTYPE: Category of junction at which collision took place helps identify where most collisions occur

• WEATHER: A description of the weather conditions during the time of the collision

• ROADCOND: The condition of the road during the collision

• LIGHTCOND: The light conditions during the collision

• SPEEDING: Whether or not speeding was a factor in the collision (Y/N)

• SEGLANEKEY: A key for the lane segment in which the collision occurred

• CROSSWALKKEY: A key for the crosswalk at which the collision occurred

• HITPARKEDCAR: Whether or not the collision involved hitting a parked car

Furthermore, because of the existence of null values in some records, the data needs to be preprocessed before any further processing.

# Preprocessing Data

In order to prepare the data, the SEVERITYCODE data was balanced and resampled. Non-relevant columns were dropped,  missing values were corrected and encoding of the data were used to clean-up the data for attributes "WEATHER", "ROADCOND", and "LIGHTCOND".

# Methodology

The methodology used emcompasses Github respository, running Jupyter notebook from the IBM watson studio. Using packages such as Pandas, NumPy, and Sklearn to preprocess data and build machine learning models. 

After reviewing the data, Exploratory Data Analysis was used to focus efforts on important features to predict the severity of an accident in Seattle. The features include "WEATHER", "ROADCOND", and "LIGHTCOND" with SEVERITYCODE being the target variable. 

Using Predictive Modeling and Evaluation, decided on using three Machine Learning models with test and train data: KNN (K-Nearest Neighbors), Decision Tree and Linear Regression.

# Results
