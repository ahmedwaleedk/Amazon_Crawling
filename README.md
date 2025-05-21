Amazon Product Scraper & Analyzer
This project is a sophisticated web crawling solution primarily focused on ethical and efficient data extraction from Amazon.com. It leverages advanced techniques to navigate Amazon's dynamic website, collect product information, and provide an interactive interface for analysis.

🚀 Key Features
Advanced Amazon Product Scraping:
Dynamic Content Handling: Utilizes Selenium to fully render JavaScript-heavy Amazon product pages, ensuring all data is accessible.
Anti-Bot Resilience: Integrates ScraperAPI to effectively manage IP rotation, CAPTCHA challenges, and other anti-bot measures, ensuring reliable data retrieval.
Targeted Data Extraction: Accurately collects key product details such as name, price, ratings, and descriptions.
Smart URL Discovery: Systematically generates Amazon search URLs and extracts individual product links from search results pages.
Ethical Web Crawling Practices:
robots.txt Compliance: Strictly adheres to Amazon's robots.txt directives, avoiding all disallowed paths (e.g., cart pages, private APIs).
Polite Delays: Implements a 2-second delay between requests to prevent server overload and maintain responsible scraping behavior.
User-Agent Randomization: Uses realistic and varied User-Agent strings to mimic human Browse patterns.
Interactive Streamlit UI: Provides an intuitive web application for initiating crawls, visualizing collected data, and generating reports.
Structured Data Output: Saves extracted product information into organized formats (e.g., CSV, PDF) for easy analysis and reporting.
🛠️ Technologies
Python: The core programming language.
requests: For making initial HTTP requests (e.g., to robots.txt).
BeautifulSoup4: For efficient HTML parsing of static content and extracting links from search results.
selenium: For automating browser interactions and rendering dynamic JavaScript content on product pages.
webdriver-manager: To automatically manage browser drivers (e.g., Chrome).
fake_useragent: For generating randomized User-Agent strings.
pandas: For robust data manipulation, analysis, and structuring the scraped information.
streamlit: For creating the interactive web application interface.
altair: For rich data visualizations within the Streamlit application.
fpdf: For generating PDF reports of the scraped data.
urllib.robotparser: For programmatic parsing and adherence to robots.txt files.
ScraperAPI: A crucial third-party service used to handle proxies, CAPTCHAs, and other anti-bot challenges when accessing Amazon.
⚙️ Setup
Clone the repository:
Bash

git clone https://github.com/NourHossam21/Web_Crawling.git
cd Web_Crawling
Create a virtual environment (recommended):
Bash

python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
Install dependencies:
Bash

pip install -r requirements.txt # Ensure your requirements.txt lists all libraries above
# Alternatively, install individually:
# pip install requests beautifulsoup4 pandas selenium webdriver-manager fake_useragent streamlit altair fpdf urllib.robotparser
ScraperAPI Key:
Obtain a ScraperAPI key by signing up at ScraperAPI.
You'll need to configure this key within your amazon_scraper.py (e.g., by setting an environment variable or directly in the code).
🚀 How to Run
Start the Streamlit application:
Bash

streamlit run app.py
Open your web browser and navigate to the local URL provided by Streamlit (e.g., http://localhost:8501).
Use the interactive interface to input search queries, specify the number of pages to crawl, and initiate the Amazon product scraping process. Results will be displayed and can be exported.
🤝 Contribution
Contributions to enhance this project are welcome! Feel free to open issues for bug reports or feature requests, or submit pull requests with improvements.
