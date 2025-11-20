Stock Market Analytics Dashboard (Power BI)
📌 Project Overview

This project analyzes stock performance across categories A, B, and C using an interactive Power BI dashboard.
It helps users understand price trends, returns, volume patterns, and volatility.

📊 Key Features

6 interactive Power BI visuals

Trend line charts for stock price movement

KPI cards (High, Low, Average Closing Price, Total Volume)

Returns comparison across stock categories

Dynamic slicers (stock name, date filters)

Individual stock-level tables

🛠 Tools Used

Power BI

DAX

Excel / CSV

Power Query (data cleaning)

📐 DAX Measures
Total Volume = SUM('Table'[Volume])

Average Closing Price = AVERAGE('Table'[Close])

Daily Returns = 
DIVIDE(
    [Close] - CALCULATE([Close], PREVIOUSDAY('Table'[Date])),
    CALCULATE([Close], PREVIOUSDAY('Table'[Date]))
)

Max Price = MAX('Table'[High])
Min Price = MIN('Table'[Low])

YTD Return = TOTALYTD(AVERAGE('Table'[Close]), 'Table'[Date])

📂 Project Structure
📁 stock-market-dashboard
│── StockDashboard.pbix
│── data/
│── screenshots/
│── README.md

📷 Screenshots

(Insert images if uploaded)

🚀 Insights Generated

Identified highest & lowest performing stocks

Discovered clear trends using daily price movement

Compared stock categories A, B, and C

Highlighted volatility and return patterns

👤 Author

Pankaj Dabholkar
Data Analytics | Power BI | Business Analytics
