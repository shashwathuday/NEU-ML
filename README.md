### README: Airbnb Data Analysis and Feature Engineering

---

# Airbnb Data Analysis and Feature Engineering

This repository contains a project focused on **Exploratory Data Analysis (EDA)** and **Feature Engineering** using Airbnb Listings and Reviews data from selected cities. The goal is to extract meaningful insights that can help optimize property listings and improve guest satisfaction on the Airbnb platform.

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

This project uses Airbnb data to explore trends and patterns in property listings and guest reviews. The objective is to perform EDA on the **Listings dataset** and engineer features from the **Reviews dataset** to gain insights that can enhance the Airbnb platform, such as identifying pricing trends, guest satisfaction factors, and neighborhood comparisons.

---

## Project Structure

```
├── dataset/
│   ├── listings_city1.csv      # Listings data for a specific city
│   ├── README.md               # Describes the data sources and structure
├── action/
│   ├── paris/                  # Directory for specific city (Paris) actions
│   │   ├── pre_requisites      # Pre-processing steps for the dataset
│   │   ├── tasks               # Tasks such as EDA, feature engineering, and results
├── README.md                   # This README file
└── requirements.txt            # Required Python packages
```

- **`dataset/`**: Contains the listings data and a `README.md` detailing the dataset structure and source.
- **`action/`**: Organized by city (e.g., Paris). Each city contains directories for specific steps, such as data preprocessing (`pre_requisites`) and task execution (`tasks`).
- **`README.md`**: Documentation for the entire project.
- **`requirements.txt`**: File for installing the required dependencies.

---

## Datasets

- **Listings dataset**: Contains property details such as `price`, `minimum_nights`, `availability`, and `review_scores_rating`.
- **Reviews dataset**: Includes guest comments, which are analyzed to understand customer satisfaction.

The data is available for download at [Inside Airbnb](http://insideairbnb.com/get-the-data.html).

---

## Tasks

1. **Descriptive Statistics**: Summarize key numerical features such as price, minimum nights, and review scores.
2. **Distribution Analysis**: Plot histograms to understand the distribution of numerical features.
3. **Correlation Analysis**: Explore relationships between variables like price and guest ratings.
4. **Price Analysis**: Examine pricing trends across neighborhoods and room types.
5. **Neighborhood Comparison**: Compare guest satisfaction across different neighborhoods.
6. **Outlier Detection**: Detect outliers in features like price and review scores.
7. **Text Length Feature**: Create a feature based on review text length and analyze its correlation with ratings.
8. **Keyword Extraction**: Identify specific keywords in reviews (e.g., "clean", "noisy") and create new features.

---

## Approach

- **EDA**: Focus on summarizing, visualizing, and understanding the distributions and relationships between different numerical features in the Listings dataset.
- **Feature Engineering**: Extract sentiment, keyword presence, and review text length from the Reviews dataset to predict guest satisfaction.

### Tools Used:
- **Pandas**: For data manipulation.
- **Seaborn & Matplotlib**: For data visualization.
- **NLTK & TextBlob**: For sentiment analysis and keyword extraction from reviews.

---

## Results

Key findings include:
- **Price Trends**: Certain neighborhoods are consistently more expensive.
- **Guest Satisfaction**: Positive keywords (e.g., "clean") and longer reviews are associated with higher guest ratings.
- **Sentiment Analysis**: Reviews with positive sentiment tend to have higher scores.

Visualizations and detailed insights can be found in the **tasks** folder under each city's directory.

---

## Requirements

To run the code, install the required dependencies:

```bash
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

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/airbnb-data-analysis.git
   ```

2. **Download the data**:
   Place the listings and reviews datasets in the `dataset/` folder.

3. **Run the analysis**:
   Go to the `action/` folder for each city and execute the Jupyter notebooks to perform the analysis.

---

## Assumptions

- Reviews reflect real guest experiences.
- Data quality issues (e.g., missing values) are handled with simple imputation or removal of invalid records.
- Keywords extracted from the reviews directly affect guest satisfaction.

---

## Limitations

- The analysis is limited to five cities, which may not represent trends in other regions.
- The sentiment analysis and keyword extraction may not capture the full context of reviews.
- Outliers in pricing and review scores may distort the overall analysis in some cities.

---

## Conclusion

This project provides valuable insights into Airbnb listings and guest reviews. Feature engineering on reviews, combined with EDA on listings, helps identify key factors that influence guest satisfaction and pricing trends. These insights can be leveraged by hosts and the Airbnb platform to improve service offerings.

---

### License

This project is licensed under the MIT License. Feel free to use, modify, and distribute as needed.

--- 

Feel free to reach out with any questions or suggestions!
