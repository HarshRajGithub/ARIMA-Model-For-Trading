# ARIMA Model For Trading

## Overview

Used ARIMA Model based on the research paper [A Quantitative Trading Strategy Based on A Position Management Model 
](https://github.com/HarshRajGithub/ARIMA-Model-For-Trading/blob/main/A%20Quantitative%20Trading%20Strategy%20Based%20on%20A%20Position.pdf)

## Colab Link [Link to Colab](https://colab.research.google.com/drive/17EH1tz9l_zUMV-t2Qyq18zfLgGh2Smcz?usp=sharing)

## Data Cleaning and Preprocessing

- **Missing Values**: Check for missing values in the dataset and decide on an appropriate strategy to handle them, such as filling with mean or median values or dropping rows/columns with too many missing values.
- **Data Types**: Ensure that the data types of each column are appropriate. For example, datetime should be in datetime format, and numerical columns should be of float or integer types.
- **Outliers**: Identify and handle outliers in the dataset, which could be due to data entry errors or extreme market events.

## Descriptive Statistics

- **Summary Statistics**: Use `df.describe()` to get a quick overview of the central tendency, dispersion, and shape of the dataset’s distribution.
- **Correlation Analysis**: Analyze the correlation between different variables using `df.corr()` to understand the relationships between them. This can help in identifying which variables might be predictive of trading signals.

## Visualizations

- **Time Series Analysis**: Plot the 'close' price over time to visualize the overall trend and seasonality.
- **Price Distribution**: Use histograms to understand the distribution of the 'close' price and identify any skewness or outliers.
- **Volume Analysis**: Plot the 'volume' against the 'close' price to understand the relationship between trading volume and price movements.
- **Signal Analysis**: Visualize the 'signal' column to see the frequency and distribution of buy, sell, and none signals over time.
- **EMAs and RSI**: Plot the EMAs and RSI to understand their behavior and how they might correlate with price movements or trading signals.
- **Fear and Greed Index**: Analyze the Fear and Greed Index over time to see if it correlates with market movements or trading signals.

## Feature Engineering

- **Lagged Variables**: Create lagged versions of the 'close' price and other relevant variables to capture the temporal dependencies in the data.
- **Rolling Statistics**: Calculate rolling means, standard deviations, or other statistics over a window of time to capture trends or volatility.
- **Technical Indicators**: If not already present, calculate technical indicators like Moving Averages, MACD, RSI, etc., to enrich the dataset with additional predictive features.

## Model Evaluation

- **Model Selection**: Based on the EDA findings, the ARIMA model was selected for predicting trading signals due to its effectiveness in handling time series data with trends and seasonality. The ARIMA model, with its parameters (p=1, d=1, q=1), was chosen for its simplicity and efficiency in capturing the underlying patterns in the data.
- **Cross-Validation**: Cross-validation techniques were employed to evaluate the performance of the ARIMA model. This involved splitting the dataset into training and testing sets to assess the model's ability to generalize to unseen data. The performance metrics, such as  Mean Squared Error (MSE), were used to quantify the model's accuracy in predicting future 'close' prices.
- **Mean Squared Error**: 17790293.505004823

## Insights and Recommendations

- **Trading Strategies**: The ARIMA model's predictions were used to generate trading signals. A 'Buy' signal was recommended when the predicted 'close' price was higher than the actual 'close' price, indicating an upward trend. Conversely, a 'Sell' signal was recommended when the predicted 'close' price was lower than the actual 'close' price, suggesting a downward trend. The model's performance in accurately predicting these trends forms the basis of the recommended trading strategy.
- **Risk Management**: The ARIMA model's predictions were analyzed to assess the risk associated with different trading signals. By comparing the predicted 'close' prices with the actual prices, the model's accuracy in predicting market movements was evaluated. This analysis helped in developing strategies to manage risk effectively, ensuring that trades are made only when there is a high degree of confidence in the model's predictions.

## Output Image
![Output Image](https://github.com/HarshRajGithub/ARIMA-Model-For-Trading/blob/main/Images%20Quant%20Trading%20APP/outputWithBuyandSellPositionpng.png)

## Conclusion

The ARIMA model has proven to be a robust and effective tool for analyzing historical price patterns, identifying trends, and predicting future market movements in trading. By leveraging the statistical properties of time series data, ARIMA enables traders to make informed decisions based on a thorough understanding of market dynamics. The model's ability to capture time-dependent patterns, handle non-stationarity, and provide interpretable results makes it a valuable tool in the trading toolkit.

This project stands as a testament to the potential of the ARIMA model in enhancing trading strategies and decision-making processes. By acknowledging its limitations and incorporating additional data sources and analysis techniques, traders can maximize the potential of ARIMA to improve their investment outcomes.

## Contributing

Contributions are welcome!

## Acknowledgements

This project was inspired by various sources and projects. I give credit where credit is due.

