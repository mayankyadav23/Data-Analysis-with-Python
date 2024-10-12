# 📊 Page View Time Series Visualizer

## 🚀 Project Overview

In this project, you will visualize time series data using various charts to understand the patterns in visits to the freeCodeCamp forum from May 9, 2016, to December 3, 2019. You will use Python libraries such as **Pandas**, **Matplotlib**, and **Seaborn** to create insightful visualizations that help identify yearly and monthly growth in page views.

---

## 📚 What You'll Learn

By completing this project, you will gain experience in:

- Importing and cleaning data using **Pandas**.
- Creating visualizations using **Matplotlib** and **Seaborn**.
- Analyzing time series data to identify trends and seasonal patterns.

---

## 📝 Dataset Description

The dataset `fcc-forum-pageviews.csv` contains the number of page views each day on the freeCodeCamp.org forum over a span of three years. The columns include:

- **date**: The date of the recorded page views.
- **value**: The number of page views on that date.

---

## 🛠️ Instructions

You will follow these steps to visualize the page view data:

### 1. Data Loading & Cleaning

- **Load the Data**: Use **Pandas** to import the dataset from `fcc-forum-pageviews.csv`, setting the date column as the index.
  
- **Clean the Data**: Filter out days when the page views are in the top 2.5% and bottom 2.5% of the dataset to focus on the typical data range.

### 2. Create Line Plot

- In the `draw_line_plot` function, use **Matplotlib** to create a line chart:
    - Title: **"Daily freeCodeCamp Forum Page Views 5/2016-12/2019"**.
    - X-axis label: **"Date"**.
    - Y-axis label: **"Page Views"**.

### 3. Create Bar Plot

- In the `draw_bar_plot` function, create a bar chart to show the average daily page views for each month grouped by year:
    - X-axis label: **"Years"**.
    - Y-axis label: **"Average Page Views"**.
    - Legend: Should show month labels and have the title **"Months"**.

### 4. Create Box Plot

- In the `draw_box_plot` function, use **Seaborn** to create two adjacent box plots:
    - The first box plot should show the year-wise distribution with the title **"Year-wise Box Plot (Trend)"**.
    - The second box plot should show the month-wise distribution with the title **"Month-wise Box Plot (Seasonality)"**.
    - Ensure that the x-axis starts at January for month labels.

---

## 🔍 Data Visualization

### 1. **Line Plot**:
Visualizes daily page views, showing trends over time.

### 2. **Bar Plot**:
Displays average daily page views for each month, allowing comparisons across years.

### 3. **Box Plot**:
Illustrates the distribution of page views for each year and month, highlighting trends and seasonality.

---

## 🔧 Development

- You will write your code in the file `time_series_visualizer.py`.
- For development and testing, you can use `main.py`, which imports unit tests from `test_module.py`.

---

## 🧪 Testing

Unit tests for this project are provided in `test_module.py`. You can run these tests by executing `main.py` to verify that your functions are producing the expected visual outputs.

---

## 📁 Dataset Source

The dataset is available through the freeCodeCamp platform:

- Source: [freeCodeCamp](https://www.freecodecamp.org/)

