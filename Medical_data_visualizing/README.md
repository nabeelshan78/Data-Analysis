# Medical Data Visualizer

This project involves visualizing and analyzing medical examination data using Python libraries such as `matplotlib`, `seaborn`, and `pandas`. The dataset contains information about patients' body measurements, blood test results, and lifestyle choices, and the goal is to explore the relationship between these factors and cardiovascular disease.

## Project Overview

The dataset, `medical_examination.csv`, includes the following columns:

- `age`: Age of the patient (in days)
- `height`: Height of the patient (in cm)
- `weight`: Weight of the patient (in kg)
- `gender`: Gender of the patient (categorical code)
- `ap_hi`: Systolic blood pressure
- `ap_lo`: Diastolic blood pressure
- `cholesterol`: Cholesterol level (1: normal, 2: above normal, 3: well above normal)
- `gluc`: Glucose level (1: normal, 2: above normal, 3: well above normal)
- `smoke`: Smoking status (binary)
- `alco`: Alcohol intake (binary)
- `active`: Physical activity (binary)
- `cardio`: Presence or absence of cardiovascular disease (binary)

## Data
![image](https://github.com/user-attachments/assets/15e56e03-7639-4990-bab4-161aa231bafb)


## Tasks

1. **Add Overweight Column**
   - Calculate the Body Mass Index (BMI) for each patient.
   - Add a column `overweight` to the dataset where:
     - `1` indicates overweight (BMI > 25)
     - `0` indicates not overweight (BMI ≤ 25)

2. **Normalize Data**
   - Normalize the `cholesterol` and `gluc` columns:
     - Convert `1` to `0` (normal)
     - Convert `2` and `3` to `1` (above normal)

3. **Create Visualization**
   - Convert the data into long format.
   - Use seaborn’s `catplot()` to create a chart showing the counts of categorical features (`cholesterol`, `gluc`, `alco`, `active`, `smoke`) for patients with `cardio=1` and `cardio=0` in separate panels.
   - The chart should be similar to `examples/Figure_1.png`.

4. **Clean the Data**
   - Filter out incorrect data based on the criteria provided.
