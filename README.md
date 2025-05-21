Amazon Product Scraper: Utilizes Selenium for dynamic content and ScraperAPI for robust anti-bot circumvention on Amazon product pages.
Ethical Crawling: Adheres to robots.txt, implements 2-second delays between requests, and uses realistic User-Agents.
Articles Crawler: Extracts structured data (titles, dates, authors, text) from news sites, exemplified by Al Jazeera.
Streamlit UI: Provides an interactive interface for general crawling, visualizations, and reporting.
Data Output: Saves extracted data to CSV/PDF.
🛠️ Technologies
Python: requests, BeautifulSoup4, pandas
Web Automation: selenium (with webdriver-manager), playwright
Proxy/Anti-Bot: ScraperAPI
Web App: streamlit, altair
Utilities: fake_useragent, fpdf, urllib.robotparser
⚙️ Setup
Clone: git clone https://github.com/NourHossam21/Web_Crawling.git
Navigate: cd Web_Crawling
Install Dependencies: pip install -r requirements.txt (or install listed libs)
Install Playwright Drivers: playwright install
ScraperAPI Key: Obtain a key from ScraperAPI and configure it in your Amazon scraper.
🚀 How to Run
Streamlit UI (General Crawler): streamlit run app.py
Amazon Product Scraper: Run amazon_scraper.py directly (check file for execution details).
Al Jazeera Crawler: Open and run cells in aljazeera_crawler.ipynb (or similar notebook).
🤝 Contribution
Feel free to open issues or submit pull requests.
