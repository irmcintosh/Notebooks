# NC Electric Cooperatives Outage Scraper

This project uses **Selenium** and **BeautifulSoup** in a **Google Colab** environment to scrape outage information from the NC Electric Cooperatives website and save the data to Google Drive in a CSV format.

## Project Overview

The script performs the following steps:
1. Sets up the necessary environment by installing dependencies.
2. Initializes a headless Chrome browser using Selenium and accesses the NC Electric Cooperatives outage page.
3. Extracts information about county-specific power outages, including:
   - County name
   - Number of members affected
   - Utility details
4. Saves the data to a DataFrame and exports it as a CSV file to Google Drive.

## Dependencies

The following packages are required to run this code:

- `wget`
- `unzip`
- `selenium`
- `webdriver-manager`
- `xvfb`
- `pyvirtualdisplay`
- `beautifulsoup4`
- `pandas`

All dependencies are automatically installed at the start of the script.

## Installation

Clone this repository and open it in **Google Colab**. To run the script, make sure that:

1. Google Chrome is installed.
2. All dependencies are installed as specified at the start of the script.

### Instructions for Colab Setup

1. **Mount Google Drive** to save the output CSV file.
2. **Run all cells** in order.

## Usage

The script is configured to automatically:

1. Initialize a headless Chrome browser.
2. Access the NC Electric Cooperatives outage information page.
3. Scrape the relevant data for counties with outage details.
4. Store the data in a DataFrame.
5. Export the DataFrame to a CSV file in your Google Drive.

### CSV Output

The CSV file `outage_details_by_county.csv` will be saved in Google Drive under the specified path:
```plaintext
/content/drive/My Drive/outage_details_by_county.csv
