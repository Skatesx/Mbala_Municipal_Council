# Mbala Municipal Council Dataset

## 1. Project Overview

This project presents a curated dataset containing important information
associated with Mbala Municipal Council in Zambia.

The dataset was created as part of the CSC 4792: Data Mining and Warehousing
Mini Project, Project Team #17.

The project involved collecting, organizing, cleaning, preprocessing, validating, and documenting information obtained from the official Mbala Municipal Council website.

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

Field	       Description
url	           URL of the original Mbala Municipal Council webpage
page_id	       Identifier associated with the source page
post_id	       Identifier associated with the source post where available
title	       Title of the webpage or publication
date	       Date associated with the webpage or publication, where available
topics	       Topic or category information associated with the record
text_content   Extracted textual content from the source page
text_length_chars	Number of characters contained in the cleaned text content

## 4. Data Collection

Data was collected from the official Mbala Municipal Council website using
web extraction/scraping techniques.

The original/raw dataset is preserved in:

data/raw/

The processed and cleaned dataset is stored in:

data/processed/

Keeping the raw and processed datasets separate helps preserve the original source data while allowing the cleaned dataset to be used for analysis.

## 5. Data Cleaning and Preprocessing

The raw data was inspected and cleaned before analysis.

The preprocessing included:

-Loading the source CSV dataset using the pipe (|) separator
-Inspecting the dataset structure and data types
-Standardizing page and post identifiers
-Handling missing values without inventing information
-Standardizing date values
-Removing unnecessary whitespace from text fields
-Cleaning and standardizing textual content
-Calculating text length in characters
-Profiling topic information
-Checking for duplicate records
-Validating the cleaned dataset
-Exporting the final dataset as a pipe-separated CSV file

Missing information was not estimated or fabricated. Where information was unavailable in the original source, the corresponding value was preserved as missing or blank.

## 6. Final Dataset

The final cleaned dataset contains:

42 records
8 fields
Pipe (|) separated values
CSV format
Original source URLs retained for provenance

The final processed dataset is located at:

data/processed/db-unza26-csc4792-mbala_municipal_council_cleaned.csv

The raw source dataset is located at:

data/raw/db-unza26-csc4792-mbala_municipal_council_pages.csv

##7. Structured CDF and LGEF Information

In addition to the page-level dataset, the project includes structured information curated from explicit CDF/LGEF projects, assets, empowerment programmes, and bursary-related items identified from the supplied source material.

The structured records preserve information such as:

Project or programme description
Category
Ward
CDF year or period
Amount in Kwacha, where explicitly stated
Progress, where explicitly stated
Beneficiaries or units, where explicitly stated
Sector
Source URL

Values were only included where supported by the source material. No missing financial or project information was estimated.

##8.Repository Structure

The project repository is organized as follows:

mbala-municipal-council/
│
├── data/
│   ├── raw/
│   │   └── db-unza26-csc4792-mbala_municipal_council_pages.csv
│   │
│   └── processed/
│       └── db-unza26-csc4792-mbala_municipal_council_cleaned.csv
│
├── documents/
│   ├── Mbala_Municipal_Council_Data_Description_Paper.pdf
│   ├── Data_Dictionary.pdf
│   ├── Data_Collection_Methodology.pdf
│   └── Data_Cleaning_Preprocessing_Report.pdf
│
├── figures/
│
├── notebooks/
│   └── db-unza26-csc4792-mbala_municipal_council.ipynb
│
└── README.md
Folder Descriptions

data/raw/
Contains the original collected dataset. The raw dataset is preserved so that the data processing workflow can be reproduced.

data/processed/
Contains the final cleaned and validated dataset used for analysis and publication.

documents/
Contains supporting project documentation, including the Data Description Paper, Data Dictionary, Data Collection and Methodology document, and Data Cleaning and Preprocessing Report.

figures/
Contains figures and visualizations generated during the analysis where applicable.

notebooks/
Contains the Jupyter Notebook documenting the data loading, cleaning, preprocessing, validation, and analysis process.

README.md
Provides an overview of the project, dataset, methodology, repository structure, and reproducibility information.

## 9.Jupyter Notebook

The Jupyter Notebook documents the main stages of the dataset creation and preparation process.

The notebook includes:

Dataset loading
Dataset inspection
Data cleaning
Data type standardization
Missing-value handling
Text preprocessing
Topic profiling
Data validation
Dataset export

The notebook is located at:

notebooks/db-unza26-csc4792-mbala_municipal_council.ipynb

Markdown explanations are included throughout the notebook to document the purpose and methodology of the different processing stages.

## 10.File Format

The datasets are provided in CSV format.

The pipe character (|) is used as the column separator.

Example:

url|page_id|post_id|title|date|topics|text_content|text_length_chars

The pipe separator was used to reduce conflicts with commas that may occur naturally within textual content.

## 11 . Dataset

The dataset is published on Kaggle: 
[Mbala Municipal Council Dataset — CDF](https://www.kaggle.com/datasets/lushomomunsaka/mbala-municipal-council-dataset-cdf/data)

## 12. Limitations

The dataset represents a collection of publicly available information from the Mbala Municipal Council website and therefore reflects the information accessible during the data-collection process.

Some council webpages may provide links to downloadable documents without containing the complete contents of those documents in the extracted webpage text.

Detailed budgets, complete development plans, Ward Development Committee records, meeting minutes, and complete beneficiary information should only be added when the underlying documents have been properly extracted and verified.

The dataset should therefore be understood as a curated snapshot of publicly available council information rather than a complete representation of all Mbala Municipal Council records.

## 15. Reproducibility and Provenance

The project maintains a separation between raw and processed data.
The raw dataset is preserved in:

data/raw/

The cleaning and preprocessing workflow is documented in the Jupyter Notebook located in:
notebooks/
The cleaned dataset is stored in:

data/processed/

Source URLs are retained in the dataset to support provenance and allow users to identify the original webpages from which information was obtained.
The project uses Python and Pandas for the main data-processing workflow.


## 10. Project Team

**Project Team #17**

**Council:** Mbala Municipal Council

**Course:** CSC 4792: Data Mining and Warehousing

### Team Members

| Name |              |Student Number |
| Mwimba Njiko          2021377229 
| Isaac Simbeye         2021381668 
| Maliseni Chavula      2022056205 
| Lushomo Munsaka       2022063643 
| Lazarous Ndlovu       2021411699

