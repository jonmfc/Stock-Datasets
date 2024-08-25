# Stock-Datasets

This repository acts as a hub for some of the datasets I created to analyze stock market trends.


### Dataset Columns Explained

- **Ticker**: The stock's ticker symbol, a unique identifier for the company (e.g., AAPL for Apple Inc.).

- **Date**: The starting date of the 7-day sequence analyzed.

- **Day 1 to Day 6**: Closing prices of the stock on consecutive trading days, starting from the date specified.

- **Day 7 Percent**: The percentage change in the stock price on the seventh day compared to Day 6.

- **Daycount**: The number of additional days after Day 6 that the stock continued to rise.

- **Overall Percent Change (Day 1 to 6)**: The total percentage change in the stock price from Day 1 to Day 6.

- **Outcome**: A categorical label based on the percentage change on Day 7, indicating the stock’s performance:
  - **0**: Day 7 Percent < -3.5%
  - **1**: -3.5% ≤ Day 7 Percent < -2.5%
  - **2**: -2.5% ≤ Day 7 Percent < -1.6%
  - **3**: -1.6% ≤ Day 7 Percent < -0.8%
  - **4**: -0.8% ≤ Day 7 Percent < 0%
  - **5**: 0% ≤ Day 7 Percent < 0.25%
  - **6**: 0.25% ≤ Day 7 Percent < 0.8%
  - **7**: 0.8% ≤ Day 7 Percent < 1.6%
  - **8**: 1.6% ≤ Day 7 Percent < 2.5%
  - **9**: 2.5% ≤ Day 7 Percent < 3.5%
  - **10**: Day 7 Percent ≥ 3.5%

This dataset is designed for pattern recognition, specifically to identify and analyze continued bull run patterns in stock prices. By studying sequences where stock prices increase over consecutive days, the dataset helps predict the likelihood of further price increases.
