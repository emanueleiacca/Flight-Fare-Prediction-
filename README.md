# Kaggle Flight Fare Prediction Project
This README provides an overview of a Kaggle project that aims to predict flight fares. Below, you'll find details about the project's objectives, dataset, data preprocessing, exploratory data analysis (EDA), and the machine learning model used.

# Objective
The objective of this project is to develop a machine learning model that can accurately predict the fares of flights based on various features such as departure time, arrival time, airline, route, and more. Accurate flight fare prediction can be valuable for both travelers looking to plan their trips and airlines for pricing strategies.

# Dataset
The dataset used for this project is the "Flight Fare Prediction" dataset from Kaggle. It includes features such as:

Date of Journey
Departure Time
Arrival Time
Total Stops
Additional Info
Price (target variable)
Duration
Airline
Source
Destination
Route (with multiple segments)
## Data Preprocessing
The data preprocessing steps performed on the dataset include:

Handling missing values.
Cleaning and standardizing airline names.
Standardizing destination names.
Mapping the "Total Stops" column to numerical values.
Handling duration data by converting it to hours and minutes.
Creating new columns for each segment of the route.
Creating dummy variables for categorical columns using one-hot encoding.
Exploratory Data Analysis (EDA)
## The EDA phase involved the following analyses:

Correlation analysis to identify relationships between numerical features.
Distribution of flight prices.
Box plots to identify outliers in flight prices.
Analysis of airline distribution.
Analysis of the distribution of flights with different numbers of stops.
Visualizing the relationship between airline and the number of stops.
Scatter plots to explore the relationship between total stops, duration, and price.
Analysis of price variation based on source and destination cities.
Analysis of the busiest month for flights.
Box plots showing price variation based on the source and destination cities.
## Model Building
Several machine learning models were built and evaluated for this project. The models tested include:

Random Forest Regressor
Logistic Regression
K-Nearest Neighbors (KNN) Regressor
Light Gradient Boosting Machine (LightGBM) Regressor
The best-performing model was the LightGBM Regressor, which achieved an R-squared score of approximately 0.826. The hyperparameters of the LightGBM model were fine-tuned using GridSearchCV to optimize its performance, the final R-squared score is 0.855.

# Conclusion
In conclusion, this Kaggle project successfully developed a machine learning model that can predict flight fares with a high degree of accuracy. The LightGBM Regressor model, after hyperparameter tuning, demonstrated the best performance in predicting flight fares(the final R-squared is one of the best according to other user's results). Accurate flight fare prediction can benefit both travelers and airlines in making informed decisions related to pricing and planning travel.
