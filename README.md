# CodeAlpha Data Analytics Internship — Task 1: Web Scraping

## Overview
For this task, I chose to scrape book listing data from [books.toscrape.com](https://books.toscrape.com), a site built for practicing web scraping. I used **Octoparse**, a no-code scraping tool, to collect a structured dataset of books that I could later use for exploratory data analysis and visualization.

## Project Details

| | |
|---|---|
| **Task** | Task 1 — Web Scraping |
| **Internship** | CodeAlpha — Data Analytics |
| **Tool used** | Octoparse |
| **Source website** | https://books.toscrape.com |
| **Fields collected** | Title, Price, Rating |
| **Total records collected** | 1,000 books |

## Methodology

### 1. Tool Setup
- Opened Octoparse and created a new scraping task targeting books.toscrape.com.
- Used Octoparse's point-and-click interface to identify the repeating book listing elements on each catalogue page.
- Configured three data fields to extract: **Title**, **Price**, and **Rating** (star rating shown on each book card).

### 2. Pagination
- Set up an auto-pagination rule so Octoparse followed the "Next" link across all catalogue pages.
- Let the task run until the full catalogue was traversed, collecting **1,000 book records** in total.

### 3. Data Cleaning
- Removed currency symbol inconsistencies and confirmed all prices were in GBP (£).
- Converted star ratings from text/image labels (e.g. "Three") into numeric values (1–5).
- Checked for and removed duplicate rows.
- Exported the final dataset to Excel format (Title, Price, Rating).

## Sample of Cleaned Data

| Title | Price | Rating |
|---|---|---|
| A Light in the Attic | £51.77 | 3 |
| Tipping the Velvet | £53.74 | 1 |
| Soumission | £50.10 | 1 |
| Sharp Objects | £47.82 | 4 |
| Sapiens: A Brief History of Humankind | £54.23 | 5 |

## Key Observations
- The dataset contains 1,000 unique book entries spanning multiple genres and price ranges.
- Prices range broadly, giving a useful spread for later statistical analysis (e.g. average price, price distribution by rating).
- Ratings are distributed across the 1–5 star scale, which can support further analysis such as correlating price with rating.

## Conclusion
Using Octoparse, I scraped a complete dataset of 1,000 books (Title, Price, Rating) from books.toscrape.com without writing any code. The exported Excel file is included in this repository and is ready for use in exploratory data analysis and visualization tasks.

## Files Included in This Repository
- `book_listings.xlsx` — full exported dataset (1,000 rows: Title, Price, Rating)
- cleaned dataset

