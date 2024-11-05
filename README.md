# NYC Airbnb 2019 Data Analysis

This project provides an exploratory data analysis (EDA) on Airbnb listings in New York City, using the 2019 dataset. The analysis focuses on data cleaning, transformation, and visualization to extract insights about room types, pricing trends, host activity, and more.

## Table of Contents

1. [Dataset Information](#dataset-information)
2. [Project Overview](#project-overview)
3. [Data Preprocessing](#data-preprocessing)
4. [Analysis & Insights](#analysis--insights)
5. [Conclusion](#conclusion)
6. [How to Use](#how-to-use)

---

## Dataset Information

- **Source**: [Airbnb NYC 2019 Dataset](https://www.kaggle.com/dgomonov/new-york-city-airbnb-open-data)
- **Data Fields**:
  - `id`, `name`, `host_id`, `host_name`
  - `neighbourhood_group`, `neighbourhood`, `latitude`, `longitude`
  - `room_type`, `price`, `minimum_nights`
  - `number_of_reviews`, `last_review`, `reviews_per_month`
  - `calculated_host_listings_count`, `availability_365`

---

## Project Overview

The project aims to:
- Clean and preprocess the dataset, handling missing values and duplicates.
- Perform descriptive and correlation analysis on various data fields.
- Visualize data distributions and relationships between different features.
- Identify trends based on room types, neighborhoods, and host activity.

## Data Preprocessing

1. **Handling Missing Values**:
   - `name` and `host_name` fields are filled with "Unknown" to retain as much data as possible.
   - `last_review` is replaced with "No review" and `reviews_per_month` with `0` for missing values.
  
2. **Formatting**:
   - Setting float precision to two decimal places for better readability.

3. **Removing Duplicates**:
   - Duplicate rows, if any, are removed to ensure unique entries.

## Analysis & Insights

1. **Room Type Distribution**:
   - Analysis of the frequency of different room types, such as entire homes, private rooms, and shared rooms.

2. **Pricing Trends**:
   - Comparison of average prices by room type and neighborhood.

3. **Listings Below Average Price**:
   - Calculation of the percentage of listings that are priced below the average listing price.

4. **Review Insights**:
   - Average number of reviews per listing and analysis of the listing with the highest number of reviews.
   - Correlation analysis between `price` and `number_of_reviews`.

5. **Host Activity**:
   - Identification of the host with the highest number of listings.
   - Average listings per host and correlation between listings and reviews.

6. **Availability**:
   - Analysis of average availability across listings and its correlation with price.

7. **Minimum Night Requirements**:
   - Average minimum nights required based on room type and neighborhood.

## Conclusion

This analysis provided insights into the NYC Airbnb market, highlighting:
- The most common and affordable room types.
- Neighborhoods with high and low average prices.
- Hosts with a significant presence and trends in availability across listings.

## How to Use

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/NYC-Airbnb-Analysis.git
   cd NYC-Airbnb-Analysis
Install required packages:

This analysis uses pandas and matplotlib.
Install dependencies with:
bash
Copy code
pip install pandas matplotlib
Run the Analysis:

Open and run the script in Jupyter Notebook or directly in your preferred IDE.
Acknowledgements
Airbnb Open Data for making this dataset available.
Kaggle for hosting the dataset.
