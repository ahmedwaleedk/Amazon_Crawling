Amazon Product Scraper & Analyzer
This project is a powerful and ethical web crawling solution designed exclusively for extracting product data from Amazon.com. It leverages advanced techniques to navigate Amazon's dynamic website, reliably collect information, and provide an interactive platform for analysis.

🚀 Key Features
Robust Amazon Product Scraping:
Dynamic Content Handling: Uses Selenium to fully render complex, JavaScript-driven Amazon product pages, ensuring all data is accessible.
Anti-Bot Resilience: Integrates ScraperAPI to effectively handle proxy rotation, CAPTCHA challenges, and other anti-bot measures, ensuring consistent data retrieval.
Targeted Data Extraction: Precisely collects vital product details such as name, price, ratings, and comprehensive descriptions.
Efficient URL Discovery: Programmatically generates Amazon search URLs and intelligently extracts individual product links from search results pages.
Ethical Web Crawling Practices:
Strict robots.txt Compliance: Adheres rigorously to Amazon's robots.txt directives, meticulously avoiding all disallowed paths (e.g., shopping cart pages, private API endpoints).
Polite Delays: Implements a consistent 2-second delay between requests. This crucial practice prevents server overload and helps avoid detection by anti-bot systems.
Realistic User-Agents: Employs varied and realistic User-Agent strings to mimic genuine human Browse patterns.
Interactive Streamlit UI: Provides an intuitive web application that allows users to easily initiate crawls, visualize collected data, and generate informative reports.
Structured Data Output: Organizes extracted product information into clean, structured formats like CSV and PDF for seamless analysis and reporting.

  

🛠️ Technologies
Python: The core programming language powering the entire project.
requests: Used for making HTTP requests, primarily for robots.txt parsing.
BeautifulSoup4: Essential for efficient HTML parsing and extracting product links from search result pages.
selenium: Automates browser interactions, crucial for rendering dynamic content on Amazon product pages.
webdriver-manager: Simplifies managing browser drivers (like Chrome's ChromeDriver) for Selenium.
fake_useragent: Generates varied and realistic User-Agent strings for requests.
pandas: Used for powerful data manipulation, structuring the scraped information into DataFrames, and preparing it for output.
streamlit: The framework for building the interactive and user-friendly web application.
altair: Enables rich, declarative data visualizations within the Streamlit UI.
fpdf: Facilitates the generation of professional PDF reports from the collected data.
urllib.robotparser: A standard library module used for programmatic parsing and adherence to robots.txt rules.
ScraperAPI: A vital third-party service that manages proxies and handles anti-bot challenges, ensuring consistent access to Amazon's website.






🚀 How to Run
Launch the Streamlit web application:
Bash

streamlit run app.py
Open your web browser and navigate to the local URL provided by Streamlit (e.g., http://localhost:8501).
Utilize the interactive interface to input search queries, specify the desired number of pages to crawl, and initiate the Amazon product scraping process. The scraped data will be displayed within the app and can be exported as CSV or PDF reports.


🤝 Contribution
We welcome contributions to improve this project! If you have suggestions for new features, bug fixes, or enhancements, please feel free to open an issue or submit a pull request.

