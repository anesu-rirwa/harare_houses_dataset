# 🏠 Harare Housing Data Scraper

This project collects real estate listings for **houses for sale in Harare, Zimbabwe** by scraping publicly available data from leading property websites. The aim is to build a clean, structured dataset that can be used for real estate analytics, housing price prediction models, or market trend analysis.

---

## 📌 Target Websites

The scraper currently extracts data from the following platforms:

1. [Property.co.zw](https://www.property.co.zw/)
2. [Classifieds.co.zw](https://www.classifieds.co.zw/zimbabwe-houses-for-sale)
3. [PropertyBook.co.zw](https://www.propertybook.co.zw/)
4. [Seeff.co.zw](https://www.seeff.co.zw/property-for-sale/harare)
5. [Guest & Tanner](https://www.guestandtanner.co.zw/property-for-sale)

Each scraper is modular and can be run independently.

---

## 🧰 Tech Stack

- **Python 3.8+**
- **BeautifulSoup** – HTML parsing
- **Selenium** – For dynamic content
- **Requests** – HTTP requests
- **Pandas** – Data processing and storage
- **ChromeDriver** – For Selenium

---

## 📂 Project Structure

```path
harare-housing-scraper/
│
├── scrapers/
│   ├── propertycozw\_scraper.py
│   ├── classifiedscozw\_scraper.py
│   ├── propertybookcozw\_scraper.py
│   ├── seeffcozw\_scraper.py
│   └── guestandtanner\_scraper.py
│
├── data/
│   └── raw\_data/               # Scraped raw CSV files
│
├── utils/
│   └── cleaning.py             # Data cleaning and transformation functions
│
├── README.md
├── requirements.txt
└── main.py                     # Script to run all scrapers
````

---

## 📊 Sample Columns in Dataset

Each scraper attempts to collect the following features (where available):

| Column Name         | Description                           |
|---------------------|---------------------------------------|
| `Listing Title`     | Title or headline of the listing      |
| `Price USD`         | Price of the property in USD          |
| `Location`          | Suburb or area in Harare              |
| `Bedrooms`          | Number of bedrooms                    |
| `Bathrooms`         | Number of bathrooms                   |
| `Land Size (sqm)`   | Size of the land                      |
| `House Size (sqm)`  | Size of the house structure           |
| `Amenities`         | e.g., borehole, solar, wall fence     |
| `Description`       | Full text description of the property |
| `Agent Name`        | Real estate agent/company name        |
| `Contact Info`      | Phone or email                        |
| `Posting Date`      | When the listing was posted           |
| `URL`               | Direct link to the listing            |

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/harare-housing-scraper.git
cd harare-housing-scraper
````

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

> Make sure you have **Chrome** and **ChromeDriver** installed and added to PATH (for Selenium).

### 3. Run a Scraper

To run a single scraper:

```bash
python scrapers/propertycozw_scraper.py
```

Or to run all scrapers:

```bash
python main.py
```

---

## ⚖️ Disclaimer

This project is for **educational and research purposes** only. Always review the [terms of service](https://www.property.co.zw/terms) of each website before scraping. Respect robots.txt and use responsible scraping practices.

---

## 👨🏽‍💻 Author

**Anesu Rirwa**
AI/ML Engineer | Data Analyst
[LinkedIn](https://www.linkedin.com/in/anesurirwa) · [Portfolio](https://tenagelabs.com)

---
