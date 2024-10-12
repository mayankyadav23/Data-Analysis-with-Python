# 🏥 Medical Data Visualizer

## 🚀 Project Overview

In this project, you will use Python's **Pandas**, **Matplotlib**, and **Seaborn** libraries to visualize and analyze medical examination data. This dataset contains information about various medical measurements, blood test results, and lifestyle habits of patients, which can be used to explore the relationship between these factors and cardiovascular disease.

📌 **Goal**: Visualize the data using categorical plots and heatmaps to discover trends related to cardiovascular disease.

---

## 📚 What You'll Learn

By completing this project, you'll enhance your skills in:

- **Data manipulation** using **Pandas**.
- **Data visualization** using **Matplotlib** and **Seaborn**.
- Cleaning and normalizing medical data.
- Visualizing categorical data and creating heatmaps to uncover correlations.

---

## 📝 Dataset Description

The dataset `medical_examination.csv` includes the following features:

| **Feature**                         | **Variable Type**        | **Description**                                     | **Value Type**            |
|-------------------------------------|--------------------------|-----------------------------------------------------|---------------------------|
| Age                                 | Objective Feature         | Age of the patient (in days)                        | `int`                      |
| Height                              | Objective Feature         | Height of the patient (in cm)                       | `int`                      |
| Weight                              | Objective Feature         | Weight of the patient (in kg)                       | `float`                    |
| Gender                              | Objective Feature         | Gender of the patient                               | Categorical (`1`: Male, `2`: Female) |
| Systolic Blood Pressure (ap_hi)     | Examination Feature       | Systolic blood pressure                             | `int`                      |
| Diastolic Blood Pressure (ap_lo)    | Examination Feature       | Diastolic blood pressure                            | `int`                      |
| Cholesterol Level (cholesterol)      | Examination Feature       | Cholesterol level                                   | Categorical (`1`: normal, `2`: above normal, `3`: well above normal) |
| Glucose Level (gluc)                | Examination Feature       | Glucose level                                       | Categorical (`1`: normal, `2`: above normal, `3`: well above normal) |
| Smoking                             | Subjective Feature        | Whether the patient smokes                          | Binary (`0`: No, `1`: Yes) |
| Alcohol Intake                      | Subjective Feature        | Whether the patient consumes alcohol                | Binary (`0`: No, `1`: Yes) |
| Physical Activity                   | Subjective Feature        | Whether the patient engages in physical activity    | Binary (`0`: No, `1`: Yes) |
| Cardiovascular Disease (cardio)      | Target Variable           | Presence or absence of cardiovascular disease       | Binary (`0`: No, `1`: Yes) |

---

## 🛠️ Instructions

You will follow these steps to process and visualize the medical data:

### 1. Data Loading & Processing

- **Load the Data**: Import the dataset `medical_examination.csv` using **Pandas** and store it in a variable called `df`.
  
- **Create an Overweight Column**: Calculate the BMI (Body Mass Index) from the `height` and `weight` columns. Create a new column `overweight` where `1` indicates a BMI over 25 (overweight) and `0` otherwise.

- **Normalize Data**: For the `cholesterol` and `gluc` columns, normalize the data so that `0` is always good and `1` is bad. Set the value to `0` if it's `1`, and set it to `1` if the value is greater than `1`.

### 2. Categorical Plot

- In the `draw_cat_plot` function, create a **categorical plot** using the following steps:
    - Melt the DataFrame into a long format using **Pandas' `melt()` function**, with `cholesterol`, `gluc`, `smoke`, `alco`, `active`, and `overweight` as value variables.
    - Group and format the data to show counts of each feature split by the `cardio` column.
    - Plot the data using **Seaborn's `catplot()`** to visualize the counts of the categorical features.
    - Store the figure in the variable `fig`.

### 3. Heatmap

- In the `draw_heat_map` function, create a **heatmap** to show correlations between the features:
    - Clean the data by filtering out rows where:
        - Diastolic pressure (`ap_lo`) is greater than systolic pressure (`ap_hi`).
        - Heights and weights are outside the 2.5th and 97.5th percentiles.
    - Calculate the **correlation matrix** using `df.corr()`.
    - Generate a mask for the upper triangle to make the heatmap easier to read.
    - Plot the heatmap using **Seaborn's `heatmap()`**, and store the figure in `fig`.

---

## 🔍 Data Visualization

Here are the key plots you will create:

### 1. **Categorical Plot**:
Visualizes the relationship between different categorical variables such as cholesterol levels, smoking status, physical activity, and cardiovascular disease.

### 2. **Heatmap**:
Shows the correlation between various medical features, helping you identify any strong relationships between attributes like blood pressure, cholesterol, weight, and cardiovascular disease.

---

## 🔧 Development

- You will write your code in the file `medical_data_visualizer.py`.
- For testing your code, you can use `main.py`, which imports the unit tests from `test_module.py`.

---

## 🧪 Testing

To verify the correctness of your code, unit tests are provided in `test_module.py`. You can run these tests by executing `main.py` to ensure that your functions produce the expected outputs.

---

## 📁 Dataset Source

The dataset used in this project is publicly available through the **UCI Machine Learning Repository**.

- Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Medical+Examination+Records)
