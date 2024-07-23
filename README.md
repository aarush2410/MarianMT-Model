## Finetuning MarianMT Model for German-English Translation
This repository contains all necessary steps to fine-tune the MarianMT model for German-English translation using datasets from OPUS100, WMT 14-20, and Europarl. Below is an overview of the contents:

### Repository Structure
research/

datasets_overview.md: Detailed research on the datasets used, including OPUS100, WMT 14-20, and Europarl. This file contains information on the key data sources, approximate size, and test set domains.
data_preparation/

prepare_datasets.py: Script for downloading, cleaning, and preparing the datasets for training.
README.md: Instructions on how to use the data preparation scripts.
exploratory_data_analysis/

eda.ipynb: Jupyter Notebook containing exploratory data analysis (EDA) of the datasets.
README.md: Summary of insights obtained from the EDA.
fine_tuning/

fine_tune_marianmt.py: Script for fine-tuning the MarianMT model.
README.md: Instructions on how to use the fine-tuning script and details about the training process and results.

## Datasets Overview
The datasets_overview.md file provides comprehensive research on the following datasets:

* OPUS100

Key Data Sources: A collection of freely available parallel corpora for machine translation.
Approximate Size: Approximately 100 million sentence pairs.
Test Set Domains: Various domains including medical, legal, and general news.
* WMT 14-20

Key Data Sources: Data from the Workshop on Machine Translation (WMT) shared tasks from 2014 to 2020.
Approximate Size: Varies by year, generally ranging from 4 to 20 million sentence pairs per year.
Test Set Domains: News articles, with specific test sets each year.
* Europarl

Key Data Sources: The proceedings of the European Parliament.
Approximate Size: Approximately 2 million sentence pairs.
Test Set Domains: Political and legislative documents.
### Data Preparation
The prepare_datasets.py script handles the following tasks:

Download: Automatically downloads the datasets from specified sources.
Cleaning: Cleans the datasets to remove unwanted characters, language mismatches, etc.
Formatting: Formats the datasets to be compatible with the MarianMT model.
Instructions on how to use this script are provided in the data_preparation/README.md.

## Exploratory Data Analysis
The eda.ipynb notebook performs exploratory data analysis on the datasets, including:

Distribution of sentence lengths.
Common words and phrases.
Language-specific characteristics.
The insights from the EDA are summarized in the exploratory_data_analysis/README.md.

## Fine-Tuning
The fine_tune_marianmt.py script fine-tunes the MarianMT model using the prepared datasets. This script includes:

Model initialization.
Training loop.
Evaluation metrics.
Detailed instructions and results from the fine-tuning process are available in the fine_tuning/README.md.

# Getting Started
To get started with this project:

Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/marianmt-finetuning-de-en.git
cd marianmt-finetuning-de-en
Prepare the datasets:

bash
Copy code
cd data_preparation
python prepare_datasets.py
Perform EDA:

bash
Copy code
cd exploratory_data_analysis
jupyter notebook eda.ipynb
Fine-tune the model:

bash
Copy code
cd fine_tuning
python fine_tune_marianmt.py
Requirements
Python 3.8+
Transformers library
Datasets library
Jupyter Notebook
Additional dependencies listed in requirements.txt
## License
This project is licensed under the MIT License.

## Acknowledgments
Special thanks to the creators and maintainers of the OPUS100, WMT, and Europarl datasets.

Feel free to contribute to this project by submitting issues or pull requests. Happy translating!

For further details, refer to the individual README files within each directory.
