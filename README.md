📊 Overview

A sales performance analysis for a globally operating retail chain. From data cleaning and database setup to multidimensional analysis and interactive dashboard creation, the project identifies key drivers of sales performance and delivers actionable recommendations for optimizing store operations, inventory allocation, and promotional strategies.
🎯 Background & Objectives
Background

A global retail chain with stores across multiple cities lacks a clear understanding of what drives its sales performance:

    Which stores are high-performing and which are underperforming?

    How do sales patterns differ across regions?

    How should product inventory be optimized?

    Do seasonal factors significantly impact revenue?

Without data-driven insights, decisions rely on intuition.
Objectives

    Clean and prepare raw sales data

    Build a relational database to enable complex multidimensional querying

    Identify sales patterns, regional differences, and product performance

    Determine whether date/seasonality impacts sales revenue

    Deliver an interactive dashboard for ongoing monitoring

🛠️ Methodology
Phase	Tools	Key Activities
Data Cleaning	Excel	Handled missing values, removed duplicates, standardized date/number formats
Data Summarization	Excel Pivot Tables	Identified high/low performing stores, regional differences, best/worst selling products
Database Setup	PostgreSQL, pgAdmin	Created database, imported six tables, wrote SQL queries
Multidimensional Analysis	PostgreSQL (ROLLUP, CUBE)	Summarized data along hierarchies, identified trends over time and regions
Statistical Analysis	Excel Regression	Evaluated impact of date on sales revenue (R²≈0, p=0.9367)
Visualization	Excel, Tableau	Line charts, bar charts, sunburst charts, scatter plots
Dashboard	Tableau	Four interactive charts with cross-chart filtering
📊 Data Sources

Six interconnected tables (imported into PostgreSQL):
Table	Description
sales.csv	Daily sales transaction data
product_hierarchy.csv	Product categorization hierarchy
product_names.csv	Product name mappings
store_cities.csv	Store-to-city mapping
store_names.csv	Store names
city_names.csv	City names
🔍 Key Findings
Finding 1: Date Does NOT Significantly Impact Sales Revenue

    R²≈0, p=0.9367 > 0.05 → No seasonal fluctuations

    Date does not explain variation in sales revenue

    Sales are not seasonal

Finding 2: Significant Store Performance Variation

    Some stores have sales significantly below the average

    Wide performance variation across stores

    Underperforming stores need targeted intervention

Finding 3: Product-City Performance Patterns

    Certain products perform exceptionally well in specific cities

    Sunburst chart revealed product concentration in particular regions

    Opportunity for optimized inventory allocation based on local preferences

💡 Recommendations
Recommendation 1: Shift from Seasonal Adjustments to Promotional Activities
Action	Rationale
Reduce seasonal staffing/inventory adjustments	No evidence of seasonal demand
Increase focus on promotional campaign effectiveness	Promotions likely drive revenue
Implement dynamic pricing strategies	Price sensitivity influences sales more than seasonality
Test and measure promotional ROI	Data-driven optimization
Recommendation 2: Targeted Interventions for Underperforming Stores
Action	Rationale
Analyze inventory levels of low-performing stores	Inventory gaps may cause lost sales
Review pricing strategies per location	Local misalignment may impact performance
Evaluate promotional execution	Inconsistent rollout may affect results
Develop city-specific improvement plans	Tailored approach for each store
Recommendation 3: Optimize Regional Inventory Allocation
Action	Rationale
Increase best-selling products in advantageous regions	Leverage proven local demand
Reduce underperforming products in weak regions	Minimize holding costs
Implement regional product mix optimization	Align with local preferences
Use sunburst chart insights for ongoing decisions	Data-driven allocation
📈 Dashboard

Tableau interactive dashboard with four chart types:
Chart Type	Purpose
Line Charts	Track sales trends over time
Bar Charts	Compare store and city performance
Sunburst Chart	Visualize product performance across regions
Scatter Plots	Identify outliers and relationships

Interactivity: Click any store to filter all other charts.
🎓 Key Outcomes

    ✅ Complete data pipeline (raw data → interactive dashboard)

    ✅ Data cleaning (missing values, duplicates, format standardization)

    ✅ PostgreSQL database setup and complex queries

    ✅ ROLLUP/CUBE multidimensional analysis

    ✅ Regression analysis interpretation (R², p-value)

    ✅ Tableau interactive dashboard with cross-filtering

    ✅ Technical findings translated into actionable recommendations

