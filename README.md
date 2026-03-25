# Commercial Flights Delay Analysis & Predictive Modeling

## Project Overview
This project is a comprehensive Business Intelligence dashboard built in Power BI to analyze commercial flight data, identify operational bottlenecks, and predict future delays. It goes beyond descriptive statistics by applying built-in machine learning models to solve complex logistical constraints for the National Aviation Authority (NAA) and provide data-driven flight recommendations for passengers.

## Business Problems Addressed
1. **Customer Satisfaction:** Identifying which factors most severely impact passenger scores and predicting required performance thresholds.
2. **Logistical Optimization:** Determining the most efficient strategy to distribute four new operational supervision offices across New York State airports.
3. **Operational Forecasting:** Anticipating future flight delay volumes and isolating historical anomalies for root-cause investigation.
4. **Consumer Risk Mitigation:** Building a predictive model to recommend specific flights with the lowest probability of delay.

## Methodology & Advanced Analytics
This dashboard heavily utilizes Power BI's advanced analytical and AI features:
* **Linear Regression:** Built a predictive model to determine the exact maximum take-off delay (7.5 minutes) allowable to maintain a passing passenger satisfaction score (>6.1). 
* **K-Means Clustering:** Applied spatial clustering algorithms to evaluate two distinct business strategies (Geographic vs. Passenger Volume).
* **Time-Series Forecasting:** Generated a 30-day predictive forecast with a 95% confidence interval using historical daily delay data.
* **Anomaly Detection:** Configured sensitivity algorithms to isolate ~15 specific dates of extreme operational failure (e.g., a massive spike of 1,209 delays on Dec 26, 2021) for targeted management review.
* **Key Influencer Analysis (Classification):** Deployed ML visuals to identify the primary drivers of delayed flights (departures after 14:00).

## Key Insights & Executive Summary
* **Flight Status vs. Satisfaction:** Flight status is the strongest categorical driver of passenger scores (±1.14 impact), while take-off delay is the strongest continuous factor (-0.62 per 12 mins).
* **Office Placement Strategy:** A Geographic-based clustering strategy proved vastly superior to a Volume-based strategy. Grouping airports by physical proximity successfully met the constraint of <5 airports per office while ensuring realistic travel distances for weekly on-site managerial visits.
* **Seasonality & Forecasting:** Delays follow a highly volatile, repeating weekly cycle with a slight overall downward trend YoY. Early January forecasts predict a temporary spike before normalizing.
* **Flight Recommendations:** Passengers seeking to minimize delay risk should prioritize morning or red-eye flights. The lowest predicted delay probabilities (37%) were found on midnight departures via specific carriers from JFK and ISP.

## Tools & Technologies
* **Power BI:** Data Modeling, DAX, Power Query, AI Visuals (Smart Narratives, Key Influencers, Anomalies, Forecasting), Azure Maps.
* **Analytical Concepts:** Linear Regression, Clustering, Time-Series Analysis, Predictive Probability.

## How to Interact with this Project
1. Download the `.pbix` file from this repository.
2. Open it in Power BI Desktop.
3. Navigate through the bottom tabs to view the descriptive dataset exploration, the predictive machine learning models, and the final executive conclusions.
