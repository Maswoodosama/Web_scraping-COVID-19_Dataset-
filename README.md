# Web_scraping-COVID-19_Dataset-
This project scrapes real-time global and country-wise COVID-19 statistics from Worldometer. The extracted data includes total cases, deaths, recoveries, active cases, and more. It can be used for data analysis, visualization, and trend monitoring.


# 🌍 Worldometer COVID-19 Data Scraper

This project is a web scraper built using Python to extract live COVID-19 statistics from [Worldometer](https://www.worldometers.info/coronavirus/). The script collects global and country-wise data such as total cases, deaths, recoveries, and active cases. The final output is stored in a structured CSV file for further analysis, visualization, or tracking.

---

## 📌 Features

- ✅ Scrapes live COVID-19 data from Worldometer
- 🌐 Captures global and country-wise statistics
- 📊 Saves data in a clean tabular format (CSV)
- 🕒 Automatically timestamps the data (date and time of scraping)
- 🔁 Can be scheduled via cron jobs or task scheduler for daily runs

---

## 📁 Data Extracted

The scraper extracts the following fields for each country:

- Country Name
- Total Cases
- New Cases (if available)
- Total Deaths
- New Deaths (if available)
- Total Recovered
- Active Cases
- Serious/Critical Cases
- Total Cases per Million
- Total Deaths per Million
- Total Tests
- Tests per Million
- Population

---

## 🛠️ Technologies Used

| Tool | Purpose |
|------|---------|
| Python | Main programming language |
| `requests` | Fetch the webpage |
| `BeautifulSoup` | Parse HTML and extract table data |
| `pandas` | Create and export structured DataFrame |
| `datetime` | Add current timestamp to scraped data |

---

## 📦 Output Example

The script creates a CSV file like this:

```csv
Date,Country,Total Cases,New Cases,Total Deaths,...
2025-05-09,India,45,712,398,+123,523,000,...
2025-05-09,USA,96,210,455,+342,1,200,000,...

