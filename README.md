# HOW TO RUN THIS PROJECT:
You can run this project on Google Colab, or run in your system.

In this notebook file you can run notebook_import_variables() to load all env variables, dataframes, scalers and another data, in any cell, to avoid re-run entire notebook to obtain data.

[Jupyter_notebook_file](notebooks\BirminghamCC_PurchaseCardTransactions.ipynb)

## System-requirements
 - Miniconda terminal

In miniconda terminal you can install, activate or close environment to run this project.

**Open a miniconda terminal in project root folder to do the following steps:**

## Environment install (dont need to do, if you already downloaded env folder on project root)
    $ conda create --prefix ./env pandas numpy matplotlib scikit-learn seaborn tensorflow pytorch jupyter statsmodels xlrd pmdarima dill

## Activate this environment to run this project:
    $ conda activate .\env

### After activate conda env, you can install and do another conda commands:
    $ conda install statsmodels

## Deactivate environment to close project:
    $ conda deactivate

# DS-BirminghamCardTransactions
Data Science work to get data insights from Birmingham City Council - Purchase Card Transactions

In this dataset you have a collection of purchase card transactions for the Birmingham City Council. https://data.birmingham.gov.uk/organization/birmingham-city-council. This is a historical dataset, you’re able to perform any of the following tasks:

- (Clustering) Discovering profiles (whether the case) or unusual transactions (anomalies detection) ...
- (Forecasting) Try to guess future transactional behaviors. For instance, what would be the next purchase? Expenditures forecasting? ...
- (Creativity) State a problem.

It’s up to you defining the time window in which your analysis will take place.

To do so, we suggest you create a notebook, like Jupyter (if you use python) or a Rmarkdown report (in case you use R) and make it available.
 
Hint to success in your quest: Develop and state clear of the data science process you'll perform over the dataset and highlight important aspects you might consider affordable to discuss over. Use the mindset of a business and curious consultant.

## Considerations : 
The origin of our dataset is a municipal chamber.
The data are distributed in excel spreadsheets, 1 per month from 2014 to 2018, with a few months missing.  

Opening 1 of the files, it can be verified that the records contain transactions per person, which will be identified by the end of the credit card, the transaction is accompanied by the value, date, and identifiers of the supplier and classifiers of the activity and type of product of this supplier.

The first processes can be done:

- Merging of spreadsheets by year (since each year differs slightly in the nomenclature of features)
- Joining dataframes standardizing features
- Clustering by people and clustering by product type

As we have a dataset of corporate cards, perhaps the client's interest is to discover corporate frauds such as purchases of products with overpriced values, and forecasts of expenses per person.

