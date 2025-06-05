# Financial Market Analysis and Sentiment Project

## Overview
This project combines financial market technical analysis with news sentiment analysis to provide comprehensive insights into market trends, focusing on Apple Inc. (AAPL) stock. The analysis includes technical indicators, news sentiment correlation, and publication trend analysis.

## Key Features
- Technical Analysis of AAPL stock (RSI, MACD, Moving Averages)
- News sentiment analysis using TextBlob
- Publication trend analysis
- Correlation studies between news sentiment and stock price movements
- Automated merging and cleaning of news and stock data
- Correlation heatmap between sentiment, returns, and technical indicators

## Project Structure
```
.
├── data/               # Raw and processed data
│   └── merged_sentiment_stock_data.csv  # Merged output from Task 3
├── notebooks/          # Jupyter notebooks for analysis
│   ├── reports/        # Generated visualizations
│   │   ├── sentiment_vs_daily_return.png
│   │   └── correlation_heatmap.png
├── src/               # Source code
├── tests/             # Unit tests
└── requirements.txt   # Project dependencies
```

## Technical Analysis Results

### 1. AAPL Stock Analysis
The project includes several technical analysis visualizations:

- **RSI (Relative Strength Index)**
  - image.png
  - Helps identify overbought/oversold conditions
  
- **MACD (Moving Average Convergence Divergence)**
  - image.png
  - Shows momentum and trend direction
  
- **Moving Averages**
  - image.png
  - Displays short and long-term price trends
  
- **Daily Returns Analysis**
  - image.png
  - Shows daily price volatility

### 2. News Publication Analysis
- **Hourly Publication Patterns**
  - Located at: `notebooks/reports/hourly_publication.png`
  - Shows peak publishing hours
  
- **Publication Trends**
  - Located at: `notebooks/reports/publication_trend.png`
  - Displays long-term trends in news coverage

## Tasks and Progress

### Completed Tasks
- [x] Initial project setup and structure
- [x] Technical indicator implementation (RSI, MACD)
- [x] Data visualization generation
- [x] Basic sentiment analysis implementation
- [x] Merging and correlation analysis of news and stock data (Task 3)

### Ongoing Tasks
- [ ] Enhance sentiment analysis accuracy
- [ ] Implement advanced correlation studies
- [ ] Create interactive dashboard
- [ ] Write comprehensive analysis report

### Future Tasks
- [ ] Add more technical indicators
- [ ] Implement machine learning predictions
- [ ] Expand to more stock symbols
- [ ] Create automated daily reports

## Task 3: Correlation between News and Stock Movement

**Goal:**  
Analyze the relationship between news sentiment and AAPL stock price movements by merging daily sentiment scores with technical and return data, and visualizing their correlation.

**Approach:**
- Load processed news data (`data/processed_analyst_ratings.csv`) and stock data (`data/processed_AAPL_historical_data.csv`).
- Convert and align date columns.
- Aggregate sentiment by date to get average daily sentiment.
- Merge sentiment and stock data on the date.
- Drop missing values to ensure clean analysis.
- Calculate the Pearson correlation between average daily sentiment and daily stock return.
- Visualize:
  - **Scatter plot:** Sentiment vs. Daily Return (`notebooks/reports/sentiment_vs_daily_return.png`)
  - **Correlation heatmap:** Sentiment, returns, and technical indicators (`notebooks/reports/correlation_heatmap.png`)
- Save merged data to `data/merged_sentiment_stock_data.csv`.

**Outputs:**
- `data/merged_sentiment_stock_data.csv`: Merged and cleaned dataset for further analysis.
- `notebooks/reports/sentiment_vs_daily_return.png`: Scatter plot of sentiment vs. daily return.
- `notebooks/reports/correlation_heatmap.png`: Heatmap of correlations between sentiment, returns, and technical indicators.

**Key Results:**
- The Pearson correlation between average daily sentiment and daily return is **0.0455** (very weak positive correlation).
- All visualizations and merged data are saved for further exploration.

## Setup Instructions

1. Clone the repository:
```
git clone https://github.com/your-username/week1-challenge.git
cd week1-challenge
```

2. Create and activate virtual environment:
```
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```
pip install -r requirements.txt
```

## Running the Analysis
- Run the Jupyter notebooks in the `notebooks/` directory.
- Task 3 notebook will generate new files in `data/` and `notebooks/reports/`.

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the LICENSE file for details.