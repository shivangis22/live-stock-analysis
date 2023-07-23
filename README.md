# Live Stock Prediction and Analysis
This project aims to build a Time Series Forecasting model using Long Short-Term Memory (LSTM) neural networks, implemented with TensorFlow. The goal is to predict the daily close prices of a specific stock for the next thirty days based on its historical price data. The pipeline involves data collection from the Polygon REST API, data cleaning and exploratory data analysis (EDA), calculation of various stock metrics, and finally building and training the LSTM model for time series forecasting.

It takes a [NASDAQ](https://www.nasdaq.com/market-activity/stocks/screener) stock name as user input and passes it to the Polygon RESTClient which returns the annual stock data.
## Project Steps
### 1.Data Collection
* Utilize the Polygon REST API to fetch historical stock data for the past one year in CSV format.
* Gather data related to daily open, high, low, volume, and closing price for each trading day.
### 2.Data Cleaning and Preparation:
* Clean the dataset by handling missing values, outliers, and any inconsistencies.
* Format the data for further analysis and modeling.
### 3.Exploratory Data Analysis (EDA):
* Conduct EDA on the stock data to gain insights into its trends, patterns, and characteristics.
* Plot various graphs and visualizations using libraries like Matplotlib, Seaborn, and Plotly to observe stock behavior over time.
* Analyze the annual stock trend using the close value and identify any seasonal patterns.
### 4.Time Series Forecasting with LSTM:
* Prepare the dataset for LSTM modeling, ensuring it is in a suitable format.
* Split the data into training and testing sets, keeping the last 30 days as the test set for validation.
* Build an LSTM model using TensorFlow with appropriate hyperparameters.
* Train the LSTM model on the training dataset.
* Validate the model on the test dataset to measure its performance.
### 5.Stock Price Prediction:
* Utilize the trained LSTM model to predict the daily close prices of the stock for the next thirty days.
* Evaluate the model's accuracy and performance using appropriate metrics.
### 6.Results and Interpretation:
* Present the predicted stock price values for the next thirty days in a clear and interpretable format.
* Analyze the model's performance and discuss any potential limitations or areas for improvement.
## Project Deliverables:
* Python code implementing data collection, data cleaning, and EDA.
* Python code for calculating stock metrics and preparing the dataset for LSTM.
* Python code for building, training, and evaluating the LSTM model using TensorFlow.
* Report or presentation summarizing the project, EDA insights, and LSTM model results.
* Visualizations and graphs illustrating the stock trends and LSTM predictions.

##### Data Visualization using the stock data
![Screenshot 2023-07-23 144646](https://github.com/shivangis22/live-stock-analysis/assets/71970506/b69ed517-45dc-4516-a41d-56e432e76225)

![Screenshot 2023-07-23 144902](https://github.com/shivangis22/live-stock-analysis/assets/71970506/306372be-5174-4bb1-8e1a-17c7e9a600c2)

## Future Enhancemets:
To enhance the project, consider implementing the following:

* Hyperparameter tuning to optimize the LSTM model's performance.
* Experiment with different model architectures for comparison.
* Incorporate external factors (e.g., economic indicators) to improve the predictive performance of the LSTM model.

## Dependencies:
* Python 3.x
* TensorFlow
* Polygon REST API
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Plotly
## How to use:
1. Clone this repository to your local machine.
2. Install the required dependencies using pip.
3. Login to [Polygon](https://polygon.io/stocks?utm_term=polygon.io&utm_campaign=Brand+-+ALL+(Conv+Value+tROAS)&utm_source=adwords&utm_medium=ppc&hsa_acc=4299129556&hsa_cam=14536485495&hsa_grp=132004734661&hsa_ad=591202818400&hsa_src=g&hsa_tgt=aud-896761709510:kwd-812066473604&hsa_kw=polygon.io&hsa_mt=p&hsa_net=adwords&hsa_ver=3&gad=1&gclid=Cj0KCQjwn_OlBhDhARIsAG2y6zOiwNKyExAR8jaWgRJk4VbxtEZSQmtv8NlqrvdkEmsDqJpKWc1NvmoaAuBxEALw_wcB) and get your API Key for stock data.
4. Run the Jupyter notebooks or Python scripts in the correct order to execute the project pipeline.
   
Feel free to contribute to this project by raising issues or submitting pull requests. Your feedback and contributions are highly appreciated!


  
