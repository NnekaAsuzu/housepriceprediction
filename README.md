# House Price Prediction Project

## Overview
This project aims to predict house prices based on various features using a dataset containing information such as number of rooms, price, property type, seller, date sold, distance from CBD, region name, property count, bedrooms, bathrooms, carspots, land size, building size, year built, council area, latitude, and longitude.

## Dataset
The dataset used for this project includes the following columns:
- Rooms: Number of rooms
- Price: Price in Australian dollars
- Method: S - property sold; SP - property sold prior; PI - property passed in; PN - sold prior not disclosed; SN - sold not disclosed; NB - no bid; VB - vendor bid; W - withdrawn prior to auction; SA - sold after auction; SS - sold after auction price not disclosed. N/A - price or highest bid not available.
- Type: br - bedroom(s); h - house,cottage,villa, semi,terrace; u - unit, duplex; t - townhouse; dev site - development site; o res - other residential.
- SellerG: Real Estate Agent
- Date: Date sold
- Distance: Distance from CBD in Kilometres
- Regionname: General Region (West, North West, North, North east …etc)
- Propertycount: Number of properties that exist in the suburb.
- Bedroom2 : Scraped # of Bedrooms (from different source)
- Bathroom: Number of Bathrooms
- Car: Number of carspots
- Landsize: Land Size in Metres
- BuildingArea: Building Size in Metres
- YearBuilt: Year the house was built
- CouncilArea: Governing council for the area
- Lattitude: Latitude
- Longtitude: Longitude

## Methodology
The methodology used for prediction includes:
1. Data Pre-processing and Cleaning: Understanding the data, dropping irrelevant columns, checking for duplicates, handling null values, and converting mixed data types.
2. Exploratory Data Analysis (EDA): Investigating the correlation between features, exploring distribution of property types and prices, and examining the correlation between region names and property prices.
3. Feature Engineering: Creating new features such as datetime features, house prices in CAD, age of the house, total rooms, price per property count, and days on market.
4. Model Selection: After comparing different regression models, the Random Forest Regressor was selected based on its superior performance, robustness, and ability to handle non-linear relationships and complex patterns in the data.
5. Model Evaluation: The model was evaluated using k-fold cross-validation, with the Random Forest Regressor outperforming other models with an R2 score of 0.4710.

## Results
The Random Forest Regressor demonstrated the highest R2 score (0.4499) among the evaluated models, indicating superior predictive performance. The model exhibited less error in predicting the target variable compared to Linear Regression and Decision Tree Regressor.

## Future Improvements
Future improvements to the project could include:
- Fine-tuning the Random Forest Regressor model to further improve its performance.
- Incorporating additional features or datasets to enhance the model's predictive capabilities.
- Experimenting with different machine learning algorithms to see if better performance can be achieved.
- Conducting more in-depth analysis on the most important features to gain deeper insights into their impact on property prices.

## Contributor(s)
- Nneka Asuzu
- [Your GitHub Profile](https://github.com/NnekaAsuzu)

## Setup
To run the project locally, follow these steps:
1. Clone the repository: `git clone https://github.com/NnekaAsuzu/house-price-prediction.git`
2. Navigate to the project directory: `cd house-price-prediction`
3. Install dependencies: `pip install -r requirements.txt`
