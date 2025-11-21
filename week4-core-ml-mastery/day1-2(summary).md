# Dataset Basics
Total rows: 1025 → after removing duplicates: 302
Total columns: 14
No missing values


## 2. Duplicates

Many rows were duplicates — removed them to avoid bias in the model.
Always check for duplicates in medical data: can affect predictions & fairness

## 3. Feature Types

Numeric: age, trestbps, chol, thalach, oldpeak
Categorical: sex, cp, fbs, restecg, exang, slope, ca, thal, target
Count unique values to confirm type

## 4. Key Statistics (Numeric Features)
Feature	Mean (No Disease)	Mean (Disease)	Note
Age	56.57	52.41	Non-disease group older (dataset quirk)
trestbps	134	129	Small difference
Chol	251	241	Slightly higher in non-disease
Thalach	139	158	Max heart rate higher in disease group
Oldpeak	1.6	0.57	ST depression higher in non-disease group

💡 Lesson: Dataset has quirks; patterns are not always intuitive. Understanding statistics helps interpret ML results later.

## 5. Histograms

Visual check: numeric features vary by disease/no disease
Look for overlaps and gaps between groups
Don’t stress if it seems weird — practice makes it clearer

6. Core Takeaways

Always explore duplicates & missing values first.
Know your numeric vs categorical columns.
Summarize features with mean, median, std.

Visuals (histograms) + numbers = better intuition.

Datasets can be messy or counterintuitive — that’s normal.

This step builds the foundation for modeling, feature engineering, and bias analysis.
