📌 Project Objective

Build a model to predict gold prices based on historical data.

Use PySpark MLlib to handle large-scale data and train a regression model.

Demonstrate how to create lag features (previous days’ prices) to predict the current day’s price.

🛠 Environment Requirements

You need to install the following tools:

Python 3.x

Apache Spark (PySpark)

Python libraries:

pyspark

numpy

matplotlib

Dataset file: gold_prices.csv (should be placed in the same directory or adjust the file path accordingly).

📖 Main Workflow in the Notebook

Initialize SparkSession for PySpark operations.

Load the CSV file containing gold price data (Date, Buy Price, Sell Price).

Preprocess the data:

Convert Date column to date format.

Rename columns with spaces.

Sort data by time.

Feature engineering: add columns lag_1 … lag_10 (gold prices of the previous 10 days).

Split the dataset into training and testing sets (70:30).

Train a Linear Regression model to predict gold prices.

Evaluate the model using metrics (RMSE, R²).

Visualize results by comparing predicted vs. actual gold prices.

✅ Results

The linear regression model successfully predicts the trend of gold prices based on historical data.

Performance is evaluated using RMSE and R² to verify accuracy.

Visualization clearly shows the gap between predicted and actual prices.

💡 Future Improvements

Try other models: Random Forest, Gradient Boosted Trees.

Add more features such as: Sell Price, Buy/Sell difference, day of week, month…

Apply additional time series techniques (ARIMA, LSTM) for comparison with PySpark MLlib.