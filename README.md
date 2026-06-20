# waze-user-churn-analysis
Initial data inspection, data cleaning, and exploratory analysis on Waze user behavioral data using Python.
# Waze User Churn Project: Data Inspection & Triage

## Project Overview
This project focuses on the initial inspection, data cleaning, and exploratory analysis of monthly user behavioral data for Waze. The ultimate goal is to build a predictive machine learning model to mitigate user churn and improve retention.

## Key Findings
* **Data Integrity:** Identified and handled 700 missing values localized entirely within the `label` column. Analysis confirmed these gaps are distributed randomly and do not introduce bias into the broader dataset.
* **Device Representation:** The platform user base is comprised of 64.5% iPhone users and 35.5% Android users. This ratio remains stable across both churned and retained segments.
* **The "Super Driver" Profile:** Discovered that churned users log an exceptional median distance of 698 km per driving day—nearly 240% higher than retained users. This indicates that churn risk is heavily concentrated among long-haul drivers or heavy commuters.

## Next Steps
1. Conduct full Exploratory Data Analysis (EDA) and build visualizations to further map the driving habits of churned users.
2. Enrich the dataset with demographic and vehicle-type data.
3. Engineer specialized metrics (like kilometers-per-drive) to prepare for machine learning classification models.

## Tools & Libraries Used
* Python
* Pandas
* NumPy
## Personal Reflection & Key Takeaways
Completing this initial phase of the Waze user churn project highlighted a few critical data principles for me:
* **The Importance of the Median:** This dataset perfectly demonstrated why data analysts cannot rely blindly on mean averages. With extreme outliers present (like a maximum driving distance exceeding 21,000 km), calculating the median was essential to getting an accurate, undistorted view of a typical user.
* **Thinking Beyond the Code:** Data science isn't just about writing Python functions; it's about translating numbers into business realities. Successfully connecting a 698 km median driving distance to a concrete "super driver" or commuter persona showed me how technical analysis directly informs corporate strategy.
* **The PACE Framework:** Walking through a structured problem-solving methodology taught me the value of careful planning and data triaging before rushing into visualizations or predictive modeling.
