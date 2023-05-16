# Mental Illness Identification Using Transformer Language Models

Mental Illness Identification Using Transformer Language Models

## Table of Contents

- [Description](#description)
- [Components](#components)
- [Usage](#usage)
- [Data](#data)
- [Models](#models)
- [Contributing](#contributing)
- [License](#license)

## Description

The goal of this project is to explore the potential of social media as a tool for detecting mental illness and facilitating early intervention and treatment. Our approach involves scrapping data from 9 mental health related subreddits and training language models on this data to help identify the mental illness.

## Components

The codebase for this project is divided into the following components:

1. **Jupyter Notebooks**: The Jupyter notebooks used for different purposes in the project are as follows:

- **DataExtractor.ipynb**: This notebook contains the code used to pull the raw Reddit data for the chosen subreddits using the PushShift API and save the extracted data to CSV files.
- **Data_Preprocessing.ipynb**: This notebook includes the code used for preprocessing the extracted dataset and also provides a visual representation of the data distribution.
- **All_models.ipynb**: The primary notebook used for designing and training all six models. It includes tokenizer definitions, data import and formatting, model definitions, training, evaluation, top-k accuracy and ensembling.
- **Hyperparameter tuning.ipynb**: This notebook was used for performing hyperparameter tuning for the models using grid search.
- **Error analysis.ipynb**: This notebook was used to generate resources for error analysis, such as confusion matrices and misclassification counts and manual analysis plots.

2. **Data**: The data folder contains various CSV files, including raw data, preprocessed data, and the final cleaned dataset (`final_dataset_cleaned.csv`), which was used for training and evaluation of the models. The folder also includes CSV files generated for error analysis. These files capture text, true labels, and predicted labels for specific combinations of classes along with manual annotation (`Manual Annotation.xlsx`)

3. **Models**: The models folder (excluded from the final submission due to its size) contains checkpointed models in `.pt` files for BERT, RoBERTa, XLNet, and their corresponding large versions.


