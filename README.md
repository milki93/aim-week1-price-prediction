# NewsAnalyzer

**NewsAnalyzer** is a Python class for performing Exploratory Data Analysis (EDA) on financial news headlines. It helps uncover trends, sentiment, keyword usage, and publishing patterns.

## Features

- Load and clean news data  
- Analyze headline lengths and publishers  
- Visualize publishing trends (by date, time, weekday)  
- Extract keywords and generate a word cloud  
- Analyze sentiment using TextBlob  
- Track keyword trends over time  
- Compare weekday vs weekend publishing  

## Usage

```python
from news_analyzer import NewsAnalyzer

analyzer = NewsAnalyzer(csv_path="data/raw_analyst_ratings.csv", show_plots=True)
analyzer.run_all()
analyzer.plot_keyword_trend("merger")
analyzer.top_keywords_by_publisher("Reuters")
analyzer.compare_weekday_weekend()
