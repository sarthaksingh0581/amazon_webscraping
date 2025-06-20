# Amazon Heater Price Tracker
> Smart Price Monitoring with Python Web Scraping and Email Notifications

---

## Project Overview

This project automates the process of tracking product prices on Amazon India and sending an email alert when the price drops below a defined threshold.

The tool was originally created to help my father purchase a heater at the most optimal price ([product link](https://amzn.in/d/0lfPSNQ)). It demonstrates how Python can be leveraged to develop practical automation solutions involving web scraping, data logging, and real-time alerts.

---

## Features

- Extracts the product title and current price from Amazon
- Sends automated email notifications when the price falls below ₹5000
- Logs each execution to a CSV file for historical price tracking
- Includes a sample screenshot of the email notification
- Easily extendable to support other products and price thresholds

---

## Project Structure

| File                           | Description                                         |
|--------------------------------|-----------------------------------------------------|
| `Amazon Web Scraper Project.ipynb` | Jupyter Notebook containing core scraping and email logic |
| `scraped_data.csv`             | CSV file logging product titles, prices, and timestamps |
| `email_sample.png`             | Screenshot of the price alert email                |
| `README.md`                    | Documentation and overview of the project          |

---

## How It Works

1. The script sends a request to a specified Amazon product URL.
2. It parses the HTML response using BeautifulSoup to extract the product title and price.
3. The current price is compared against a predefined threshold (₹5000).
4. If the price is below the threshold, an email alert is sent using the SMTP protocol.
5. Product data and timestamps are logged into a CSV file on each run.

---

## Potential Improvements

- Incorporate scraping of product reviews and ratings
- Enable support for multiple product URLs and comparison
- Schedule regular scraping jobs using cron (Linux/macOS) or Task Scheduler (Windows)
- Visualize historical pricing trends using libraries such as `matplotlib` or `seaborn`
- Expand compatibility to other e-commerce platforms like Flipkart

---

## Disclaimer

This project is intended strictly for personal and educational use. Please ensure compliance with Amazon’s [Terms of Service](https://www.amazon.in/gp/help/customer/display.html?nodeId=201909000) when using web scraping tools.

---

## Author

**Sarthak Singh**  
Python Developer | Data Automation Enthusiast  
[LinkedIn Profile](https://www.linkedin.com/in/sarthak-singh-4a2738358/)  
Email alerts powered by Python and SMTP automation

