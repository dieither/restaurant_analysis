# Restaurant Data Analysis

An in-depth analysis of restaurant order data to identify sales patterns, product performance, and menu optimization opportunities.

## Project Overview

This project analyzes a restaurant's sales data to uncover insights about:
- Most popular products by quantity and revenue
- Time-based revenue patterns (hourly, daily, monthly, yearly)
- Common dish combinations that could be leveraged for promotions
- Menu optimization opportunities

## Table of Contents
- [Setup](#setup)
- [Data Structure](#data-structure)
- [Key Features](#key-features)
- [Main Findings](#main-findings)
- [Visualizations](#visualizations)
- [Future Work](#future-work)

## Setup

### Prerequisites
- Python 3.x
- SQLite3
- Required Python packages:
  ```
  pandas
  numpy
  matplotlib
  seaborn
  ```

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/restaurant-analysis.git
   cd restaurant-analysis
   ```

2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the analysis:
   ```bash
   python restaurant_analysis.py
   ```

## Data Structure

The analysis uses three main database tables:
- `restaurant_orderitem`: Contains order items, quantities, and links to orders and products (74,818 rows)
- `restaurant_product`: Contains product names and prices (248 rows)
- `restaurant_order`: Contains order timestamps (13,397 rows)

## Key Features

- **Database Exploration**: Comprehensive analysis of relational data structure
- **Sales Performance Analysis**: Identification of top-performing products
- **Temporal Analysis**: Revenue patterns by hour, day, month, and year
- **Combination Analysis**: Discovery of frequently paired menu items
- **Visualization**: Various charts and graphs to represent findings

## Main Findings

### Product Performance
- Higher-priced main dishes (e.g., Chicken Tikka Masala) generate the most revenue
- Low-cost sides (e.g., Plain Papadum) are ordered most frequently
- Sales volume doesn't always correlate with profit contribution

### Revenue Patterns
- **Peak Hours**: 17:00, 18:00, and 20:00, with highest revenue at 18:00
- **Peak Days**: Friday and Saturday, with Sunday also performing well
- **Seasonal Trends**: Peaks in May–July and December
- **Annual Trends**: Growth from 2016–2018, decline in 2019

### Dish Combinations
- Identified top 10 most common dish pairings
- Each order contains approximately 5.58 items on average
- Potential for combo meal promotions based on frequent pairings

## Visualizations

The analysis includes various visualizations:
- Pie charts for top products by quantity and revenue
- Bar charts for temporal analysis (hourly, daily, monthly, yearly)
- Bar charts for common dish combinations

## Future Work

- Implement customer segmentation analysis
- Develop a recommendation system for menu items
- Create a dashboard for real-time sales monitoring
- Analyze pricing elasticity to optimize menu pricing
