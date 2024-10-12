# 🌊 Sea Level Predictor

## 🚀 Project Overview

In this project, you will analyze a dataset containing global average sea level changes since 1880. You will create visualizations to understand past trends and predict future sea level changes through the year 2050. This project utilizes Python libraries such as **Pandas** and **Matplotlib** to facilitate data manipulation and visualization.

---

## 📚 What You'll Learn

By completing this project, you will gain experience in:

- Importing and analyzing time series data using **Pandas**.
- Visualizing data with **Matplotlib**.
- Fitting linear regression models to make predictions about future trends.

---

## 📝 Dataset Description

The dataset `epa-sea-level.csv` includes:

- **Year**: The year of the recorded sea level data.
- **CSIRO Adjusted Sea Level**: The global average sea level (in inches) for that year.

---

## 🛠️ Instructions

Follow these steps to analyze and visualize sea level changes:

### 1. Data Loading

- **Load the Data**: Use **Pandas** to import the dataset from `epa-sea-level.csv`.

### 2. Scatter Plot

- Create a scatter plot using **Matplotlib**:
  - X-axis: **Year**.
  - Y-axis: **CSIRO Adjusted Sea Level** (in inches).

### 3. Line of Best Fit

- Use the `linregress` function from **scipy.stats** to calculate the slope and y-intercept for the line of best fit based on the entire dataset.
- Plot this line of best fit over the scatter plot, extending it to the year 2050 to predict the sea level rise.

### 4. Second Line of Best Fit

- Filter the data to include only years from 2000 to the most recent year in the dataset.
- Calculate the slope and y-intercept for this new line of best fit and plot it over the scatter plot.
- Extend this line to the year 2050 to predict the sea level rise based on recent trends.

### 5. Labels and Title

- Set the x-axis label to **"Year"**.
- Set the y-axis label to **"Sea Level (inches)"**.
- Set the plot title to **"Rise in Sea Level"**.

---

## 🔍 Data Visualization

This project will result in a single plot that includes:
- A scatter plot of the sea level data.
- Two lines of best fit predicting sea level changes up to 2050 based on different time frames.

---

## 🔧 Development

- You will write your code in the file `sea_level_predictor.py`.
- For development and testing, you can use `main.py`, which imports unit tests from `test_module.py`.

---

## 🧪 Testing

Unit tests for this project are provided in `test_module.py`. You can run these tests by executing `main.py` to ensure your functions work correctly.

---

## 📁 Dataset Source

The dataset is sourced from the US Environmental Protection Agency, with data from CSIRO and NOAA, covering global average absolute sea level change from 1880 to 2014.
