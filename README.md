# Python Tool for Data Normalization, Matching, and Classification

A Python-based data analysis tool that automates the normalization, matching, classification, and visualization of datasets, integrated with SQLite for efficient data management.

---

## Table of Contents

- [Overview](#overview)  
- [Features](#features)
- [Technologies used](#Technologies-Used) 
- [How It Works](#how-it-works)  
- [How to run](#how-to-run)  



---

## Overview

This tool reads train, ideal, and test datasets from CSV files, normalizes the data, matches train functions with ideal functions based on minimum error, classifies test data points, visualizes the results, and stores everything in an SQLite database.

---

## Features

- Load CSV datasets using SQLAlchemy 
- Z-score normalization of datasets  
- Match train functions to ideal functions by minimizing sum of squared errors  
- Classify test data based on closest ideal function  
- Visualization of train vs ideal functions using Matplotlib  
- Store classification results back into the database  
- Unit tests for core functionality  

---

## Technologies Used

   Python 3,
   Pandas,
   NumPy Bokeh (for visualization),
   SQLAlchemy (for SQLite),
   unittest (for testing)

---

## How It Works

1. **Load Data**  
   Import CSV files into tables.

2. **Normalize Data**  
   Apply Z-score normalization for standardized comparison.

3. **Match Functions**  
   Identify the ideal function best matching each train function by minimizing squared error.

4. **Plot Data**  
   Generate comparison plots of train and ideal functions.

5. **Classify Test Data**  
   Assign test points to the closest ideal function based on minimal Y-value difference.

6. **Save Results**  
   Persist classification results

---


## How to Run
1. Install required packages:
   pip3 install pandas numpy bokeh sqlalchemy

2. Run Main.py file
   python3 Main.py

3. Run Tests
   python3 -m unittest unit.py

---




