# aliexpress-puppeteer

Dynamic Puppeteer Web Scraping for AliExpress

Scrape product data from AliExpress based on a given keyword using Puppeteer.

## Prerequisites

* **Node.js** (version 22.13.1)
* **npm** (version 10.9.2)

Install them from [Node.js official website](https://nodejs.org/).

## Setup and Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/p3nnatr4tion/aliexpress-puppeteer.git
   cd aliexpress-puppeteer
   ```

2. **Install dependencies**:

   ```bash
   npm install
   ```

3. **Install Puppeteer version 24.8.0**:

   ```bash
   npm install puppeteer@24.8.0
   ```

4. **Configure the scraper** in `scraper-starter.js`:
   Modify `keyword` and `maxPage` to your needs:

   ```javascript
   const keyword = "laptop";  // Search keyword
   const maxPage = 1;         // Max number of pages to scrape
   ```

5. **Run the scraper**:

   ```bash
   node scraper-starter.js
   ```

## Features

* **Stealth Plugin**: Avoids detection by using Puppeteer’s Stealth Plugin.
* **Tab Pooling**: Limits concurrent tabs to avoid overload, improving stability.
* **Retry Mechanism**: Retries failed operations up to 3 times.
* **Captcha Handling**: Automatically solves CAPTCHA challenges.
* **Random Delays**: Introduces random delays between requests to mimic human behavior.
* **Comprehensive Data**: Collects detailed product info such as title, price, specifications, images, reviews, shipping, and more.
* **Efficient Page Navigation**: Handles scrolling and pagination to collect data from multiple pages.

## Dependencies

* **Puppeteer**: Web scraping library (version 24.8.0)
* **Node.js** and **npm**

## Notes

* Make sure to comply with [AliExpress Terms of Service](https://www.aliexpress.com).
* Be mindful of rate limiting to avoid IP blocks.

## License

MIT License
