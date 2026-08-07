# Financial Dashboards with API Integration

This project demonstrates the creation of **simple financial dashboards** in Jupyter Notebooks, integrating real-time data from the Yahoo Finance API (`yfinance`). The focus is on building interactive visualizations for stock analysis, including candlestick charts, moving averages, and trading volume.

---

## Strategic Raw Materials Dashboard — Automotive & EV Industry

### Objective
Create an interactive dashboard to monitor **strategic raw materials** relevant to the automotive and electric vehicle industry, using financial data from Yahoo Finance.

### Libraries Used
- pandas, numpy  
- yfinance (financial data API)  
- plotly (graph_objects, io)  
- ipywidgets (widgets, display)  
- warnings  

### Dataset
Data retrieved dynamically from **Yahoo Finance API** for key materials:  
- Copper (HG=F) – Wiring / EV motors  
- Aluminum (ALI=F) – Lightweight chassis  
- Palladium (PA=F) – Gasoline catalysts  
- Platinum (PL=F) – Diesel catalysts  
- Lithium ETF (LIT) – Batteries  

### Main Results
- Implemented caching to optimize API queries and avoid redundant requests.  
- Interactive dashboard with candlestick charts and volume analysis for multiple commodities.  
- Real-time monitoring of price trends for strategic materials in the automotive and EV sector.  
- Enhanced error handling for robust API integration.  

---

## Dashboard-Simple_EHG

### Objective
Develop a lightweight dashboard to visualize stock prices and trading volume using candlestick charts, enriched with moving averages and interactive controls.

### Libraries Used
- **pandas, numpy** – data manipulation  
- **yfinance** – financial data API  
- **plotly (graph_objects, make_subplots)** – interactive visualizations  
- **ipywidgets (interact, display)** – interactive controls  
- **warnings** – error handling  

### Dataset
Stock market data retrieved dynamically from **Yahoo Finance API** via `yfinance`.  
Default ticker: **AAPL (Apple Inc.)**, with customizable period and interval.

### Main Results
- Interactive candlestick chart with OHLC data.  
- Moving averages (50-day and 200-day) plotted for trend analysis.  
- Trading volume visualized with color-coded bars (green for bullish, red for bearish).  
- Console output showing latest price, percentage change, and maximum price.  
- Dashboard fully interactive with Plotly and ipywidgets.  

---

## Finanzas-EHG

### Objective
Extend dashboard functionality to broader financial analysis, integrating multiple widgets and subplots for enhanced exploration.

### Libraries Used
- **pandas** – data handling  
- **yfinance** – financial data API  
- **plotly (graph_objects, make_subplots, io)** – interactive visualizations  
- **ipywidgets** – interactive controls  
- **IPython.display** – notebook integration  

### Dataset
Financial data retrieved from **Yahoo Finance API**.  
Supports multiple tickers and customizable visualization options.

### Main Results
- Configured interactive dashboards for financial data exploration.  
- Enabled visualization of multiple financial indicators in Jupyter Notebook.  
- Integrated widgets for dynamic user interaction.  
- Successfully combined API-driven data with interactive dashboards.  

---

## Key Takeaways
- **API integration** with `yfinance` enables real-time financial data analysis.  
- **Interactive dashboards** built with Plotly and ipywidgets enhance usability and exploration.  
- These projects demonstrate practical skills in **data visualization, financial analytics, and dashboard development**.  

