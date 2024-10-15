# ETL-System
### Overview
This project is designed to automate the process of compiling a list of the top 10 largest banks in the world by market capitalization, converting this data into multiple currencies, and storing the results in both a CSV file and an SQL database table. The code is intended to be executed on a quarterly basis to prepare financial reports.

### Key Features:
Data Extraction: Scrapes data from a Wikipedia page listing the largest banks by market capitalization.
Currency Conversion: Transforms the extracted data by converting market capitalization values from USD to GBP, EUR, and INR based on provided exchange rates.
Storage: Stores the final data in both a CSV file and an SQL database table.
Logging: Tracks the progress of the system execution through a log file for debugging and review purposes.

### Project Structure
* Etl_System.py - Main script that runs the entire process.
* exchange_rate.csv - CSV file containing exchange rate information (USD to GBP, EUR, INR).
* Largest_banks_data.csv - Output file where processed bank data is saved.
* Banks.db - SQLite database where bank data is stored.
* code_log.txt - Log file tracking the progress of the script at various stages.

### Setup
* Install the required Python libraries:
`pip install requests pandas beautifulsoup4 sqlite3`

* Download or clone this repository to your local machine.
Ensure you have internet access, as the project scrapes data from Wikipedia.
