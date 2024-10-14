# Project Overview: Property Prices and Criminality in Lincolnshire

## Objective
The goal of this project is to design and implement an end-to-end system architecture that can ingest, store, process, and analyze data, while applying best practices in DataOps and MLOps. This system will handle realistic data and deploy models to extract meaningful insights. Throughout the project, we focus on building a robust pipeline that addresses real-world challenges and demonstrates good development practices for data-driven systems.

## Context
For this project, we worked with two datasets that provide insights into property prices and criminality in Lincolnshire and its districts:

- **Property Prices Dataset**: This dataset contains average monthly house prices (£) for Lincolnshire and its districts, covering the period from June 2020 to June 2022. It was sourced from [data.europa.eu](https://data.europa.eu/data/datasets/house-prices1?locale=es).
  
- **Criminality Dataset**: The crime dataset includes information about various crimes reported in the same districts, from June 2021 to April 2022, sourced from the [UK Police website](https://data.police.uk/data/fetch/561534ac-c79d-46ab-a45f-5b91428a47aa/).

Although the datasets cover slightly different time frames, this doesn’t affect our analysis. We assume that property prices in a given month are influenced by criminal activity from previous months. Specifically, we’ve decided to analyze the impact of crimes that occurred in the six months leading up to a given property price. For example, the property price in July 2020 would be influenced by crime data from January to June 2020.

## Analysis Goals
Our main objective is to explore whether there is a correlation between criminal activity in Lincolnshire's districts and the fluctuations in property prices. If we find such a relationship, we’ll also analyze whether different types of crime affect property prices differently, potentially causing property values to rise or fall more depending on the type of crime.

This project provides hands-on experience in building a scalable data pipeline and deploying it in a real-world context. By working with real data, we aim to gain a deeper understanding of how to manage, process, and analyze data at scale, while exploring a relevant and meaningful topic.

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the libraries necessary for running the backbone.

```bash
pip install -r requirements.txt
```

## Usage

By default, the repository comes with all the available files in the data/temporal directory. They can be found in a zip file. To be able to run the project, you will have to extract in the data/temporal directory. Once they have been extracted, there are two options:

- Running main.py with all the files in dataManagementBackbone/data/landing/temporal
- Keeping some files back and running main.py. Then placing the files you have saved back into the dataManagementBackbone/data/landing/temporal directory and running main.py again. That way you can simulate the process of the data management backbone receiving new data, processing and adding it to the exploitation zone database.


```bash
python main.py
```
