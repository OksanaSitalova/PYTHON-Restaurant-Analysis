# Restaurant Data Analysis (SQLite, Pandas, Visualization)

## Overview
This project covers the full cycle of exploratory data analysis (EDA) on a restaurant order database using SQLite.  
The goal is to identify the most popular and profitable dishes, analyze peak operating hours, and examine revenue distribution across weekdays to support business decision-making.

## Data Source
The `db_new.sqlite3` database contains three main tables:

- `restaurant_orderitem` — items within each order;
- `restaurant_order` — general order information (including date and time);
- `restaurant_product` — product catalog with names and prices.

## Analysis Workflow

### 1. Merging Tables
- Joined the three tables using an SQL query  
- Exported the result to a `.csv` file  
- Optimized data types to reduce memory usage

### 2. Top 10 Products by Sales Volume
- Created a pie chart of the most frequently ordered items  
- Top-selling products: **Plain Papadum**, **Pilau Rice**, **Plain Naan**

### 3. Top 10 Products by Revenue
- Calculated revenue as: `price × quantity`  
- Highest-earning dish: **Chicken Tikka Masala** (~17.5% of total top-10 revenue)  
- Other key contributors: **Pilau Rice**, **Garlic Naan**

### 4. Revenue by Hour of the Day
- Peak hours: **17:00 – 19:00**  
- Sharp decline in sales after **21:00**  
- Low activity before **11:00** — ideal time for preparation and staff training

### 5. Revenue by Day of the Week
- Most profitable days: **Saturday**, **Friday**, **Sunday**  
- Weakest days: **Monday** and **Tuesday** — suitable for maintenance or promotional campaigns

### 6. Heatmap: Day × Hour
- Visualized order activity using a heatmap  
- Highest intensity: **Friday, Saturday, Sunday evenings**

## Technologies Used
- **SQLite** — Data storage
- **Pandas** — Data manipulation and aggregation
- **Matplotlib**, **Seaborn** — Visualization
- **Jupyter Notebook / Google Colab** — Analysis environment

## Business Insights
- Focus operations and marketing on **Friday to Sunday**, between **17:00–19:00**
- Ensure availability of top dishes like **Chicken Tikka Masala**
- Test promotions on **Tuesdays**, the weakest day
- Use mornings for **preparation**, **training**, or **new menu testing**

## Project Structure
├── db_new.sqlite3 # Original database

├── restaurant.csv # Merged dataset

├── restaurant_analysis.ipynb # Jupyter notebook with analysis

├── README.md # Documentation


## Project Status
✅ Completed

### Potential Extensions
- Sales forecasting  
- Customer segmentation  
- Lifetime Value (LTV) estimation or seasonality analysis

