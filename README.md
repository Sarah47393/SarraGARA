# SarahGARA
README for TechnicalTest Notebook
Requirements :
- Python 3.x
-Jupyter Notebook
-Required Python libraries: os, random, datetime, timedelta, glob, collections

Part 1: Generating Log Files Randomly
Overview: The "TechnicalTest" notebook aims to generate random log files containing song streaming data. Each log file follows the format: sng_id | user_id | country. This notebook is designed as a solution to the technical test where real log data was not provided. It provides a function to generate a single log file and another function to generate multiple log files over consecutive days.
Why Randomly Generating Log Files? Since real log files were not provided in the technical test, I implemented a random log file generation approach to demonstrate the log analysis process. This allowed me to showcase the analysis code on synthetic data and test its performance and functionality.
Part 2: Log File Analysis - Top 50 Songs by Country
The notebook continues to perform log file analysis on the generated log files. It processes the log files to compute the top 50 songs per country based on their stream counts. The analysis considers the last 7 log files, and the output is saved in a file named "country_top50_yyyymmdd.txt" in a folder named "country_top50".

How to Use:
1-Open the "TechnicalTest" notebook in Jupyter Notebook.
2-Execute the notebook to generate the desired number of log files.
3-By default, the log files will be saved in a folder named "sample_listen_2Generated".
4-The analysis will compute the top 50 songs per country based on the log data from the last 7 log files.
5-The output file "country_top50_yyyymmdd.txt" will be saved in the "country_top50" folder.

Running on Linux: To run the notebook on Linux, follow these steps:
1-Ensure you have Python 3.x and Jupyter Notebook installed on your Linux system.
2-Download or clone the repository containing the notebook files.
3-Open a terminal and navigate to the directory where the notebook files are located.
4-Launch Jupyter Notebook by running the command: jupyter notebook
5-In the Jupyter Notebook interface, click on the "TechnicalTest" notebook to open it.
6-Execute the notebook cells to generate the log files and perform the log file analysis.

README for Testing_Corrupted_Data Notebook

Generating Log File With Corrupted Data
Overview: The "Testing_Corrupted_Data" notebook aims to create a log file with corrupted data for testing purposes. The log file will be generated with intentionally introduced errors, such as missing rows and missing values, simulating scenarios where log data may not strictly adhere to the expected format. This notebook is designed to demonstrate how the log analysis script from the "TechnicalTest" notebook can handle and process such corrupted log data.

How to Use:
1-Open the "Testing_Corrupted_Data" notebook in Jupyter Notebook.
2-Execute the notebook to generate the log file with corrupted data.
3-The log file will be saved in a folder named "sample_listen_custom".
4-The generated log file will contain four log entries, intentionally introducing errors to test the log analysis script.

Intentional Errors Introduced in the Log File:
1-First Log Entry: Correct format with valid song_id, user_id, and country.
2-Second Log Entry: Correct format with valid song_id, user_id, and country.
3-Third Log Entry: Missing row with only song_id and user_id, simulating a data inconsistency.
4-Fourth Log Entry: Missing user_id value, simulating incomplete data for a song.

Purpose: 
The purpose of this notebook is to demonstrate that the log analysis script from the "TechnicalTest" notebook can effectively handle log files with corrupted data. By processing the log file with intentional errors, we can observe how the script skips rows with missing values and continues analyzing the valid log entries.

Author: Sarra GARA 
Email: garasarra68@gmail.com 
