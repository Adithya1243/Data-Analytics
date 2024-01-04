# Analyzing Sales Patterns in UK E-commerce

Author: Adithya Praneeth Parupudi

## Introduction

This project analyzes transnational e-commerce data from a UK-based online retail, focusing on transactions between 01/12/2010 and 09/12/2011. The aim is to understand sales patterns and customer behavior in a business predominantly dealing with wholesalers.

## Architecture

Leveraging Google Big Query and its integration with RStudio via the bigrquery library, this project efficiently processes and analyzes large volumes of transactional e-commerce data.

![Project Architecture](arc.png)

## About the Dataset

The dataset, sourced from "The UCI Machine Learning Repository", contains details like InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, and Country. 

## Research Questions

Key questions addressed include:
- Distribution of unique products sold across different countries.
- Seasonal patterns in sales data.
- Characteristics of top revenue-contributing customers.
- Shopping trends based on specific keywords.

## The Code Part

### Loading Libraries

The project utilizes libraries like bigrquery, dbplyr, lubridate, scales, stringr, purrr, and ggplot2 for data manipulation and visualization.

### Establishing Connection

Connection between RStudio and Google Big Query is established, allowing direct access to the dataset.

### Data Cleaning

Null values in the dataset are identified and handled, particularly in the Description and CustomerID columns.

### Answering Research Questions

The project includes SQL queries and R scripts to analyze and visualize data trends, addressing the research questions.

## Conclusions

The analysis reveals diverse customer bases, seasonal sales trends, and specific product preferences tied to different times of the year.

## Future Scope

Potential expansions include predictive analytics for sales trends, sentiment analysis through reviews, and the impact of marketing campaigns.

## References

- UCI Machine Learning Repository: [Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)
- Google Big Query: [Documentation](https://cloud.google.com/bigquery/docs)
- R Packages: [bigrquery](https://bigrquery.r-dbi.org/), [purrr](https://purrr.tidyverse.org/), [scales](https://scales.r-lib.org/)
