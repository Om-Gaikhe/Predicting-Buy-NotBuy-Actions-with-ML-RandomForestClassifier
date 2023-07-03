# Predicting Buy/NotBuy Actions with ML-RandomForestClassifier
This project applies machine learning algorithms (RandomForestClassifier) to predict whether to buy or not to buy S&P 500 stocks based on historical data.

We use Python programming language, data analysis libraries such as Pandas and NumPy, and machine learning libraries including Scikit-learn. For data visualization, we employ Matplotlib, Seaborn, and Plotly. We acquire our data using the yfinance library which allows us to download stock market data from Yahoo Finance. We also use the TA-Lib library for technical analysis.

## Process:
We download the S&P 500 data from Yahoo Finance.

We add features using technical analysis library TA-Lib, including Relative Strength Index (RSI) and Moving Average Convergence Divergence (MACD).

We create a target variable that is binary, indicating whether the closing price will be higher the next day ("Buy") or not ("Not Buy").

We split the data into training, validation, and test datasets.

We create a pipeline that first scales the data using StandardScaler and then applies a RandomForestClassifier.

We use RandomizedSearchCV to tune the hyperparameters of the RandomForestClassifier on the training set.

We evaluate the best model on the validation set and report the F1-score.

We perform cross-validation on the training set.

We make predictions on the test set and again evaluate the F1-score.

We visualize the actual vs. predicted buy/sell actions using interactive Plotly graphs.

## Results:
F1-score is used to evaluate the model's performance. It's a balance between precision and recall and is a better metric when there are imbalanced classes.

Confusion matrix is visualized to understand the true positive, true negative, false positive, and false negative.

We also map the actual vs. predicted actions onto the stock's closing prices. This allows us to visualize how our model's predictions align with the actual movements of the stock price.

## Visualization:
We use Plotly to create an interactive plot that shows:

The stock's closing price over time.
The actual actions (buy or not buy) over time.
The predicted actions (buy or not buy) over time.
The closing price is represented as a bar chart, while the actual and predicted actions are represented as scatter plots. We adjust the colors and opacity of the plots to provide a clear and informative visualization.

## Note:
This project is for educational and informational purposes only and should not be considered financial advice. The stock market is risky and unpredictable, and while machine learning can provide insights, it cannot guarantee profits. Always do your own research and consider seeking advice from financial professionals. 
Lastly, download the images before viewing or use a white theme on your Git Hub to preview the images. Thank you. 
