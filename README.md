# McDonald's Menu Nutritional Analysis

This project involves analyzing the nutritional information of McDonald's menu items. The goal is to clean the dataset, create useful features, and prepare it for further analysis or modeling.

## Dataset

The dataset contains nutritional information for various McDonald's menu items, including:

- Category (e.g., Breakfast, Burgers)
- Item name
- Serving size (including weight in grams)
- Calories and calories from fat
- Fat content and percentage daily values
- Carbohydrates, sugars, protein, vitamins, minerals, etc.

## Data Cleaning and Feature Engineering

Steps performed:

- Checked for missing values and duplicates to ensure data quality
- Extracted the numeric serving size in grams from the 'Serving Size' text field
- Created new features:
  - `calories_per_gram`: Ratio of calories to serving size in grams
  - `sugar_to_fat_ratio`: Ratio of sugars to total fat (with +1 to avoid division by zero)
- Added a binary label `is_healthy` indicating whether an item has less than 400 calories
- Generated descriptive statistics to understand data distributions

## Usage

The cleaned and enriched dataset can be used for:

- Nutritional analysis and visualization
- Predictive modeling of healthy vs unhealthy items
- Recommender systems for healthier meal choices

## Getting Started

1. Load the dataset into a pandas DataFrame
2. Run the data cleaning and feature engineering scripts
3. Explore the enhanced dataset with statistical summaries or visualizations

## Dependencies

- Python 3.x
- pandas
- numpy (optional)
