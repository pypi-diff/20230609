# Comparing `tmp/spoiltracker-0.0.8.tar.gz` & `tmp/spoiltracker-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spoiltracker-0.0.8.tar", last modified: Tue Jun  6 17:08:39 2023, max compression
+gzip compressed data, was "spoiltracker-0.0.9.tar", last modified: Fri Jun  9 04:22:54 2023, max compression
```

## Comparing `spoiltracker-0.0.8.tar` & `spoiltracker-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-06-06 17:08:39.161816 spoiltracker-0.0.8/
--rw-r--r--   0 bloom      (501) staff       (20)     1044 2023-06-06 15:14:11.000000 spoiltracker-0.0.8/LICENSE
--rw-r--r--   0 bloom      (501) staff       (20)    10092 2023-06-06 17:08:39.161675 spoiltracker-0.0.8/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)     9503 2023-06-06 17:06:31.000000 spoiltracker-0.0.8/README.md
--rw-r--r--   0 bloom      (501) staff       (20)      509 2023-06-06 17:08:15.000000 spoiltracker-0.0.8/pyproject.toml
--rw-r--r--   0 bloom      (501) staff       (20)       38 2023-06-06 17:08:39.161855 spoiltracker-0.0.8/setup.cfg
--rw-r--r--   0 bloom      (501) staff       (20)      830 2023-06-06 17:08:03.000000 spoiltracker-0.0.8/setup.py
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-06-06 17:08:39.160416 spoiltracker-0.0.8/src/
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-06-06 17:08:39.161524 spoiltracker-0.0.8/src/spoiltracker.egg-info/
--rw-r--r--   0 bloom      (501) staff       (20)    10092 2023-06-06 17:08:39.000000 spoiltracker-0.0.8/src/spoiltracker.egg-info/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)      201 2023-06-06 17:08:39.000000 spoiltracker-0.0.8/src/spoiltracker.egg-info/SOURCES.txt
--rw-r--r--   0 bloom      (501) staff       (20)        1 2023-06-06 17:08:39.000000 spoiltracker-0.0.8/src/spoiltracker.egg-info/dependency_links.txt
--rw-r--r--   0 bloom      (501) staff       (20)        1 2023-06-06 17:08:39.000000 spoiltracker-0.0.8/src/spoiltracker.egg-info/top_level.txt
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-06-09 04:22:54.516391 spoiltracker-0.0.9/
+-rw-r--r--   0 bloom      (501) staff       (20)     1044 2023-06-09 02:47:41.000000 spoiltracker-0.0.9/LICENSE
+-rw-r--r--   0 bloom      (501) staff       (20)     9745 2023-06-09 04:22:54.516260 spoiltracker-0.0.9/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)     9188 2023-06-09 04:21:52.000000 spoiltracker-0.0.9/README.md
+-rw-r--r--   0 bloom      (501) staff       (20)      524 2023-06-09 04:21:26.000000 spoiltracker-0.0.9/pyproject.toml
+-rw-r--r--   0 bloom      (501) staff       (20)       38 2023-06-09 04:22:54.516518 spoiltracker-0.0.9/setup.cfg
+-rw-r--r--   0 bloom      (501) staff       (20)      846 2023-06-09 04:21:18.000000 spoiltracker-0.0.9/setup.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-06-09 04:22:54.515168 spoiltracker-0.0.9/src/
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-06-09 04:22:54.516103 spoiltracker-0.0.9/src/spoiltracker.egg-info/
+-rw-r--r--   0 bloom      (501) staff       (20)     9745 2023-06-09 04:22:54.000000 spoiltracker-0.0.9/src/spoiltracker.egg-info/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)      201 2023-06-09 04:22:54.000000 spoiltracker-0.0.9/src/spoiltracker.egg-info/SOURCES.txt
+-rw-r--r--   0 bloom      (501) staff       (20)        1 2023-06-09 04:22:54.000000 spoiltracker-0.0.9/src/spoiltracker.egg-info/dependency_links.txt
+-rw-r--r--   0 bloom      (501) staff       (20)        1 2023-06-09 04:22:54.000000 spoiltracker-0.0.9/src/spoiltracker.egg-info/top_level.txt
```

### Comparing `spoiltracker-0.0.8/LICENSE` & `spoiltracker-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spoiltracker-0.0.8/PKG-INFO` & `spoiltracker-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: spoiltracker
-Version: 0.0.8
-Summary: A Simple Expiry Management System
+Version: 0.0.9
+Summary: A Simple Product Expiration Date Management Tool
 Home-page: https://github.com/psibir/spoiltracker
 Author: psibir
-Author-email: Trevor Bloomfield <bloomfieldtm@gmail.com>
-Project-URL: Homepage, https://github.com/psibir/spoiltracker
-Project-URL: Bug Tracker, https://github.com/psibir/spoilertracker/issues
+Author-email: bloomfieldtm@gmail.com
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/psibir/spoiltracker/issues
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # spoiltracker
 
