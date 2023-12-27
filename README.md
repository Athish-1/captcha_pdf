# Crash Report Scraper

## Overview

This Python script automates the retrieval of crash reports from the Chicago Police Department's Driver Information Exchange website. It utilizes Selenium for web automation, TwoCaptcha for solving reCAPTCHA challenges, and pdfkit for converting HTML to PDF.

## Prerequisites

Before running the script, make sure you have the following installed:

- [Python](https://www.python.org/downloads/)
- [wkhtmltopdf](https://wkhtmltopdf.org/downloads.html) - Download the latest version and place the executable (`wkhtmltopdf.exe`) in the `wkhtmltopdf/bin` directory.

## 2Captcha API Key

To use the script, you'll need a 2Captcha API key. Follow these steps:

1. Visit [2Captcha](https://2captcha.com/) and sign up for an account.

2. After logging in, navigate to the "Dashboard" section.

3. Load your balance by selecting a payment method and completing the transaction.

4. Once your balance is loaded, go to the "API" section to find your API key.

## Installation

1. Install the required Python packages using the following command:

    ```bash
    pip install selenium twocaptcha pdfkit
    ```

2. Download the latest version of [wkhtmltopdf](https://wkhtmltopdf.org/downloads.html) and place the executable (`wkhtmltopdf.exe`) in the same directory as the `main.py` script.

## Usage

1. Open a terminal or command prompt in the script's directory.

2. Run the script using the following command:

    ```bash
    python main.py
    ```

3. Follow the prompts to enter the RD number prefix, start and end numbers, date, and your 2Captcha API key obtained in the previous steps.

4. The script will automate the process of accessing the crash report information, solving reCAPTCHA challenges using your 2Captcha API key, and saving the results as both HTML and PDF files in the script's directory.

## Notes

- The PDF and HTML files of the crash report will be saved in the same directory as the script.
- Ensure that the `wkhtmltopdf.exe` executable is in the `wkhtmltopdf/bin` directory.
- Make sure you have an active internet connection as the script interacts with an online service for solving reCAPTCHA challenges.

Feel free to reach out if you encounter any issues or have questions.
