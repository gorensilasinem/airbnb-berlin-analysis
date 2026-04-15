Airbnb Berlin Price Analysis

Project Objective

The goal of this project is to analyze Airbnb listing data from Berlin and identify the key factors that influence price.  
The project includes data cleaning, exploratory data analysis (EDA), visualization, and predictive modeling.



## Dataset

Source: Inside Airbnb

The dataset contains detailed information about Airbnb listings in Berlin, including:

- price
- property type
- room type
- number of bedrooms
- number of bathrooms
- accommodates capacity
- neighbourhood
- availability
- review scores



## Data Cleaning

Key cleaning steps:

- Converted price column from string to numeric
- Removed extreme outliers (prices above 500€)
- Handled missing values in bedrooms, beds and bathrooms using median imputation
- Removed irrelevant columns such as URLs
- Encoded categorical variables using one-hot encoding



## Exploratory Data Analysis

Key findings:

- Most listings are priced between 50€ and 160€ per night
- Entire homes/apartments are more expensive than private rooms
- Central neighbourhoods tend to have higher prices
- Price distribution is right-skewed due to luxury listings



## Modeling

Two models were tested:

### Linear Regression
R² score: 0.41

### Random Forest Regressor
R² score: 0.42

Random Forest slightly outperformed Linear Regression, suggesting non-linear relationships in the data.



## Key Insights

- Property size is the strongest predictor of price
- Bedrooms, accommodates capacity and bathrooms have the highest feature importance
- Location also plays an important role
- Central neighbourhoods such as Alexanderplatz and Prenzlauer Berg show higher prices
- Price prediction has moderate difficulty due to qualitative factors not included in the dataset



## Tools Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook