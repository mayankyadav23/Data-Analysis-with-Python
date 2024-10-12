# 📊 Demographic Data Analyzer

## 🚀 Project Overview

This project is designed to analyze demographic data extracted from the **1994 Census** dataset using **Pandas**. By analyzing this data, we can uncover various demographic trends related to race, education, income, and work hours. If you're new to working with data and Python's Pandas library, this project is an excellent introduction to data manipulation and analysis.

📌 **Goal**: Use Pandas to answer specific questions about the dataset, such as average age, education levels, income brackets, and more.

---

## 📚 What You'll Learn

In this project, you'll enhance your skills in:

- Reading and analyzing large datasets using **Pandas**.
- Calculating key statistics like average age, income brackets, and employment trends.
- Deriving insights from data by answering questions about race, education, salary, and occupation.
- Handling and transforming real-world data in a structured format.

---

## 🛠️ How It Works

The dataset provided contains various demographic and work-related features. Your task is to use **Pandas** to answer the following questions:

1. **Racial Representation**: How many people of each race are represented in the dataset? (Use the `race` column)
2. **Average Age of Men**: Calculate the average age of all male individuals.
3. **Education Statistics**:
   - What percentage of people have a **Bachelor's degree**?
   - What percentage of people with **advanced education** (Bachelor's, Master's, or Doctorate) earn more than 50K?
   - What percentage of people **without advanced education** earn more than 50K?
4. **Working Hours**:
   - What is the minimum number of hours someone works per week?
   - What percentage of people working the **minimum hours per week** earn more than 50K?
5. **Country-Based Insights**:
   - Which country has the **highest percentage** of people earning more than 50K? What is that percentage?
6. **Occupation in India**: Identify the most popular occupation for people in **India** who earn more than 50K.

You will write a function to answer each question, using the dataset provided in the project files.

### 💡 Example Questions

- What percentage of the people in the dataset who work the minimum number of hours per week have a salary greater than 50K?
- What is the most popular occupation for those earning >50K in India?

### 📊 Dataset Structure

The dataset includes the following columns:

|    |   age | workclass        |   fnlwgt | education   |   education-num | marital-status     | occupation        | relationship   | race   | sex    |   capital-gain |   capital-loss |   hours-per-week | native-country   | salary   |
|---:|------:|:-----------------|---------:|:------------|----------------:|:-------------------|:------------------|:---------------|:-------|:-------|---------------:|---------------:|-----------------:|:-----------------|:---------|
|  0 |    39 | State-gov        |    77516 | Bachelors   |              13 | Never-married      | Adm-clerical      | Not-in-family  | White  | Male   |           2174 |              0 |               40 | United-States    | <=50K    |

---

## 🔍 Data Analysis Steps

1. **Load the data** from the provided CSV file.
2. **Perform calculations** using Pandas for each of the required metrics.
3. **Update the starter code** in `demographic_data_analyzer.py`, ensuring all calculations are correct.
4. **Round all decimal results** to the nearest tenth.

---

## 🧪 Testing

- The project includes unit tests in the file `test_module.py`.
- Run these tests to ensure your code works correctly by importing them into `main.py`.
- Make sure your calculations match the expected outputs!

---

## 📁 Dataset Source

This dataset is sourced from the **UCI Machine Learning Repository**. It was extracted from the 1994 Census database.

- Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/adult)

