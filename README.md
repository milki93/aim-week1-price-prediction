# NewsAnalyzer, stockAnalyzer and SentimentStockAnalyzer

**NewsAnalyzer** is a class for performing Exploratory Data Analysis (EDA) on financial news headlines. It helps uncover trends, sentiment, keyword usage, and publishing patterns.

##### Features

- Load and clean news data  
- Analyze headline lengths and publishers  
- Visualize publishing trends (by date, time, weekday)  
- Extract keywords and generate a word cloud  
- Analyze sentiment using TextBlob  
- Track keyword trends over time  
- Compare weekday vs weekend publishing  



**StockAnalyzer** is a class computes and visualizes common financial indicators using historical stock price data.

#### Features

- **Load stock data** from:
  - CSV files (e.g., `AAPL_historical_data.csv`)

- **Compute indicators** using **TA-Lib**:
  - Simple Moving Average (SMA)
  - Relative Strength Index (RSI)
  - MACD (Moving Average Convergence Divergence)
  - Bollinger Bands

- **Generate and save plots** for each indicator

- **Optional**: Portfolio summary using **PyNance**



**SentimentStockAnalyzer** is a class correlates daily average sentiment from news with daily stock price returns.

#### Features

- Assign sentiment scores using **TextBlob**
- Aggregate **average sentiment per day**
- Calculate **daily stock returns**
- Merge **sentiment and stock data by date**
- Compute **Pearson correlation coefficient**
- Visualize:
  - **Sentiment vs return scatter plot** with regression line
  - **Sentiment trend over time**
