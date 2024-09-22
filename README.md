### README: Airbnb Data Analysis and Feature Engineering Project

---

# Airbnb Data Analysis and Feature Engineering

This project focuses on **Exploratory Data Analysis (EDA)** and **Feature Engineering** on Airbnb Listings and Reviews datasets from five selected cities. The goal is to derive actionable insights to improve Airbnb's platform, optimize property listings, and enhance guest satisfaction.

---

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Datasets](#datasets)
- [Tasks](#tasks)
- [Approach](#approach)
- [Results](#results)
- [Requirements](#requirements)
- [Usage](#usage)
- [Assumptions](#assumptions)
- [Limitations](#limitations)
- [Conclusion](#conclusion)

---

## Introduction

This project uses data from Airbnb to analyze property listings and reviews for five cities. The objective is to gain insights into pricing, guest satisfaction, and trends across different neighborhoods and room types. In addition, feature engineering on the review text is performed to predict customer satisfaction using text sentiment and keyword extraction.

---
## Project Structure
 
```
├── dataset/
│   ├── listings_city1.csv
│   ├── README.md
├── action/
│   ├── paris
│       ├── pre_requisites
|       ├── tasks
├── README.md
└── requirements.txt
```
 
- `dataset/`: Contains Airbnb Listings and Reviews datasets for the selected cities.
- `notebooks/`: Contains Jupyter notebooks for EDA and feature engineering tasks.
- `scripts/`: Contains reusable Python functions for EDA and feature engineering.
- `results/`: Contains visualizations and data files generated from the analysis.
 
---

## Datasets

- **Listings dataset**: Includes detailed information about each Airbnb property, such as price, location, availability, and host details.
- **Reviews dataset**: Contains guest comments on various properties, reflecting their experiences.

The data is available from the [Inside Airbnb website](http://insideairbnb.com/get-the-data.html).

---

## Tasks

1. **Descriptive Statistics**: Calculate summary statistics for features such as `price`, `minimum_nights`, and `review_scores_rating`.
2. **Distribution Analysis**: Visualize the distribution of key numerical features.
3. **Correlation Analysis**: Analyze correlations between variables like `price`, `availability_365`, and `review_scores_rating`.
4. **Price Analysis**: Analyze the distribution of prices across neighborhoods and room types.
5. **Neighborhood Comparison**: Compare average `review_scores_rating` across neighborhoods.
6. **Outlier Detection**: Detect outliers in features such as price and review scores.
7. **Text Length Analysis**: Create a new feature to measure review text length.
8. **Keyword Extraction**: Count occurrences of specific keywords in reviews, such as "clean" or "noisy."

---

## Approach

### 1. **Exploratory Data Analysis (EDA)**:
   - Summary statistics of the listings.
   - Histograms and density plots for distributions.
   - Correlation matrix to find relationships between variables.
   - Outlier detection and visualization.

### 2. **Feature Engineering**:
   - Sentiment analysis of reviews using `TextBlob` and `VADER`.
   - Extraction of keywords to create binary features.
   - Analysis of the impact of these features on guest satisfaction.

### 3. **Visualization**:
   - Generated visual insights such as histograms for pricing, bar plots for keyword occurrences, and heatmaps for correlation analysis.

---

## Results

### Key Insights:

- **Price Distribution**: Certain neighborhoods are more expensive, and outliers exist with extremely high prices.
- **Guest Satisfaction**: Keywords like "clean" and "comfortable" correlate with higher ratings, while "noisy" correlates with lower ratings.
- **Sentiment Analysis**: Positive sentiment in reviews tends to correlate with higher guest ratings, indicating text sentiment is a good predictor of customer satisfaction.
  
Visuals and data files can be found in the `results/` directory.

---

## Requirements

To run the code, the following Python libraries are required:

```bash
# Install required packages
pip install -r requirements.txt
```

Contents of `requirements.txt`:

```
pandas
numpy
matplotlib
seaborn
nltk
textblob
swifter
scikit-learn
```

---

## Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/airbnb-data-analysis.git
   ```

2. Place the Airbnb data files in the `dataset/` folder.

3. Run the Jupyter notebooks in `tasks/` for EDA and feature engineering.


---

## Assumptions

- Sentiment scores and keyword presence correlate strongly with guest satisfaction.
- Listings and review datasets accurately reflect Airbnb properties and guest experiences.
- Missing values in numerical features are imputed where necessary.

---

## Limitations

- The analysis is limited to only five cities, which may not generalize globally.
- Some reviews may be biased or lack sufficient details to gauge guest satisfaction accurately.
- The analysis of keywords is case-insensitive and may not capture nuanced meanings.

---

## Conclusion

This project provided meaningful insights into Airbnb property listings and guest reviews. Through the analysis of pricing, guest satisfaction, and keyword occurrences in reviews, we identified actionable factors that can help improve the Airbnb platform. Sentiment analysis and keyword extraction proved valuable in predicting customer satisfaction.

---

Feel free to reach out with any questions or suggestions. Thank you for exploring this project!

--- 

### License

This project is licensed under the MIT License.
