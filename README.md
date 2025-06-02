Restaurant Data Analysis (SQLite + Pandas + Visualization)
Project Overview
This project is a full-cycle exploratory data analysis (EDA) of a restaurant’s order database (db_new.sqlite3) using SQLite, pandas, matplotlib, and seaborn.
The goal is to identify the most popular and profitable products, peak business hours, and revenue patterns by day to derive practical business insights.

Data Source
The SQLite database contains three main tables:

restaurant_orderitem – individual items in orders;

restaurant_order – general order information (with timestamps);

restaurant_product – product catalog with names and prices.

Key Analysis Steps
Step 1: Data extraction and merging
Joined all three tables into a single DataFrame via SQL.

Exported to CSV and optimized data types to reduce memory usage.

Step 2: Top-selling products by quantity
Pie chart of top 10 most frequently ordered items.

Plain Papadum, Pilau Rice, and Plain Naan are the most ordered.

Step 3: Most profitable products by revenue
Chicken Tikka Masala generates the highest revenue (~17.5%).

Several side dishes (e.g., Pilau Rice, Garlic Naan) also contribute significantly.

Step 4: Revenue by hour
Revenue peaks during 5 PM – 7 PM, especially on weekends.

Low traffic before lunch; consider using that time for prep or training.

Step 5: Revenue by weekday
Saturday, Friday, and Sunday are the most profitable.

Monday and Tuesday are the weakest — ideal for maintenance or promotional testing.

Step 6: Heatmap (hour × weekday)
Visualized order patterns by hour and day.

Highlighted key time slots to reinforce with staff and advertising.

Tools & Technologies
SQLite – for raw data extraction

pandas – data wrangling and aggregation

matplotlib, seaborn – visualizations (pie, bar, heatmap)

Jupyter Notebook / Google Colab – analysis environment

Business Insights
Focus marketing and operations on Friday–Sunday, 5 PM–7 PM

Ensure top products (e.g., Chicken Tikka Masala) are always available

Test Tuesday promotions to boost traffic on slowest days

Use early mornings (before 11 AM) for kitchen prep, training, or new menu testing

Project Structure
bash
Copy
Edit
├── db_new.sqlite3             # Source database
├── restaurant.csv             # Cleaned and joined data
├── restaurant_analysis.ipynb  # Notebook with full analysis
├── README.md                  # Project description
Status: Completed
The analysis can be extended with forecasting models, customer segmentation, or LTV analysis.

Optional: requirements.txt
txt
Copy
Edit
pandas
matplotlib
seaborn
sqlite3
