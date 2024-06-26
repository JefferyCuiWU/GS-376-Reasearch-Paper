# GS-376-Reasearch-Paper
This repository is for our group's research on GS 376 course. It contains the data collected and python scripts used to process the data.

## Usage

- [parsing_pdf_files.py](parsing_pdf_files.py) is for reading the PDF files that contain the HS 8 code of products that China had imposed additional tariffs on.
It prints out the HS 6 code of products that had additional tariffs of one PDF file.

- [tariff_visualization.py](tariff_visualization.py) is for reading the word document we collected that contains names tariff waves, HS 6 code of products that had additional tariffs, and the amount of additional tariffs in percentages.
It saves a file that contains HS 6 code of products that had additional tariffs, and the amount of additional tariffs in percentages, and the year the additional tariffs were imposed.

- [value_quantity_processing.py](value_quantity_processing.py) is for processing the data collected from China Customs.
It reads through a folder containing data of values and quantities in each year, calculates the prices by dividing the values with the quantities, and saves three excel files (one for prices only, one for prices and values, and one for prices, quantites and values).

- [value_quantity_visualization.py](value_quantity_visualization.py) is for visualizing the data of prices, quantities and values.
It reads the files generated by [tariff_visualization.py](tariff_visualization.py) and ([value_quantity_processing.py](value_quantity_processing.py), plots two graphs [Proportional Change in Average Import Prices by Tariff Wave from 2015 to 2021](Results/Proportional%20Change%20in%20Average%20Import%20Prices%20by%20Tariff%20Wave%20from%202015%20to%202021.png) and [Proportional Change in Total Import Values by Tariff Wave from 2015 to 2021](Results/Proportional%20Change%20in%20Total%20Import%20Values%20by%20Tariff%20Wave%20from%202015%20to%202021.png)), and runs a panel data regression.

## Sources

- Data of import values and import quantities are from China Customs.

- Data of additional tariffs imposed are from WTO and China Ministry of Finance.
