# Flipkart Price Monitoring System

A Python-based automated system for monitoring Flipkart product prices, ratings, availability, and historical price changes.

## Features

* Multiple Flipkart product monitoring
* Product ID, name, brand, price, rating, and availability extraction
* Historical price tracking
* Price change and percentage calculation
* Availability change detection
* Excel report generation
* Error handling
* Windows Task Scheduler support

## Workflow

```text
products.csv
     ↓
Load Products
     ↓
Selenium Scraping
     ↓
Extract Product Data
     ↓
Save Price History
     ↓
Calculate Price Changes
     ↓
Generate Excel Report
```

## Input

Create `products.csv`:

```csv
Product_ID,Product_Name,Platform,URL
P001,TRIGGR UltraBuds N5,Flipkart,https://www.flipkart.com/...
P002,Mivi DuoPods Solo,Flipkart,https://www.flipkart.com/...
```

Only products with `Platform = Flipkart` are processed.

## Output

```text
data/
└── price_history.csv

reports/
└── Flipkart_Price_Monitoring_Report.xlsx
```

The Excel report contains:

* `Price_History`
* `Latest_Status`
* `Price_Changes`
* `Availability_Changes`

## Installation

```bash
pip install -r requirements.txt
```

Required packages:

```text
selenium
webdriver-manager
pandas
openpyxl
```

## Run

```bash
python flipkart_price_monitor.py
```

The program starts scraping immediately when executed.

## Automation

For automatic monitoring, use **Windows Task Scheduler** to run:

```text
run_price_monitor.bat
```

It can be scheduled hourly, every few hours, or daily.

## Technologies

Python • Selenium • Pandas • OpenPyXL • Chrome WebDriver • CSV • Excel

## Portfolio Skills

Python Programming • Web Scraping • Selenium Automation • Data Processing • Price Monitoring • Excel Automation • Historical Data Analysis • Task Scheduler

## Important Note

Website HTML structure and selectors may change over time. Automated data collection should comply with the target website's terms, robots.txt, and applicable laws.

## Author

**Tapu Kumar Debnath**

Python | Web Scraping | Selenium | Pandas | Data Automation
