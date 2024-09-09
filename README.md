# Seoul bike sharing demand prediction : Regression

Currently many big communities have adopted the use of rental bikes to improve transportation comfort. It is crucial to make the rental bikes accessible and available to the general public at the appropriate time since it reduces waiting. Eventually, maintaining a steady supply of rental bikes for the city emerges as a top priority. Predicting how many bikes will be needed each hour to maintain a steady supply of rental bikes is important

![361324002-fc7fce28-bd60-4f3f-bb9b-6dc784e8bf38](https://github.com/user-attachments/assets/bbc62af4-6825-42c4-9070-eedf814c4e3d)

# Problem description
The Seoul bike sharing demand data set contains the count of the number of bikes rented at each hour in the Seoul bike-sharing system and information regarding weather conditions.
The final product will consist of a model that predicts the number of bicycles rented in any given day based on the hour and other weather-related variables such as rainfall and humidity. The system’s predictions are used to guarantee that available bikes will meet the demand for the service.

# Project Summery

This project revolves around predictive modeling for Seoul's bike rental demand, leveraging a dataset comprising 8,760 rows and 14 columns. The workflow adheres to a systematic and formal structure, commencing with data collection and preliminary analysis to ascertain the dataset's fundamental characteristics, including its dimensions and data types. Subsequently, data filtering and cleaning are executed to enhance data quality by eliminating superfluous columns and addressing missing values.

The project progresses to Exploratory Data Analysis (EDA), where insightful visualizations are generated to illuminate relationships between dependent and independent variables. This phase also encompasses an analysis of mean distributions and correlations between columns. With a well-informed understanding of the data, attention shifts towards data preparation, encompassing feature engineering, encoding, and the division of data into training and testing sets.

Data scaling ensures optimal model performance. Model selection is a deliberate process aimed at choosing the most suitable algorithm. Model evaluation employs various metrics to gauge model performance, with hyperparameter tuning employed to enhance accuracy and mitigate overfitting. Ultimately, a comprehensive comparison between test and train data illuminates the model's performance and errors, ensuring a robust predictive model for Seoul's bike rental demand.


# Data Description:

The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.

# Feature Description:

### Date :
Date feature which is str type is needed to convert it into Datetime format DD/MM/YYYY.The new feature extracted from Date are Day, Month and year

### Rented Bike Count :
Number of bike rented which is our Dependent variable according to our problem statement which is int type.

### Hour: 
Hour feature which is in 24 hour format which tells us number bike rented per hour is int type.

### Temperature:
Temperature feature which is in celsius scale(°C) is Float type.

### Humidity(%): 
Feature humidity in air (%) which is int type.

### Wind speed (m/s) :
Wind Speed feature which is in (m/s) is float type.

### Visibility (10m): 
Visibility feature which is in 10m, is int type.

### Dew point temperature(°C): 
Dew point Temperature in (°C) which tells us temperature at the start of the day is Float type.

### Solar Radiation (MJ/m2): 
Solar radiation or UV radiation is Float type.

### Rainfall(mm):
Rainfall feature in mm which indicates 1 mm of rainfall which is equal to 1 litre of water per metre square is Float type.

### Snowfall (cm): 
Snowfall in cm is Float type. Seasons: Season, in this feature four seasons are present in data is str type.

### Holiday:
whether no holiday or holiday can be retrieved from this feature is str type.

### Functioning Day: 
Whether the day is Functioning Day or not can be retrieved from this feature is str type.

### Weekend :
Weekend extracted from Day 1 when the day is Saturday or Sunday while 0 when weekdays
