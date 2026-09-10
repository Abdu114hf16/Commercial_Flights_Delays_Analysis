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
* **Linear Regression:** Built a predictive model to determine the exact maximum take-off delay allowable to maintain a a specific passing passenger satisfaction score. 
* **K-Means Clustering:** Applied clustering algorithms to evaluate two distinct business strategies (Geographic vs. Passenger Volume).
* **Time-Series Forecasting:** Generated a 30-day predictive forecast with a 95% confidence interval using historical daily delay data.
* **Anomaly Detection:** Configured sensitivity algorithms to isolate specific dates of extreme operational anomalies.
* **Key Influencer Analysis (Classification):** Deployed ML visuals to identify the primary drivers of delayed flights in order to recommend flights with highest 'on time' propability.

## Key Insights & Executive Summary
* **Flight Status vs. Satisfaction:** Flight status is the strongest categorical driver of passenger scores (±1.14 impact), while take-off delay is the strongest continuous factor (-0.62 per 12 mins).
* **Office Placement Strategy:** A Geographic-based clustering strategy proved vastly superior to a Volume-based strategy. Grouping airports by physical proximity successfully met the constraint of <5 airports per office while ensuring realistic travel distances for weekly on-site managerial visits.
* **Seasonality & Forecasting:** Delays follow a highly volatile, repeating weekly cycle with a slight overall downward trend Year-over-Year.
* **Flight Recommendations:** Passengers seeking to minimize delay risk should prioritize morning or red-eye flights. The lowest predicted delay probabilities (37%) were found on midnight departures via specific airports such as JFK and ISP, specific airlines such as United States Airways and Unique Air Lines Inc.

## Report Preview
*(Note: View the full report in the `CDF_Report.pdf` file).*

## Tools & Technologies
* **Power BI:** Data Modeling, DAX, Power Query, AI Visuals (Smart Narratives, Key Influencers, Anomalies, Forecasting), Azure Maps.
* **Analytical Concepts:** Linear Regression, Clustering, Time-Series Analysis, Anomaly detection, Predictive Probability.

## How to Interact with this Project
1. Download the `.pbix` file from this repository.
2. Open it in Power BI Desktop.
3. Navigate through the bottom tabs to view the interactive visuals, the predictive machine learning models, and the final executive conclusions.

## Data source and scope

A full year of commercial departures from **New York airports in 2021**, in
`datasets/`, joined to reference tables describing the airports and airlines.

## About the stakeholder in this project

This is an independent project worked from a **scenario brief**. The brief
supplies a hypothetical aviation authority as the stakeholder the analysis is
addressed to. That authority is part of the exercise: no organisation
commissioned this work, and nothing here was delivered to a client.

## Limitations

- One year, one region. Nothing transfers to another period or network without
  being refit, and **2021 was not an ordinary year for air travel**.
- The influence and regression results are **associations**. The analysis
  identifies what moves together, not what causes what.
- Weather, air-traffic constraints, aircraft rotation and schedule changes are
  not in the dataset, and they are among the largest real drivers of delay.
- The forecast projects the existing weekly pattern forward. It does not
  anticipate events or disruptions, and its confidence interval is wide.
- The satisfaction threshold was derived for one season. Applying it year-round
  reads more from the regression than it says.
- The lowest predicted delay probability available was **37%**. The flight
  recommendation is relative, not safe.

## Case study

A full write-up: the business question, the method, the evidence, and what the
result does not support.

<https://alshammari.dev/projects/commercial-flights-delays/>

## License

MIT. See [LICENSE](LICENSE).
