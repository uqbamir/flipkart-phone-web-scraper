# Flipkart Phone Web Scraper

A Python-based web scraping project that extracts real-time smartphone listing data from Flipkart, cleans it using regular expressions, and structures it into an analysis-ready dataset. Built with **Python, Requests, BeautifulSoup, Regex, and Pandas**, this project demonstrates end-to-end skills in **web scraping, data extraction, data cleaning, and data wrangling**.

## Overview

This project scrapes product listings for smartphones from Flipkart's search results across multiple pages and extracts key details including product name, price, rating, number of ratings/reviews, and technical specifications. Raw specification text is parsed using regular expressions to isolate structured fields such as Brand, Processor, RAM, ROM, Battery capacity, Display size, and Camera details. The final cleaned dataset is exported to a CSV file for further analysis.

## Key Features

- **Automated Web Scraping**: Sends HTTP requests with custom User-Agent headers to bypass basic bot detection and retrieve HTML content.
- **HTML Parsing**: Uses BeautifulSoup to parse and navigate the DOM to locate product elements.
- **Multi-Page Scraping**: Iterates through multiple search result pages to build a larger dataset.
- **Data Extraction**: Pulls product name, price, rating, number of ratings, number of reviews, and full specification text.
- **Regex-Based Data Cleaning**: Extracts structured fields (Brand, Processor, RAM, ROM, Battery, Display Size, Camera) from unstructured specification strings using regular expressions.
- **Data Transformation**: Converts extracted text fields into proper numeric data types (float, int) using Pandas.
- **Data Export**: Outputs the final cleaned dataset as a structured CSV file ready for analysis or visualization.

## Tech Stack / Skills Demonstrated

| Category | Tools / Concepts |
|---|---|
| Programming Language | Python |
| Web Scraping | Requests, BeautifulSoup, HTTP Headers, HTML Parsing |
| Data Cleaning | Regular Expressions (Regex), String Manipulation |
| Data Analysis | Pandas, NumPy |
| Data Handling | CSV Export, DataFrame Operations, Type Conversion |
| Core Concepts | Web Scraping, Data Extraction, Data Wrangling, ETL (Extract-Transform-Load) |

## Project Workflow

1. **Send Request** — Send an HTTP GET request to Flipkart's search page with appropriate headers to avoid a 403 (Forbidden) response.
2. **Parse HTML** — Parse the returned HTML content using BeautifulSoup.
3. **Extract Raw Data** — Loop through each product listing and extract name, price, rating, ratings/reviews count, and specification text.
4. **Scale Across Pages** — Repeat extraction across multiple pages of search results to build a larger dataset.
5. **Clean & Structure Data** — Apply regex patterns to break down the specification string into individual columns (Brand, Processor, RAM, ROM, Battery, Display Size, Camera).
6. **Transform Data Types** — Convert price and rating fields from strings to numeric types for analysis.
7. **Export Dataset** — Save the final structured dataset as a CSV file.

## Sample Output Columns

`Brand | Product_name | Processor | RAM | ROM | Battery | Display_Size | Camera | No_of_ratings | No_of_reviews | Rating | Price`

## How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/<your-username>/flipkart-phone-web-scraper.git
   cd flipkart-phone-web-scraper
   ```

2. Install dependencies
   ```bash
   pip install numpy pandas matplotlib seaborn requests beautifulsoup4
   ```

3. Open and run the notebook
   ```bash
   jupyter notebook Web_Scraping.ipynb
   ```

4. The scraped and cleaned dataset will be saved as `Flipkart Phones.csv`.

## Requirements

- Python 3.x
- numpy
- pandas
- matplotlib
- seaborn
- requests
- beautifulsoup4
- jupyter

## Disclaimer

This project is for learning purposes only, intended to demonstrate web scraping, data extraction, and data cleaning techniques.

## Author

**Uqba Mir**
[LinkedIn](https://www.linkedin.com/in/uqbamir) | [GitHub](https://github.com/uqbamir/) | [Email]uqbamir11@gmail.com)
