# FoodHub Order Analysis (Delivery App Simulation)

Exploratory data analysis of a New York food delivery aggregator to uncover order patterns, delivery performance, and customer rating behavior; with actionable business recommendations.

## Overview

FoodHub is a food aggregator app that connects customers with restaurants across New York City. This project analyzes 1,898 orders across 9 variables to help the business understand demand patterns, delivery efficiency, and customer satisfaction — ultimately informing decisions around restaurant partnerships, staffing, and marketing.

## Dataset

`foodhub_order.csv` — 1,898 orders with the following key variables:

- `restaurant_name`, `cuisine_type` — restaurant and food category
- `cost_of_the_order` — order value in USD
- `day_of_the_week` — weekday vs weekend
- `rating` — customer rating (or "Not given")
- `food_preparation_time`, `delivery_time` — time in minutes

## Analysis Highlights

- Order volume is heavily concentrated among a small subset of restaurants, with many receiving only a few orders
- The majority of ratings are "Not given", limiting feedback signal quality
- Average delivery time is longer on weekdays (28.34 min) vs weekends (22.48 min)
- 200 orders (~10.5%) exceed 60 minutes total time from order to delivery
- Spanish cuisine has the highest average ratings; Vietnamese the lowest
- Revenue analysis using a tiered commission model (25% on orders >$20, 15% on $5-$20)

## Recommendations

- Incentivize customers to leave ratings to improve feedback data quality
- Investigate weekend delivery delays - likely driven by traffic and higher order volume
- Prioritize partnerships with high-demand, high-rated cuisine types
- Focus marketing on the long tail of underperforming restaurants or consolidate toward proven performers

## Tech Stack

Python, pandas, NumPy, matplotlib, seaborn
