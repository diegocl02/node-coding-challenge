# Node.js Backend Coding Challenge

Welcome to our Node.js Backend Coding Challenge! In this test, you will create a web server with specific endpoints that perform various data processing tasks on a provided sales dataset.

## Objective

Your task is to build a Node.js web server with the following endpoints:

### 1. Process Data Endpoint (`/process-data`)
- **Function**: Reads a provided CSV file containing sales data and stores this data in memory.
- **Method**: `GET`
- **Response**: A success message indicating data processing is complete.

### 2. Total Sales Endpoint (`/total-sales`)
- **Function**: Calculates total sales either per product or category.
- **Method**: `GET`
- **Query Parameters**:
  - `type`: "product" or "category"
- **Response**: A JSON object with total sales figures.
- **Error Handling**: If data is not processed, return HTTP status code 503 (Service Unavailable).

### 3. Average Sale Value Endpoint (`/average-sale-value`)
- **Function**: Finds the average sale value per region.
- **Method**: `GET`
- **Response**: A JSON object with the average sale value for each region.
- **Error Handling**: If data is not processed, return HTTP status code 503 (Service Unavailable).

### 4. Highest Sales Volume Day Endpoint (`/highest-sales-volume-day`)
- **Function**: Determines the day with the highest sales volume.
- **Method**: `GET`
- **Response**: A JSON object with the date(s) having the highest sales volume.
- **Error Handling**: If data is not processed, return HTTP status code 503 (Service Unavailable).

## Data Source
The CSV file `sales_data.csv` is provided in the repository. This file contains sample sales data which your endpoints will process and analyze.