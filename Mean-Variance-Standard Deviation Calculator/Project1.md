# 📊 Mean-Variance-Standard Deviation Calculator

## 🚀 Project Overview

This project is a statistical calculator that uses **Numpy** to compute essential metrics—**mean**, **variance**, **standard deviation**, **min**, **max**, and **sum**—from a 3x3 matrix. It transforms a simple list of numbers into meaningful insights across both rows, columns, and the entire matrix (flattened).

📌 **Goal**: Implement a function that calculates statistics for a matrix from a list of numbers, returning results in a clear, easy-to-read dictionary format.

---

## 📚 What You'll Learn

By working through this project, you’ll gain a hands-on understanding of:

- Transforming lists into Numpy arrays for matrix operations.
- Calculating descriptive statistics like **mean**, **variance**, and more across different axes.
- Returning results in an organized format that’s easy to interpret.
- Handling errors efficiently by validating input data.

---

## 🛠️ How It Works

The main function, `calculate()`, takes a list of **exactly 9 numbers** as input, reshapes it into a 3x3 matrix, and performs calculations to generate the following statistics:

1. **Mean** (average values)
2. **Variance** (spread of data)
3. **Standard Deviation** (average distance from the mean)
4. **Max** (maximum values)
5. **Min** (minimum values)
6. **Sum** (total values)

### 📐 Structure of the Output

The function returns a **dictionary** structured like this:

```python
{
  'mean': [mean_across_rows, mean_across_columns, overall_mean],
  'variance': [variance_across_rows, variance_across_columns, overall_variance],
  'standard deviation': [std_across_rows, std_across_columns, overall_std],
  'max': [max_across_rows, max_across_columns, overall_max],
  'min': [min_across_rows, min_across_columns, overall_min],
  'sum': [sum_across_rows, sum_across_columns, overall_sum]
}
