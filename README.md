# Plato Pizza Report

## Project Overview

This is a Power BI project on sales analysis of an imaginary store PLATO’S PIZZA STORES. Things are going well at Plato's, but there's room for improvement. They have been collecting transactional data for the year 2015, but really haven't been able to put it to good use. They look forward to an analysis of the data and a report to help them find opportunities to drive more sales and work more efficiently.

## Data Sources

The dataset used for this project can be found [here](https://drive.google.com/drive/folders/1sT5AReif21UXjW1kICtZPrBb8yshNSOs). This dataset contains 4 tables in CSV format.

- The Orders table contains the date & time that all table orders were placed.
- The Order Details table contains the different pizzas served with each order in the Orders table, and their quantities.
- The Pizzas table contains the size and price for each distinct pizza in the Order Details table, as well as its broader pizza type.
- The Pizza Types table contains details on the pizza types in the Pizzas table, including their name as it appears on the menu, the category it falls under, and its list of ingredients.

## Data Cleaning/Preparation

Data was efficiently cleaned and transformed with the Power Query Editor of Power BI. The following data transformation steps were taken:

- Datatype for IDs changed from “WHOLE NUMBER” to “TEXT”.
- I used the first row as header in the PIZZA TYPES table.
- Converted price column from decimal to dollar.
- As I kept digging for more insights, I continued to iterate to suit my needs.

## Exploratory Data Analysis

The company has the following questions and problem to solve with the data:

- What days and times do we tend to be busiest?
- What are our best and worst selling pizzas?
- What's our average order value?
- How much money did we make this year? Can we identify any seasonality in the sales?

## Data Analysis

### Data Modelling

Table relationships were manually detected and below is the schema of the data model:

![image](https://github.com/user-attachments/assets/fd190534-43c3-45ae-9d50-512c6167d683)

### DAX Measures

The DAX measures created for this project are as follows:

Hour Column
Hour
- Revenue Column - `Revenue`
- AVG Order Value - `AVG Order Value`
- AVG Quantity per Order - `AVG Quantity per Order`

## Results and Findings




