# Overview

## This project seeks to answer the following questions:

    A. What does the distribution of salary look like overall? 

    B. In what locations or regions are most companies hiring? 

    C. How are salaries trending? 

    D. What are the most optimal skills to learn for Data Analysts? (High-demand vs. high-paying) 

    E. For job seekers: How likely it is to get a job without a degree, and how reasonable it is to expect WFH & health benefits?

The data analyzed in this project was collected by Luke Barousse, a submariner-turned-data-analyst who has supported numerous individuals seeking to enter the data analytics field, including myself. The dataset provides comprehensive information on job titles, salaries, locations, essential skills, and other factors of interest to both job seekers and individuals exploring trends within the industry.

## Tools

1. Python: The foundation of this project. I also used the following libraries:
    - Pandas: for data analysis; 
    - Matplotlib & Seaborn: for data visualization; 

2. Jupyter Notebooks: I used this to run Python scripts; 

3. Visual Studio Code: for Python script execution; and

4. Git & GitHub: for version control and sharing.

## Data Cleaning and Preparation

### Step One - Importing libraries and loading data

```python
import ast
import numpy as np
import pandas as pd
from datasets import load_dataset
import matplotlib.pyplot as plt  
import seaborn as sns
from adjustText import adjust_text

# This is the "raw" dataset
df = pd.read_csv('/Users/andreawei/Documents/Learnings/Python Project/Datasets/gsearch_jobs.csv')
```
### Step Two - Preliminary Data Cleaning

Before diving into my analysis, I did the following to clean up or format the data:
1. Remove the rows where salary information wasn't available; 
2. Rename certain columns so the headings are more descriptive of the values; 
3. Reset index; 
4. Explode the 'job_skills' column (to pave the way for Objective E); and
5. Extract the "state" from the 'location' column (e.g., "California") and re-format the strings.

To find the details of these steps, please view my notebook: [Data_Cleaning_(Preliminary)](Data_Cleaning_(Preliminary).ipynb).

## In-Depth Analysis

The dataset covers positions posted between November 2022 and April 2025.

### Objective A - What does the distribution of salary look like overall? 

As shown in the histogram below, most data analyst jobs pay around $100,000 annually.

View my notebook for details: [Objective_A_(Salary Distribution)](Objective_A_(Salary Distribution).ipynb)

![alt text](image.png)

### Objective B - In what locations or regions are most companies hiring? 

View my notebook for details: [Objective_B_(Job Postings by Region)](Objective_B_(Job Postings by Region).ipynb)




