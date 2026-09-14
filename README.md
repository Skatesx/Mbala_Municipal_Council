# Mbala Municipal Council Dataset

## 1. Project Overview

This project presents a curated dataset containing important information
associated with Mbala Municipal Council in Zambia.

The dataset was created as part of the CSC 4792: Data Mining and Warehousing
Mini Project, Project Team #17.

## 2. Data Source

The primary source of the dataset is the official Mbala Municipal Council
website:

https://www.mbalacouncil.gov.zm/

The data was collected from publicly available council webpages and
documents.

## 3. Dataset Contents

The dataset contains information extracted from the council's digital
footprints, including council pages, publications, projects and other
relevant municipal information.

The dataset includes fields such as:

- URL
- Page ID
- Post ID
- Title
- Date
- Topics
- Text content
- Text length
- Record type

## 4. Data Collection

Data was collected from the official Mbala Municipal Council website using
web extraction/scraping techniques.

The raw data is preserved in:

data/raw/

The cleaned dataset is stored in:

data/

## 5. Data Cleaning and Preprocessing

The raw data was inspected and cleaned before analysis.

The preprocessing included:

- Checking for missing values
- Identifying and removing duplicate records
- Cleaning unnecessary whitespace
- Converting identifiers to appropriate data types
- Validating text content
- Validating text-length values
- Adding a record type classification
- Preserving source information where values were missing or non-standard

The final cleaned dataset is provided as a pipe-separated CSV file.

## 6. Repository Structure

text
data/
├── db-unza26-csc4792-mbala_municipal_council_cleaned.csv
└── raw/
    └── db-unza26-csc4792-mbala_municipal_council_pages.csv

documents/

figures/

notebooks/
└── db-unza26-csc4792-mbala_municipal_council.ipynb

7. Notebook
The Jupyter notebook documents the data extraction, cleaning, preprocessing, validation and analysis process.
8. File Format
The datasets are provided in CSV format using the pipe character | as the column separator.

## 9. Project Team

**Project Team #17**

**Council:** Mbala Municipal Council

**Course:** CSC 4792: Data Mining and Warehousing

### Team Members

| Name | Student Number |
| Mwimba Njiko | 2021377229 |
| Isaac Simbeye | 2021381668 |
| Maliseni Chavula | — |
