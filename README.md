# 📈💰⚽ Sports product sales analysis

This repository contains a sports product sales data visualization project using Power BI. 

## Table of content
 - [Introduction](https://github.com/herrerovir/Power-BI-sports-product-sales-analysis/blob/main/README.md#Introduction)
 - [Goal](https://github.com/herrerovir/Power-BI-sports-product-sales-analysis/blob/main/README.md#Goal)
 - [Project overview](https://github.com/herrerovir/Power-BI-sports-product-sales-analysis/blob/main/README.md#Project-Overview)
 - [Dependencies](https://github.com/herrerovir/Power-BI-sports-product-sales-analysis/blob/main/README.md#Dependencies)
 - [Technical skills](https://github.com/herrerovir/Power-BI-sports-product-sales-analysis/blob/main/README.md#Technical-skills)
 - [Dataset](https://github.com/herrerovir/Power-BI-sports-product-sales-analysis/blob/main/README.md#Data-set)
 - [Data loading](https://github.com/herrerovir/Power-BI-sports-product-sales-analysis/blob/main/README.md#Data-loading)
 - [Data cleaning](https://github.com/herrerovir/Power-BI-sports-product-sales-analysis/blob/main/README.md#Data-cleaning)
 - [Data modeling](https://github.com/herrerovir/Power-BI-sports-product-sales-analysis/blob/main/README.md#Data-exploration)
 - [Data analysis](https://github.com/herrerovir/Power-BI-sports-product-sales-analysis/blob/main/README.md#Data-visualization)
 - [Data visualization](https://github.com/herrerovir/Power-BI-sports-product-sales-analysis/blob/main/README.md#Insights)

## Introduction

Sales analysis is the process of evaluating sales data to gain insights into sales performance. It involves examining past sales metrics and trends to understand what is working well and what can be improved.

The goal of sales analysis is to help the sales team and management make better-informed decisions to optimize revenue and growth. It provides insights into sales performance so they can identify both opportunities and problems before taking action.

## Goal
The main objective of this project is to perform an analysis of sports product sales in the United States during 2020 and 2021 and to visualize the main KPIs and valuable information obtained from the analysis. 

## Project overview
1. Data loading
2. Data cleaning
3. Data modeling
4. Data analysis
5. Data visualization

## Dependencies
The following tools are required to carry out this project:

* Power BI desktop

## Technical skills
Throughout the implementation of this project, the following skills were applied: 

* Data extraction, transforming and loading
* Data modeling
* Data analysis
* Data visualization

## Dataset
The dataset used for this analysis is an Excel file which can be found uploaded in this repository as Sports-product-sales-analysis-dataset.xlsx.

The dataset consists of:
* 9645 entries
* 13 columns

## Data loading
The data is loaded into Power BI by importing it from the Excel file.

## Data cleaning
Upon loading the data into Power BI, it must be subjected to a pre-processing phase in which the data will be cleaned and transformed to ensure the integrity and reliability of the data.

The cleaning and transformation process is performed using Power Query within Power BI.

The preprocessing workflow includes: renaming columns, changing data types, and removing null and duplicate values.

The cleaned data set is then loaded into Power BI for further analysis and visualization.

## Data modeling
In order to create consistent and high quality structured data to achieve consistent results, the data will be modeled in a star schema. This type of model separates the business process data into facts, which contain the measurable and quantitative data about a business, and dimensions, which are descriptive attributes related to the fact data.

The original table loaded in Power BI is the fact table and stores the quantitative information needed for this analysis. Four dimensional tables are created that contain the descriptive information from the fact table. The dimensional tables created are: product, retailer, region and sales methods. Also a new dynamic date table is created from 01.01.2020 to 31.12.2021. This date dynamic table will also be a dimensional table in the star schema. 

The last step of data modeling is to establish the relationships between the dimensional tables and the fact table.

The following image shows the star model of this project.

![Data-star-model](https://github.com/user-attachments/assets/757e59f8-ac6d-4ca8-8e23-522883c3d758)

## Data analysis
An in-depth analysis of the data was performed to obtain useful sales, product and regional information from this dataset. Multiple measures were created using DAX functions to facilitate the analysis.

## Data visualization
Data visualization plays a central role in data analysis, as it is the stage at which the conclusions drawn from the analysis are effectively communicated. I used Power BI to turn this dataset into an engaging, interactive and information-boosting dashboard.

The dashboard contains two pages: the overview page and the sales analysis page. It is an interactive dashboard where the results for the chosen year or region can be selected and displayed. In addition, data can also be selected and previewed directly from the graphs.

**Overview Page**
At the top of the overview page are the main KPIs of this analysis: total sales, total profit, total units sold and total orders.

The graphs included on the overview page of this dashboard are:

* Ribbon chart
* Matrix chart
* Donut chart
* Clustered bar
* Shape map

**Sales analysis Page**
At the top of the sales analysis page, the same main KPIs are displayed as in the overview.

The charts included on this page are:

* Donut chart
* Clustered bar
* Clustered column
* Decomposition tree

![Overview page](https://github.com/user-attachments/assets/0d1e85d8-5886-42e7-8c3e-45eef7ef6525)

![Sales analysis page](https://github.com/user-attachments/assets/592d739b-0a5e-4adc-b61f-16cb65ea5575)

