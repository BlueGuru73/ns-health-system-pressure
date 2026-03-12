Response 1: Problem Definition

This project investigates whether upstream primary care access activity can serve as an early indicator of downstream Emergency Health Services demand across Nova Scotia health zones. Alternative primary care services such as community clinics, pharmacies, and mobile clinics often expand when patients cannot access attached primary care. If changes in these services precede increases in EMS demand, they may provide an early signal of health system pressure. A useful outcome would be the ability to identify periods of elevated EMS demand earlier and support planning decisions for health system administrators.



Response 2: Approach and Tool Selection

I approached this problem by constructing time series signals from public health system datasets. Using Python and pandas, I cleaned and aggregated primary care access activity and EMS response data into monthly indicators by health zone. I engineered features such as rolling averages, percent change, and lagged variables to capture short term trends and potential leading relationships between signals. I then trained a logistic regression classification model using scikit-learn to identify high EMS demand months defined as responses above the seventy fifth percentile for each zone. Logistic regression was chosen because the dataset is relatively small and the model is interpretable. I also created a Power BI visualization to examine trends in primary care activity and EMS demand over time. AI tools were also used during development as a learning and troubleshooting aid. These tools helped identify coding errors, refine Python and pandas operations, and suggest approaches for feature engineering such as rolling averages and lagged variables. All modeling decisions, interpretation of results, and final implementation were reviewed and completed by the author.



Response 3: Reflection

One of the biggest lessons from this project was how much time is required for data preparation compared to modeling. Cleaning datasets, selecting meaningful indicators, and engineering features such as rolling averages and lagged variables required significantly more effort than building the model itself. I also learned that model performance alone does not fully explain system behavior. While the logistic regression model was able to identify some high demand periods, the results suggested that primary care access activity alone cannot fully predict EMS demand. In future work I would include additional indicators such as hospital capacity, seasonal illness trends, and demographic factors to improve predictive performance.