-![spoiltracker logo](/spoiltracker_logo.png)
+![spoiltracker logo](https://github.com/psibir/psibir.github.io/blob/main/assets/images/spoiltracker_logo.png?raw=true)
 
 Spoiltracker is a Python package that helps track the expiration dates of products. It calculates expiration dates based on the production dates and shelf life information and generates an expiry report for products that are approaching their expiration dates.
 
-## Simple Product Expiry Management
+## A Simple Product Expiration Date Management Tool
 
 Spoiltracker is useful for businesses that deal with perishable products and need to keep track of their expiration dates. It can be used in various industries such as food and beverage, agriculture, perishable goods logistics, warehousing, pharmaceuticals, and cosmetics. The package helps businesses to:
 
 - Maintain a record of product SKUs, names, brands, and expiration dates.
 - Calculate expiration dates based on the production dates and shelf life information.
 - Generate an expiry report that lists products approaching their expiration dates within a specified number of days.
 - Remove expired entries from the history file to keep the record up to date.
@@ -42,134 +43,169 @@
 
 - Ensure product quality and safety: Maintaining accurate and up-to-date records of product expiration dates is crucial for ensuring product quality and safety. Spoiltracker allows businesses to monitor and manage expiration dates effectively, reducing the risk of serving or selling expired products to customers. By staying on top of product freshness, businesses can enhance customer satisfaction and reputation.
 
 - Streamline operations: Spoiltracker streamlines the process of managing product expiration dates. With its ability to remove expired entries from the history file and clear the history file, businesses can maintain a clean and organized record of products. This streamlines operations, making it easier for deli and cheese counter staff to access information, plan for product usage, and maintain compliance with food safety regulations.
 
 ## Installation
 
-The package can be installed using pip:
+To install Spoiltracker, follow these steps:
 
-```shell
-pip install spoiltracker
-```
+1. Clone the repository from GitHub:
 
-## Usage
+   ```shell
+   git clone https://github.com/psibir/spoiltracker.git
+   ```
 
-Spoiltracker can be used from the command line or integrated into other Python scripts.
+2. Navigate to the `spoiltracker/src` directory:
 
-### Command Line Usage
+   ```shell
+   cd spoiltracker/src
+   ```
 
-To use Spoiltracker from the command line, run the following command:
+3. Create a virtual environment and install the required dependencies:
 
-```shell
-python -m spoiltracker [csv_file] [production_date] [--days DAYS] [--remove-expired] [--expiry-report-dest FILE] [--clear-history]
-```
+   ```shell
+   python -m venv .venv
+   source .venv/bin/activate
+   pip install -r requirements.txt
+   ```
 
-- `[csv_file]` (optional): The path to the CSV file containing the product data. If not provided, Spoiltracker will generate an expiry report based on the existing history file.
-- `[production_date]` (optional): The production date in the format "YYYY-MM-DD". If not provided, Spoiltracker will generate an expiry report based on the existing history file.
-- `--days DAYS` (optional): The threshold for the number of days until expiration. Default is 3 days.
-- `--remove-expired` (optional): Flag to remove expired entries from the history file and clear the expiry report file.
-- `--expiry-report-dest FILE` (optional): Destination file for the expiry report. If not provided, the default file "expiryreport.csv" will be used.
-- `--clear-history` (optional): Flag to clear the history file.
+4. Run the `spoiltracker.py` script:
 
-### Python Script Integration
+   ```shell
+   python spoiltracker.py
+   ```
 
-To use Spoiltracker in a Python script, you can import the `ExpiryTracker` class and create an instance of it. Then, call the `run` method with the desired parameters.
+   This will execute the SpoilerTracker script.
 
-```python
-from spoiltracker import ExpiryTracker
+The package can also be installed using pip:
 
-expiry_tracker = ExpiryTracker()
-expiry_tracker.run(csv_file="sku_list.csv", production_date="2023-06-01", days=5, remove_expired=True)
+```shell
+pip install spoiltracker
 ```
 
-### Shelf Life Data
+## Usage
 
-Spoiltracker requires shelf life data to calculate expiration dates. By default, it expects a CSV file named "shelflife.csv" in the same directory as the script or package using Spoiltracker. The file should have the following columns: SKU, Name, Brand, Shelf Life (in days).
+### Single CSV Processing
 
-```csv
-SKU,Name,Brand,Shelf Life
-123,Product 1,Brand 1,10
-456,Product 2,Brand 2,7
+To process a single CSV file, use the `--csv_file` and `--production_date` arguments. Specify the path to the CSV file and the production date in the format `YYYY-MM-DD`.
+
+```bash
+spoiltracker --csv_file path/to/file.csv --production_date 2023-06-01
 ```
 
-You can customize the shelf life file path by providing it when creating an instance of `ExpiryTracker`.
+This command will process the specified CSV file, calculate the expiration dates based on the shelf life data, and append the results to the history file.
 
-```python
-expiry_tracker = ExpiryTracker(shelf_life_file="custom_shelflife.csv")
+### Batch Processing
+
+To batch process multiple CSV files, place the files in a directory and use the `--batch` argument to specify the directory path. The files in the directory must be named in the format `YYYY-MM-DD.csv`, representing the production dates.
+
+```bash
+spoiltracker --batch path/to/directory
 ```
 
-## Functions
+SpoilTracker will process each CSV file in the batch, calculate the expiration dates, and append the results to the history file.
 
-- Load Shelf Life Data:
-  - The script automatically loads the shelf life data from the `shelflife.csv` file.
+### Expiry Report
 
-- Process CSV File:
-  - Specify the input CSV file and the production date using the `--csv-file` and `--production-date` options.
-  - The script calculates the expiration dates for the products and writes the data to the history file.
+To generate an expiry report, use the `--days` argument to set the threshold for the number of days until expiration. By default, SpoilTracker uses a threshold of 3 days. The expiry report includes the SKUs, names, brands, and expiration dates of the products that fall within the specified threshold.
 
-- Generate Expiry Report:
-  - By default, the script generates an expiry report for products expiring within the next 3 days.
-  - Use the `--days` option to specify a different threshold for the number of days until expiration.
-  - The report is saved in the `expiryreport.csv` file (or a custom destination if specified).
+```bash
+spoiltracker --days 5
+```
 
-- Remove Expired Entries:
-  - Use the `--remove-expired` option to remove expired entries from the history file and clear the expiry report file.
+The expiry report will be saved in the default output file `./output/expiryreport.csv`. You can also specify a custom output file using the `--output-dest` argument.
 
-- Clear History File:
-  - Use the `--clear-history` option to clear the history file.
+### Clearing Expired Entries
 
-By running the script with different combinations of these functionalities and adjusting the command-line options accordingly, you can effectively manage product expiration dates, generate reports, and maintain an up-to-date history of your products.
+If you want to remove expired entries from the history file and clear the expiry report file, use the `--clear-expired` flag.
 
-## Methods
+```bash
+spoiltracker --clear-expired
+```
 
-Spoiltracker provides the following functionality:
+This command will remove expired entries from the history file and clear the expiry report file.
 
-### Load Shelf Life Data
+### Clearing History File
 
-The `load_shelf_life_data` method loads the shelf life data from the shelf life file. It
+To clear the history file, use the `--clear-history` flag.
 
- reads the CSV file and stores the data in memory for later use.
+```bash
+spoiltracker --clear-history
+```
 
-### Calculate Expiration Date
+This command will clear the history file, removing all entries.
 
-The `calculate_expiration_date` method calculates the expiration date based on the production date and shelf life information. It takes the production date and the shelf life as input and returns the expiration date.
+### Outputting a Pretty-Printed Expiry Report
 
-### Write to History CSV
+To output a pretty-printed expiry report as a text file, use the `--table` flag.
 
-The `write_to_history_csv` method writes data to the history CSV file. It takes a list of data as input, appends it to the existing file, and creates a new file if it doesn't exist.
+```bash
+spoiltracker --table
+```
 
-### Write to Expiry Report
+This command will generate the expiry report and save it as `./output/expiryreport.txt`. The text file will contain a nicely formatted table with the SKUs, names, brands, and expiration dates of the products that fall within the specified threshold.
 
-The `write_to_expiry_report` method generates an expiry report based on the data provided. It compares the expiration dates with the current date and the specified threshold (number of days). It writes the report to the expiry report file, appending new entries and creating a new file if it doesn't exist.
+## Method Descriptions
 
-### Sort Expiry Report
+The SpoilTracker package provides the following methods:
 
-The `sort_expiry_report` method is responsible for sorting the entries in the expiry report based on the expiration date. It takes the `expiry_report_dest` parameter, which represents the path to the expiry report file.
+- `load_shelf_life_data()`: Loads the shelf life data from the shelf life file.
+- `calculate_expiration_date(production_date, shelf_life)`: Calculates the expiration date based on the production date and shelf life.
+- `append_to_history(data)`: Appends data to the history file.
+- `append_to_expiry_report(data, days, output_dest=None)`: Appends data to the expiry report file for products that fall within the specified threshold.
+- `sort_expiry_report(output_dest)`: Sorts the expiry report file by expiration date.
+- `generate_expiry_report(days, output_dest=None)`: Generates the expiry report for products that fall within the specified threshold.
+- `clear_expired_entries()`: Removes expired entries from the history file and clears the expiry report file.
+- `clear_history_file()`: Clears the history file.
+- `process_csv(csv_file_path, prod_date)`: Processes a CSV file, calculates expiration dates, and returns the processed data.
+- `print_table(output_dest=None, show_console=False)`: Prints a pretty-formatted table of the expiry report and saves it as a text file.
+- `run(csv_file=None, production_date=None, days=3, clear_expired=False, output_dest=None, clear_history=False, print_table=False)`: Runs the SpoilTracker functionality based on the provided arguments.
 
-### Generate Expiry Report
+### Python Script Integration
 
-The `generate_expiry_report` method generates an expiry report based on the existing history file. It reads the history file, filters the entries that are approaching their expiration dates within the specified number of days, and writes the report to the expiry report file.
+To use Spoiltracker in a Python script, you can import the `ExpiryTracker` class and create an instance of it. Then, call the `run` method with the desired parameters.
 
-### Remove Expired Entries
+```python
+from spoiltracker import ExpiryTracker
 
-The `remove_expired_entries` method removes expired entries from the history file. It reads the expiry report file to get the SKUs of expired products and filters out those entries from the history file. It also clears the expiry report file.
+expiry_tracker = ExpiryTracker()
+expiry_tracker.run(csv_file="sku_list.csv", production_date="2023-06-01", days=5, remove_expired=True)
+```
 
-### Clear History File
+## Customize Shelf Life Data
 
-The `clear_history_file` method clears the history file by removing all its contents.
+Spoiltracker requires shelf life data to calculate expiration dates. By default, it expects a CSV file named "shelflife.csv" in the `./csv` directory. The file should have the following columns: SKU, Name, Brand, "Shelf Life" (in days).
 
-### Process CSV
+```csv
+SKU,Name,Brand,Shelf Life
+123,Product 1,Brand 1,10
+456,Product 2,Brand 2,7
+```
 
-The `process_csv` method processes the provided CSV file and generates the history data. It reads the CSV file, retrieves the shelf life information for each SKU, calculates the expiration dates, and writes the data to the history file. It returns the history data.
+You can customize the shelf life file path by providing it when creating an instance of `ExpiryTracker`.
+
+```python
+expiry_tracker = ExpiryTracker(shelf_life_file="custom_shelflife.csv")
+```
 
-### Run
+## Dependencies
 
-The `run` method is the main entry point for using Spoiltracker. It accepts command line arguments or direct parameters and executes the necessary functions based on the provided options.
+SpoilTracker has the following dependencies:
 
-### Error Handling
+- `argparse`: For parsing command-line arguments.
+- `csv`: For reading and writing CSV files.
+- `os`: For working with file paths and directories.
+- `datetime`, `timedelta`: For working with dates and calculating expiration dates.
+- `tabulate`: For generating formatted tables.
 
-Spoiltracker provides basic error handling for file not found errors and invalid date formats. If the shelf life file, history file, or expiry report file is not found, an error message is displayed. If an invalid date format is encountered in the CSV files, an error message is displayed as well.
+Make sure to install these dependencies before using SpoilTracker.
 
 ## Contributions
 
 See [Contributions](/CONTRIBUTIONS).
+
+## License
+
+See [License](/LICENSE).
+
+
```

### Comparing `spoiltracker-0.0.8/README.md` & `spoiltracker-0.0.9/src/spoiltracker.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,31 @@
+Metadata-Version: 2.1
+Name: spoiltracker
+Version: 0.0.9
+Summary: A Simple Product Expiration Date Management Tool
+Home-page: https://github.com/psibir/spoiltracker
+Author: psibir
+Author-email: bloomfieldtm@gmail.com
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/psibir/spoiltracker/issues
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # spoiltracker
 
-![spoiltracker logo](/spoiltracker_logo.png)
+![spoiltracker logo](https://github.com/psibir/psibir.github.io/blob/main/assets/images/spoiltracker_logo.png?raw=true)
 
 Spoiltracker is a Python package that helps track the expiration dates of products. It calculates expiration dates based on the production dates and shelf life information and generates an expiry report for products that are approaching their expiration dates.
 
-## Simple Product Expiry Management
+## A Simple Product Expiration Date Management Tool
 
 Spoiltracker is useful for businesses that deal with perishable products and need to keep track of their expiration dates. It can be used in various industries such as food and beverage, agriculture, perishable goods logistics, warehousing, pharmaceuticals, and cosmetics. The package helps businesses to:
 
 - Maintain a record of product SKUs, names, brands, and expiration dates.
 - Calculate expiration dates based on the production dates and shelf life information.
 - Generate an expiry report that lists products approaching their expiration dates within a specified number of days.
 - Remove expired entries from the history file to keep the record up to date.
@@ -26,134 +43,169 @@
 
 - Ensure product quality and safety: Maintaining accurate and up-to-date records of product expiration dates is crucial for ensuring product quality and safety. Spoiltracker allows businesses to monitor and manage expiration dates effectively, reducing the risk of serving or selling expired products to customers. By staying on top of product freshness, businesses can enhance customer satisfaction and reputation.
 
 - Streamline operations: Spoiltracker streamlines the process of managing product expiration dates. With its ability to remove expired entries from the history file and clear the history file, businesses can maintain a clean and organized record of products. This streamlines operations, making it easier for deli and cheese counter staff to access information, plan for product usage, and maintain compliance with food safety regulations.
 
 ## Installation
 
-The package can be installed using pip:
+To install Spoiltracker, follow these steps:
 
-```shell
-pip install spoiltracker
-```
+1. Clone the repository from GitHub:
 
-## Usage
+   ```shell
+   git clone https://github.com/psibir/spoiltracker.git
+   ```
 
-Spoiltracker can be used from the command line or integrated into other Python scripts.
+2. Navigate to the `spoiltracker/src` directory:
 
-### Command Line Usage
+   ```shell
+   cd spoiltracker/src
+   ```
 
-To use Spoiltracker from the command line, run the following command:
+3. Create a virtual environment and install the required dependencies:
 
-```shell
-python -m spoiltracker [csv_file] [production_date] [--days DAYS] [--remove-expired] [--expiry-report-dest FILE] [--clear-history]
-```
+   ```shell
+   python -m venv .venv
+   source .venv/bin/activate
+   pip install -r requirements.txt
+   ```
 
-- `[csv_file]` (optional): The path to the CSV file containing the product data. If not provided, Spoiltracker will generate an expiry report based on the existing history file.
-- `[production_date]` (optional): The production date in the format "YYYY-MM-DD". If not provided, Spoiltracker will generate an expiry report based on the existing history file.
-- `--days DAYS` (optional): The threshold for the number of days until expiration. Default is 3 days.
-- `--remove-expired` (optional): Flag to remove expired entries from the history file and clear the expiry report file.
-- `--expiry-report-dest FILE` (optional): Destination file for the expiry report. If not provided, the default file "expiryreport.csv" will be used.
-- `--clear-history` (optional): Flag to clear the history file.
+4. Run the `spoiltracker.py` script:
 
-### Python Script Integration
+   ```shell
+   python spoiltracker.py
+   ```
 
-To use Spoiltracker in a Python script, you can import the `ExpiryTracker` class and create an instance of it. Then, call the `run` method with the desired parameters.
+   This will execute the SpoilerTracker script.
 
-```python
-from spoiltracker import ExpiryTracker
+The package can also be installed using pip:
 
-expiry_tracker = ExpiryTracker()
-expiry_tracker.run(csv_file="sku_list.csv", production_date="2023-06-01", days=5, remove_expired=True)
+```shell
+pip install spoiltracker
 ```
 
-### Shelf Life Data
+## Usage
 
-Spoiltracker requires shelf life data to calculate expiration dates. By default, it expects a CSV file named "shelflife.csv" in the same directory as the script or package using Spoiltracker. The file should have the following columns: SKU, Name, Brand, Shelf Life (in days).
+### Single CSV Processing
 
-```csv
-SKU,Name,Brand,Shelf Life
-123,Product 1,Brand 1,10
-456,Product 2,Brand 2,7
+To process a single CSV file, use the `--csv_file` and `--production_date` arguments. Specify the path to the CSV file and the production date in the format `YYYY-MM-DD`.
+
+```bash
+spoiltracker --csv_file path/to/file.csv --production_date 2023-06-01
 ```
 
-You can customize the shelf life file path by providing it when creating an instance of `ExpiryTracker`.
+This command will process the specified CSV file, calculate the expiration dates based on the shelf life data, and append the results to the history file.
 
-```python
-expiry_tracker = ExpiryTracker(shelf_life_file="custom_shelflife.csv")
+### Batch Processing
+
+To batch process multiple CSV files, place the files in a directory and use the `--batch` argument to specify the directory path. The files in the directory must be named in the format `YYYY-MM-DD.csv`, representing the production dates.
+
+```bash
+spoiltracker --batch path/to/directory
 ```
 
-## Functions
+SpoilTracker will process each CSV file in the batch, calculate the expiration dates, and append the results to the history file.
 
-- Load Shelf Life Data:
-  - The script automatically loads the shelf life data from the `shelflife.csv` file.
+### Expiry Report
 
-- Process CSV File:
-  - Specify the input CSV file and the production date using the `--csv-file` and `--production-date` options.
-  - The script calculates the expiration dates for the products and writes the data to the history file.
+To generate an expiry report, use the `--days` argument to set the threshold for the number of days until expiration. By default, SpoilTracker uses a threshold of 3 days. The expiry report includes the SKUs, names, brands, and expiration dates of the products that fall within the specified threshold.
 
-- Generate Expiry Report:
-  - By default, the script generates an expiry report for products expiring within the next 3 days.
-  - Use the `--days` option to specify a different threshold for the number of days until expiration.
-  - The report is saved in the `expiryreport.csv` file (or a custom destination if specified).
+```bash
+spoiltracker --days 5
+```
 
-- Remove Expired Entries:
-  - Use the `--remove-expired` option to remove expired entries from the history file and clear the expiry report file.
+The expiry report will be saved in the default output file `./output/expiryreport.csv`. You can also specify a custom output file using the `--output-dest` argument.
 
-- Clear History File:
-  - Use the `--clear-history` option to clear the history file.
+### Clearing Expired Entries
 
-By running the script with different combinations of these functionalities and adjusting the command-line options accordingly, you can effectively manage product expiration dates, generate reports, and maintain an up-to-date history of your products.
+If you want to remove expired entries from the history file and clear the expiry report file, use the `--clear-expired` flag.
 
-## Methods
+```bash
+spoiltracker --clear-expired
+```
 
-Spoiltracker provides the following functionality:
+This command will remove expired entries from the history file and clear the expiry report file.
 
-### Load Shelf Life Data
+### Clearing History File
 
-The `load_shelf_life_data` method loads the shelf life data from the shelf life file. It
+To clear the history file, use the `--clear-history` flag.
 
- reads the CSV file and stores the data in memory for later use.
+```bash
+spoiltracker --clear-history
+```
 
-### Calculate Expiration Date
+This command will clear the history file, removing all entries.
 
-The `calculate_expiration_date` method calculates the expiration date based on the production date and shelf life information. It takes the production date and the shelf life as input and returns the expiration date.
+### Outputting a Pretty-Printed Expiry Report
 
-### Write to History CSV
+To output a pretty-printed expiry report as a text file, use the `--table` flag.
 
-The `write_to_history_csv` method writes data to the history CSV file. It takes a list of data as input, appends it to the existing file, and creates a new file if it doesn't exist.
+```bash
+spoiltracker --table
+```
 
-### Write to Expiry Report
+This command will generate the expiry report and save it as `./output/expiryreport.txt`. The text file will contain a nicely formatted table with the SKUs, names, brands, and expiration dates of the products that fall within the specified threshold.
 
-The `write_to_expiry_report` method generates an expiry report based on the data provided. It compares the expiration dates with the current date and the specified threshold (number of days). It writes the report to the expiry report file, appending new entries and creating a new file if it doesn't exist.
+## Method Descriptions
 
-### Sort Expiry Report
+The SpoilTracker package provides the following methods:
 
-The `sort_expiry_report` method is responsible for sorting the entries in the expiry report based on the expiration date. It takes the `expiry_report_dest` parameter, which represents the path to the expiry report file.
+- `load_shelf_life_data()`: Loads the shelf life data from the shelf life file.
+- `calculate_expiration_date(production_date, shelf_life)`: Calculates the expiration date based on the production date and shelf life.
+- `append_to_history(data)`: Appends data to the history file.
+- `append_to_expiry_report(data, days, output_dest=None)`: Appends data to the expiry report file for products that fall within the specified threshold.
+- `sort_expiry_report(output_dest)`: Sorts the expiry report file by expiration date.
+- `generate_expiry_report(days, output_dest=None)`: Generates the expiry report for products that fall within the specified threshold.
+- `clear_expired_entries()`: Removes expired entries from the history file and clears the expiry report file.
+- `clear_history_file()`: Clears the history file.
+- `process_csv(csv_file_path, prod_date)`: Processes a CSV file, calculates expiration dates, and returns the processed data.
+- `print_table(output_dest=None, show_console=False)`: Prints a pretty-formatted table of the expiry report and saves it as a text file.
+- `run(csv_file=None, production_date=None, days=3, clear_expired=False, output_dest=None, clear_history=False, print_table=False)`: Runs the SpoilTracker functionality based on the provided arguments.
 
-### Generate Expiry Report
+### Python Script Integration
 
-The `generate_expiry_report` method generates an expiry report based on the existing history file. It reads the history file, filters the entries that are approaching their expiration dates within the specified number of days, and writes the report to the expiry report file.
+To use Spoiltracker in a Python script, you can import the `ExpiryTracker` class and create an instance of it. Then, call the `run` method with the desired parameters.
 
-### Remove Expired Entries
+```python
+from spoiltracker import ExpiryTracker
 
-The `remove_expired_entries` method removes expired entries from the history file. It reads the expiry report file to get the SKUs of expired products and filters out those entries from the history file. It also clears the expiry report file.
+expiry_tracker = ExpiryTracker()
+expiry_tracker.run(csv_file="sku_list.csv", production_date="2023-06-01", days=5, remove_expired=True)
+```
 
-### Clear History File
+## Customize Shelf Life Data
 
-The `clear_history_file` method clears the history file by removing all its contents.
+Spoiltracker requires shelf life data to calculate expiration dates. By default, it expects a CSV file named "shelflife.csv" in the `./csv` directory. The file should have the following columns: SKU, Name, Brand, "Shelf Life" (in days).
 
-### Process CSV
+```csv
+SKU,Name,Brand,Shelf Life
+123,Product 1,Brand 1,10
+456,Product 2,Brand 2,7
+```
 
-The `process_csv` method processes the provided CSV file and generates the history data. It reads the CSV file, retrieves the shelf life information for each SKU, calculates the expiration dates, and writes the data to the history file. It returns the history data.
+You can customize the shelf life file path by providing it when creating an instance of `ExpiryTracker`.
+
+```python
+expiry_tracker = ExpiryTracker(shelf_life_file="custom_shelflife.csv")
+```
 
-### Run
+## Dependencies
 
-The `run` method is the main entry point for using Spoiltracker. It accepts command line arguments or direct parameters and executes the necessary functions based on the provided options.
+SpoilTracker has the following dependencies:
 
-### Error Handling
+- `argparse`: For parsing command-line arguments.
+- `csv`: For reading and writing CSV files.
+- `os`: For working with file paths and directories.
+- `datetime`, `timedelta`: For working with dates and calculating expiration dates.
+- `tabulate`: For generating formatted tables.
 
-Spoiltracker provides basic error handling for file not found errors and invalid date formats. If the shelf life file, history file, or expiry report file is not found, an error message is displayed. If an invalid date format is encountered in the CSV files, an error message is displayed as well.
+Make sure to install these dependencies before using SpoilTracker.
 
 ## Contributions
 
 See [Contributions](/CONTRIBUTIONS).
+
+## License
+
+See [License](/LICENSE).
+
+
```

### Comparing `spoiltracker-0.0.8/setup.py` & `spoiltracker-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "spoiltracker",
-    version = "0.0.8",
+    version = "0.0.9",
     author = "psibir",
     author_email = "bloomfieldtm@gmail.com",
-    description = "Simple Product Expiry Management",
+    description = "A Simple Product Expiration Date Management Tool",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/psibir/spoiltracker",
     project_urls = {
         "Bug Tracker": "https://github.com/psibir/spoiltracker/issues",
     },
     classifiers = [
```

### Comparing `spoiltracker-0.0.8/src/spoiltracker.egg-info/PKG-INFO` & `spoiltracker-0.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,14 @@
-Metadata-Version: 2.1
-Name: spoiltracker
-Version: 0.0.8
-Summary: A Simple Expiry Management System
-Home-page: https://github.com/psibir/spoiltracker
-Author: psibir
-Author-email: Trevor Bloomfield <bloomfieldtm@gmail.com>
-Project-URL: Homepage, https://github.com/psibir/spoiltracker
-Project-URL: Bug Tracker, https://github.com/psibir/spoilertracker/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # spoiltracker
 
-![spoiltracker logo](/spoiltracker_logo.png)
+![spoiltracker logo](https://github.com/psibir/psibir.github.io/blob/main/assets/images/spoiltracker_logo.png?raw=true)
 
 Spoiltracker is a Python package that helps track the expiration dates of products. It calculates expiration dates based on the production dates and shelf life information and generates an expiry report for products that are approaching their expiration dates.
 
-## Simple Product Expiry Management
+## A Simple Product Expiration Date Management Tool
 
 Spoiltracker is useful for businesses that deal with perishable products and need to keep track of their expiration dates. It can be used in various industries such as food and beverage, agriculture, perishable goods logistics, warehousing, pharmaceuticals, and cosmetics. The package helps businesses to:
 
 - Maintain a record of product SKUs, names, brands, and expiration dates.
 - Calculate expiration dates based on the production dates and shelf life information.
 - Generate an expiry report that lists products approaching their expiration dates within a specified number of days.
 - Remove expired entries from the history file to keep the record up to date.
@@ -42,134 +26,167 @@
 
 - Ensure product quality and safety: Maintaining accurate and up-to-date records of product expiration dates is crucial for ensuring product quality and safety. Spoiltracker allows businesses to monitor and manage expiration dates effectively, reducing the risk of serving or selling expired products to customers. By staying on top of product freshness, businesses can enhance customer satisfaction and reputation.
 
 - Streamline operations: Spoiltracker streamlines the process of managing product expiration dates. With its ability to remove expired entries from the history file and clear the history file, businesses can maintain a clean and organized record of products. This streamlines operations, making it easier for deli and cheese counter staff to access information, plan for product usage, and maintain compliance with food safety regulations.
 
 ## Installation
 
-The package can be installed using pip:
+To install Spoiltracker, follow these steps:
 
-```shell
-pip install spoiltracker
-```
+1. Clone the repository from GitHub:
 
-## Usage
+   ```shell
+   git clone https://github.com/psibir/spoiltracker.git
+   ```
 
-Spoiltracker can be used from the command line or integrated into other Python scripts.
+2. Navigate to the `spoiltracker/src` directory:
 
-### Command Line Usage
+   ```shell
+   cd spoiltracker/src
+   ```
 
-To use Spoiltracker from the command line, run the following command:
+3. Create a virtual environment and install the required dependencies:
 
-```shell
-python -m spoiltracker [csv_file] [production_date] [--days DAYS] [--remove-expired] [--expiry-report-dest FILE] [--clear-history]
-```
+   ```shell
+   python -m venv .venv
+   source .venv/bin/activate
+   pip install -r requirements.txt
+   ```
 
-- `[csv_file]` (optional): The path to the CSV file containing the product data. If not provided, Spoiltracker will generate an expiry report based on the existing history file.
-- `[production_date]` (optional): The production date in the format "YYYY-MM-DD". If not provided, Spoiltracker will generate an expiry report based on the existing history file.
-- `--days DAYS` (optional): The threshold for the number of days until expiration. Default is 3 days.
-- `--remove-expired` (optional): Flag to remove expired entries from the history file and clear the expiry report file.
-- `--expiry-report-dest FILE` (optional): Destination file for the expiry report. If not provided, the default file "expiryreport.csv" will be used.
-- `--clear-history` (optional): Flag to clear the history file.
+4. Run the `spoiltracker.py` script:
 
-### Python Script Integration
+   ```shell
+   python spoiltracker.py
+   ```
 
-To use Spoiltracker in a Python script, you can import the `ExpiryTracker` class and create an instance of it. Then, call the `run` method with the desired parameters.
+   This will execute the SpoilerTracker script.
 
-```python
-from spoiltracker import ExpiryTracker
+The package can also be installed using pip:
 
-expiry_tracker = ExpiryTracker()
-expiry_tracker.run(csv_file="sku_list.csv", production_date="2023-06-01", days=5, remove_expired=True)
+```shell
+pip install spoiltracker
 ```
 
-### Shelf Life Data
+## Usage
 
-Spoiltracker requires shelf life data to calculate expiration dates. By default, it expects a CSV file named "shelflife.csv" in the same directory as the script or package using Spoiltracker. The file should have the following columns: SKU, Name, Brand, Shelf Life (in days).
+### Single CSV Processing
 
-```csv
-SKU,Name,Brand,Shelf Life
-123,Product 1,Brand 1,10
-456,Product 2,Brand 2,7
+To process a single CSV file, use the `--csv_file` and `--production_date` arguments. Specify the path to the CSV file and the production date in the format `YYYY-MM-DD`.
+
+```bash
+spoiltracker --csv_file path/to/file.csv --production_date 2023-06-01
 ```
 
-You can customize the shelf life file path by providing it when creating an instance of `ExpiryTracker`.
+This command will process the specified CSV file, calculate the expiration dates based on the shelf life data, and append the results to the history file.
 
-```python
-expiry_tracker = ExpiryTracker(shelf_life_file="custom_shelflife.csv")
+### Batch Processing
+
+To batch process multiple CSV files, place the files in a directory and use the `--batch` argument to specify the directory path. The files in the directory must be named in the format `YYYY-MM-DD.csv`, representing the production dates.
+
+```bash
+spoiltracker --batch path/to/directory
 ```
 
-## Functions
+SpoilTracker will process each CSV file in the batch, calculate the expiration dates, and append the results to the history file.
+
+### Expiry Report
 
-- Load Shelf Life Data:
-  - The script automatically loads the shelf life data from the `shelflife.csv` file.
+To generate an expiry report, use the `--days` argument to set the threshold for the number of days until expiration. By default, SpoilTracker uses a threshold of 3 days. The expiry report includes the SKUs, names, brands, and expiration dates of the products that fall within the specified threshold.
 
-- Process CSV File:
-  - Specify the input CSV file and the production date using the `--csv-file` and `--production-date` options.
-  - The script calculates the expiration dates for the products and writes the data to the history file.
+```bash
+spoiltracker --days 5
+```
 
-- Generate Expiry Report:
-  - By default, the script generates an expiry report for products expiring within the next 3 days.
-  - Use the `--days` option to specify a different threshold for the number of days until expiration.
-  - The report is saved in the `expiryreport.csv` file (or a custom destination if specified).
+The expiry report will be saved in the default output file `./output/expiryreport.csv`. You can also specify a custom output file using the `--output-dest` argument.
 
-- Remove Expired Entries:
-  - Use the `--remove-expired` option to remove expired entries from the history file and clear the expiry report file.
+### Clearing Expired Entries
 
-- Clear History File:
-  - Use the `--clear-history` option to clear the history file.
+If you want to remove expired entries from the history file and clear the expiry report file, use the `--clear-expired` flag.
 
-By running the script with different combinations of these functionalities and adjusting the command-line options accordingly, you can effectively manage product expiration dates, generate reports, and maintain an up-to-date history of your products.
+```bash
+spoiltracker --clear-expired
+```
 
-## Methods
+This command will remove expired entries from the history file and clear the expiry report file.
 
-Spoiltracker provides the following functionality:
+### Clearing History File
 
-### Load Shelf Life Data
+To clear the history file, use the `--clear-history` flag.
 
-The `load_shelf_life_data` method loads the shelf life data from the shelf life file. It
+```bash
+spoiltracker --clear-history
+```
 
- reads the CSV file and stores the data in memory for later use.
+This command will clear the history file, removing all entries.
 
-### Calculate Expiration Date
+### Outputting a Pretty-Printed Expiry Report
 
-The `calculate_expiration_date` method calculates the expiration date based on the production date and shelf life information. It takes the production date and the shelf life as input and returns the expiration date.
+To output a pretty-printed expiry report as a text file, use the `--table` flag.
 
-### Write to History CSV
+```bash
+spoiltracker --table
+```
 
-The `write_to_history_csv` method writes data to the history CSV file. It takes a list of data as input, appends it to the existing file, and creates a new file if it doesn't exist.
+This command will generate the expiry report and save it as `./output/expiryreport.txt`. The text file will contain a nicely formatted table with the SKUs, names, brands, and expiration dates of the products that fall within the specified threshold.
 
-### Write to Expiry Report
+## Method Descriptions
 
-The `write_to_expiry_report` method generates an expiry report based on the data provided. It compares the expiration dates with the current date and the specified threshold (number of days). It writes the report to the expiry report file, appending new entries and creating a new file if it doesn't exist.
+The SpoilTracker package provides the following methods:
 
-### Sort Expiry Report
+- `load_shelf_life_data()`: Loads the shelf life data from the shelf life file.
+- `calculate_expiration_date(production_date, shelf_life)`: Calculates the expiration date based on the production date and shelf life.
+- `append_to_history(data)`: Appends data to the history file.
+- `append_to_expiry_report(data, days, output_dest=None)`: Appends data to the expiry report file for products that fall within the specified threshold.
+- `sort_expiry_report(output_dest)`: Sorts the expiry report file by expiration date.
+- `generate_expiry_report(days, output_dest=None)`: Generates the expiry report for products that fall within the specified threshold.
+- `clear_expired_entries()`: Removes expired entries from the history file and clears the expiry report file.
+- `clear_history_file()`: Clears the history file.
+- `process_csv(csv_file_path, prod_date)`: Processes a CSV file, calculates expiration dates, and returns the processed data.
+- `print_table(output_dest=None, show_console=False)`: Prints a pretty-formatted table of the expiry report and saves it as a text file.
+- `run(csv_file=None, production_date=None, days=3, clear_expired=False, output_dest=None, clear_history=False, print_table=False)`: Runs the SpoilTracker functionality based on the provided arguments.
 
-The `sort_expiry_report` method is responsible for sorting the entries in the expiry report based on the expiration date. It takes the `expiry_report_dest` parameter, which represents the path to the expiry report file.
+### Python Script Integration
 
-### Generate Expiry Report
+To use Spoiltracker in a Python script, you can import the `ExpiryTracker` class and create an instance of it. Then, call the `run` method with the desired parameters.
 
-The `generate_expiry_report` method generates an expiry report based on the existing history file. It reads the history file, filters the entries that are approaching their expiration dates within the specified number of days, and writes the report to the expiry report file.
+```python
+from spoiltracker import ExpiryTracker
 
-### Remove Expired Entries
+expiry_tracker = ExpiryTracker()
+expiry_tracker.run(csv_file="sku_list.csv", production_date="2023-06-01", days=5, remove_expired=True)
+```
 
-The `remove_expired_entries` method removes expired entries from the history file. It reads the expiry report file to get the SKUs of expired products and filters out those entries from the history file. It also clears the expiry report file.
+## Customize Shelf Life Data
 
-### Clear History File
+Spoiltracker requires shelf life data to calculate expiration dates. By default, it expects a CSV file named "shelflife.csv" in the `./csv` directory. The file should have the following columns: SKU, Name, Brand, "Shelf Life" (in days).
 
-The `clear_history_file` method clears the history file by removing all its contents.
+```csv
+SKU,Name,Brand,Shelf Life
+123,Product 1,Brand 1,10
+456,Product 2,Brand 2,7
+```
 
-### Process CSV
+You can customize the shelf life file path by providing it when creating an instance of `ExpiryTracker`.
 
-The `process_csv` method processes the provided CSV file and generates the history data. It reads the CSV file, retrieves the shelf life information for each SKU, calculates the expiration dates, and writes the data to the history file. It returns the history data.
+```python
+expiry_tracker = ExpiryTracker(shelf_life_file="custom_shelflife.csv")
+```
 
-### Run
+## Dependencies
 
-The `run` method is the main entry point for using Spoiltracker. It accepts command line arguments or direct parameters and executes the necessary functions based on the provided options.
+SpoilTracker has the following dependencies:
 
-### Error Handling
+- `argparse`: For parsing command-line arguments.
+- `csv`: For reading and writing CSV files.
+- `os`: For working with file paths and directories.
+- `datetime`, `timedelta`: For working with dates and calculating expiration dates.
+- `tabulate`: For generating formatted tables.
 
-Spoiltracker provides basic error handling for file not found errors and invalid date formats. If the shelf life file, history file, or expiry report file is not found, an error message is displayed. If an invalid date format is encountered in the CSV files, an error message is displayed as well.
+Make sure to install these dependencies before using SpoilTracker.
 
 ## Contributions
 
 See [Contributions](/CONTRIBUTIONS).
+
+## License
+
+See [License](/LICENSE).
```

