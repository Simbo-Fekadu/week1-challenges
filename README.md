# Financial Market Analysis and Sentiment Project

## Overview
This project combines financial market technical analysis with news sentiment analysis to provide comprehensive insights into market trends, focusing on Apple Inc. (AAPL) stock. The analysis includes technical indicators, news sentiment correlation, and publication trend analysis.

## Key Features
- Technical Analysis of AAPL stock (RSI, MACD, Moving Averages)
- News sentiment analysis using TextBlob
- Publication trend analysis
- Correlation studies between news sentiment and stock price movements

## Project Structure
```
.
├── data/               # Raw and processed data
├── notebooks/          # Jupyter notebooks for analysis
│   └── reports/       # Generated visualizations
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

## Setup Instructions

1. Clone the repository:
```bash
git clone https://github.com/your-username/week1-challenge.git
cd week1-challenge
```

2. Create and activate virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Running the Analysis
1. Navigate to the notebooks directory
2. Start Jupyter Notebook or JupyterLab
3. Open the analysis notebooks in sequential order

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the LICENSE file for details.
