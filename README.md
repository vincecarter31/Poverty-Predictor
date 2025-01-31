# Poverty-Predictor

This project aimed to identify the key factors influencing poverty rates by integrating multiple datasets, performing data manipulation in MySQL, and applying machine learning techniques in Python. I began by downloading five datasets containing information on poverty rates, corruption, cost of living, education, and drug use. Each dataset was uploaded into MySQL and stored as its own table within a relational database.

Once the data was stored, I wrote SQL queries to join relevant parts of each table into a single, unified dataset. This allowed me to ensure that all key relationships, such as state and year, were properly aligned. After creating the final dataset, I transferred it from MySQL to Jupyter Notebooks for further processing and machine learning analysis.

In Python, I performed preprocessing tasks such as feature scaling and handling missing values before training two machine learning models: a Neural Network using Keras and an XGBoost model. The models were evaluated using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² scores to assess their predictive accuracy. The results showed that XGBoost outperformed the Neural Network, likely due to its ability to efficiently handle structured data.

To better understand the relationship between features and poverty rates, I used XGBoost’s built-in feature importance analysis. This revealed that education levels and cost of living had the strongest correlation with poverty, while corruption levels also played a significant role.
