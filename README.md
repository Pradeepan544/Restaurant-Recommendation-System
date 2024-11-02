# 🍽️ Restaurant Recommendation System

## 📚 Overview
Welcome to the Restaurant Recommendation System! This project leverages data from the Bengaluru Zomato dataset to provide personalized dining recommendations. With over 60,000 entries, this dataset captures the vibrant culinary scene of Bengaluru, and our system aims to simplify your dining choices.

## 🌟 Key Features
* Dataset: Utilizes the comprehensive Zomato dataset for Bengaluru restaurants.
* Data Preprocessing: Cleaned and preprocessed the dataset using Excel and Pandas to enhance data quality and usability.
* Exploratory Data Analysis (EDA): Conducted thorough EDA to uncover insights and trends in restaurant ratings, cuisines, and dining costs.
* Efficiency: Used only 40% of the dataset to ensure optimal performance without compromising the quality of recommendations.

## Dataset
The Dataset used for the recommender system is taken from Kaggle: Zomato Bangalore Dataset. Users can refer the link to download use it: https://www.kaggle.com/datasets/absin7/zomato-bangalore-dataset/data

## 🔍 Data Preprocessing
* Data preprocessing is a crucial step in any data-driven project. Here’s how I approached it:
* Initial Cleaning: Removed duplicates, handled missing values, and ensured data consistency.
* Feature Selection: Focused on key attributes such as ratings, votes, cuisines, and location for meaningful recommendations.
* Sample Data: Due to the large dataset size, I selected a manageable subset (40%) for analysis and modeling.

## 📊 Exploratory Data Analysis (EDA)
The EDA phase revealed valuable insights
### Overall Summary from EDA
#### Summary of Descriptive Statistics
Ratings Distribution:
* Over 75% of restaurants have ratings greater than 3 stars, with the maximum rating reaching 4.9 stars.
* Some restaurants appear to have unusually high ratings, such as one with 16,832 votes, which raises questions about data accuracy or potential outliers.

Votes Analysis:
* The maximum number of votes for a restaurant is 16,832, indicating popularity, but this can skew recommendations, as restaurants with many votes may dominate visibility.
* A positive correlation exists between ratings and popularity, suggesting that higher-rated restaurants tend to receive more votes.

Cost Insights:
* The average cost for two people is 555, with a wide range: a minimum of 40 and a maximum of 4,500.
* Certain areas like MG Road, Koramangala 5th Block, Residency Road, and Lavelle Road show both high median costs and significant variability, indicating upscale dining options.
* Conversely, areas such as Jakkur and Hosur Road feature lower median costs and less variability, suggesting more affordable dining choices.

Location and Cost Correlation:
* Dining costs generally increase in central or upscale locations, while suburban or less commercialized areas (e.g., Hennur) maintain lower and more consistent costs.
* There’s a strong relationship between location and dining costs, with specific neighborhoods being associated with certain cuisines.

#### Insights on Cuisine and Location

* Popular Cuisines by Type:
  * North Indian: BTM, Marathahalli, HSR, Whitefield, JP Nagar
  * Chinese: BTM, HSR, Koramangala 5th Block, Marathahalli, Whitefield
  * South Indian: BTM, HSR, Jayanagar, JP Nagar, Marathahalli
  * Fast Food: BTM, HSR, Koramangala 5th Block, Jayanagar, Indiranagar
  * Biryani: BTM, HSR, Whitefield, Marathahalli, Bellandur
  * Continental: Koramangala 5th Block, Indiranagar, JP Nagar, HSR, BTM
  * Desserts: Koramangala 5th Block, Jayanagar, BTM, Whitefield, Indiranagar

* Restaurant Popularity:
  * The most popular restaurants based on votes include:
  * Onesta: 373,002 votes
  * Hammered: 362,399 votes
  * Empire Restaurant: 355,211 votes
  * Truffles: 309,580 votes
  * Green Theory: 299,096 votes
  * Top-Rated Restaurants:

* The highest-rated restaurants include:
  * Asia Kitchen By Mainland China: 4.9 stars
  * Byg Brewski Brewing Company: 4.9 stars
  * Punjab Grill: 4.875 stars

#### General Observations

* Dining Trends: The data indicates that certain cuisines are consistently associated with specific locations, suggesting that restaurant type preferences vary by neighborhood. BTM and HSR are repeatedly listed as top locations across multiple cuisines, indicating their popularity or centrality in the dining landscape.
* Cost Implications: Higher dining costs are likely correlated with more upscale areas, and recommendations should consider both popularity (votes) and quality (ratings) to provide a balanced view.
