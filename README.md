# ARIMA Model For Trading

## Overview

Used ARIMA Model based on the research paper [Link to PDF](https://github.com/HarshRajGithub/ARIMA-Model-For-Trading/blob/main/A%20Quantitative%20Trading%20Strategy%20Based%20on%20A%20Position.pdf)

This project includes parameters like datetime, open, high, low, close, volume, reserve, funding rates, MVRV, NRPL, NUPL, stock-to-flow reversion, STH, SOPR, signal (buy, sell, none), RSI, EMAs, and the Fear and Greed Index. Conducting an Exploratory Data Analysis (EDA) is crucial to understand the data's characteristics, identify patterns, and inform further analysis or modeling.

## Data Cleaning and Preprocessing

- **Missing Values**: Check for missing values in the dataset and decide on an appropriate strategy to handle them, such as filling with mean or median values or dropping rows/columns with too many missing values.
- **Data Types**: Ensure that the data types of each column are appropriate. For example, datetime should be in datetime format, and numerical columns should be of float or integer types.
- **Outliers**: Identify and handle outliers in the dataset, which could be due to data entry errors or extreme market events.

## Descriptive Statistics

- **Summary Statistics**: Use `df.describe()` to get a quick overview of the central tendency, dispersion, and shape of the dataset’s distribution.
- **Correlation Analysis**: Analyze the correlation between different variables using `df.corr()` to understand the relationships between them. This can help in identifying which variables might be predictive of trading signals.

## Visualizations

- **Time Series Analysis**: Plot the 'close' price over time to visualize the overall trend and seasonality.
- **Price Distribution**: Use histograms or box plots to understand the distribution of the 'close' price and identify any skewness or outliers.
- **Volume Analysis**: Plot the 'volume' against the 'close' price to understand the relationship between trading volume and price movements.
- **Signal Analysis**: Visualize the 'signal' column to see the frequency and distribution of buy, sell, and none signals over time.
- **EMAs and RSI**: Plot the EMAs and RSI to understand their behavior and how they might correlate with price movements or trading signals.
- **Fear and Greed Index**: Analyze the Fear and Greed Index over time to see if it correlates with market movements or trading signals.

## Feature Engineering

- **Lagged Variables**: Create lagged versions of the 'close' price and other relevant variables to capture the temporal dependencies in the data.
- **Rolling Statistics**: Calculate rolling means, standard deviations, or other statistics over a window of time to capture trends or volatility.
- **Technical Indicators**: If not already present, calculate technical indicators like Moving Averages, MACD, RSI, etc., to enrich the dataset with additional predictive features.

## Model Evaluation

- **Model Selection**: Based on the EDA findings, select appropriate models for predicting trading signals. This could include time series models like ARIMA, machine learning models like Random Forest or Gradient Boosting, or deep learning models for more complex patterns.
- **Cross-Validation**: Use cross-validation techniques to evaluate the performance of the selected models and tune their hyperparameters.

## Insights and Recommendations

- **Trading Strategies**: Based on the EDA and model evaluations, identify potential trading strategies. For example, if certain technical indicators or market conditions consistently precede profitable trades, these could form the basis of a trading strategy.
- **Risk Management**: Analyze the risk associated with different trading signals and develop strategies to manage risk effectively.

This comprehensive EDA process will provide a solid foundation for understanding the Bitcoin trading dataset, identifying patterns, and informing the development of trading strategies or predictive models.

## Output Image
![Output Image](https://github.com/HarshRajGithub/ARIMA-Model-For-Trading/blob/main/Images%20Quant%20Trading%20APP/outputWithBuyandSell.png)

