# aliexpress-puppeteer

Dynamic Puppeteer Web Scraping for AliExpress

This project provides a scraping solution using **Puppeteer** to extract product information from **AliExpress** based on a given keyword. You can easily set up the scraper and use it to collect data dynamically from the website.

## Prerequisites

Before running the scraping script, make sure that you have the following installed on your system:

* **Node.js** (version 22.13.1)
* **npm** (version 10.9.2)

You can download and install both Node.js and npm from [Node.js official website](https://nodejs.org/).

## Setup and Installation

### Step 1: Clone the Repository

First, clone the repository to your local machine:

```bash
git clone https://github.com/p3nnatr4tion/aliexpress-puppeteer.git
```

### Step 2: Install Dependencies

Navigate to the project directory:

```bash
cd aliexpress-puppeteer
```

Install the required dependencies:

```bash
npm install
```

This will install **Puppeteer** and other dependencies defined in `package.json`.

### Step 3: Install Puppeteer Version 24.8.0

The project uses **Puppeteer 24.8.0**, which is specified in the `requirements.txt`. Install the required version using npm:

```bash
npm install puppeteer@24.8.0
```

### Step 4: Configure the Scraper

The core of the scraper is in the `scraper-starter.js` file. By default, it is set up to scrape data using the keyword `laptop` and scrape up to 1 page of results. You can modify these values by editing the file.

Open `scraper-starter.js` and change the values of the following variables to fit your scraping needs:

```javascript
const keyword = "laptop";   // Modify this value to your search keyword
const maxPage = 1;          // Modify this value to set the maximum number of pages to scrape
```

### Step 5: Run the Scraper

To run the scraper, execute the following command:

```bash
node scraper-starter.js
```

The script will open a headless browser, search for the specified keyword, and scrape product data from the first `maxPage` pages of results.

---

## How It Works

1. **Puppeteer** is used to control a headless browser and interact with the AliExpress website.
2. The scraper performs a search using the specified keyword.
3. It collects product information from the search results, such as product name, price, and link.
4. The script can scrape multiple pages by adjusting the `maxPage` value.

The results are outputted to the terminal (or can be modified to be saved into a file, such as CSV, for further analysis).

---

## Dependencies

* **Puppeteer**: A Node.js library for headless Chrome or Chromium scraping.

  * Version: 24.8.0 (specified in `requirements.txt`)

* **Node.js**: JavaScript runtime used to execute the scraping scripts.

  * Version: 22.13.1

* **npm**: Node.js package manager used to install dependencies.

  * Version: 10.9.2

---

## Notes

* **AliExpress Terms of Service**: Please make sure you comply with AliExpress’s [Terms of Service](https://www.aliexpress.com) before running the scraper.
* **Rate Limiting**: Be mindful of the rate at which you scrape AliExpress to avoid getting your IP blocked.
* **Headless Mode**: Puppeteer runs in headless mode by default, which means it doesn't open a visible browser window. You can change this behavior in the script if needed.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Let me know if you need further adjustments or improvements to this `README.md`!
