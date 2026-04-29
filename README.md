# 🌐 Dynamic Website Scraper using Selenium

A Python scraper built with Selenium that extracts dynamically loaded data from a JavaScript-heavy website. Handles full pagination automatically and exports clean, structured data into a formatted multi-sheet Excel file.

---

## 📌 Project Overview

This project targets **quotes.toscrape.com** — a JavaScript-rendered site — and collects all quotes, authors, and tags across **10 pages** automatically using a real Chrome browser controlled by Selenium.

---

## ✨ Features

- ✅ Scrapes **dynamically loaded** JavaScript content using real Chrome browser
- ✅ Extracts **quote text, author name, tags, and author bio link**
- ✅ Handles **full pagination** automatically
- ✅ Uses **WebDriverWait** for reliable element detection
- ✅ Cleans data — removes duplicates, strips whitespace, adds word count
- ✅ Exports to **formatted Excel (.xlsx)** with 3 sheets:
  - 📄 **All Quotes** — complete dataset with alternating row colors
  - 📄 **Authors Summary** — quote count & tags per author
  - 📄 **Top Tags** — most frequently used tags ranked

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| Python | Core programming language |
| Selenium | Browser automation & dynamic content scraping |
| Pandas | Data cleaning, transformation & analysis |
| OpenPyXL | Excel export with formatting |
| ChromeDriver | Controls Chrome browser headlessly |

---

## 📁 Project Structure

```
dynamic-website-scraper/
│
├── selenium_scraper.py   # Main Selenium scraper script
├── quotes_data.xlsx      # Output Excel file (generated after running)
└── README.md             # Project documentation
```

---

## ⚙️ How to Run

**1. Clone the repository**
```bash
git clone https://github.com/YOUR_USERNAME/dynamic-website-scraper.git
cd dynamic-website-scraper
```

**2. Install dependencies**
```bash
pip install selenium pandas openpyxl
```

**3. Make sure Google Chrome is installed, then run:**
```bash
# Scrape all 10 pages
python selenium_scraper.py

# Or test with fewer pages (e.g. 3)
python selenium_scraper.py 3
```

**4. Open `quotes_data.xlsx` to see your results!**

---

## 📊 Sample Output

| Quote | Author | Tags | Word Count |
|-------|--------|------|------------|
| The world as we have created it... | Albert Einstein | change, deep-thoughts | 18 |
| It is our choices that show... | J.K. Rowling | choices, inspirational | 12 |

---

## 📈 Auto-Generated Summary

```
Total quotes     : 100
Unique authors   : 50
Unique tags      : 140
Most quoted      : Albert Einstein (10 quotes)
Most used tag    : #inspirational
Avg word count   : 21.3 words/quote
```

---

## 🚀 Skills Demonstrated

- Browser automation with Selenium WebDriver
- Scraping JavaScript-rendered / dynamic content
- Pagination handling across multiple pages
- Data cleaning & transformation with Pandas
- Multi-sheet formatted Excel export with OpenPyXL

---

## 📬 Contact

Available for freelance web scraping & automation projects on [Upwork](https://www.upwork.com)!
