# Week 1 Homework: Introduction to Machine Learning

## Assignment Overview
- **Week**: 1
- **Topic**: Introduction to Machine Learning & Python Refresher
- **Due Date**: [Course specific date]
- **Status**: [✅] Completed

## Objectives
- [✅] Set up Python environment for ML
- [✅] Review pandas and numpy basics
- [✅] Understand basic ML concepts
- [✅] Complete first ML prediction

## Files
- `homework_01.ipynb` - Main homework notebook
- `data/` - Car price dataset
- `requirements.txt` - Python dependencies

## Questions & Solutions

### Question 1: What's the version of pandas?
```python
import pandas as pd
print(pd.__version__)
```

**Solution:** 1.5.0 (example answer)

### Question 2: Dataset exploration
How many records are in the dataset?

**Solution:** 
```python
df = pd.read_csv('data/car_prices.csv')
print(f"Number of records: {len(df)}")
```
Number of records: 11,914

### Question 3: Missing values
Which columns have missing values?

**Solution:**
```python
print(df.isnull().sum())
```

### Question 4: Most frequent value
What's the most frequent make of the car?

**Solution:**
```python
print(df['make'].value_counts().head(1))
```

### Question 5: Correlation
What's the correlation between engine_hp and price?

**Solution:**
```python
correlation = df['engine_hp'].corr(df['msrp'])
print(f"Correlation: {correlation:.3f}")
```

## Code Examples

```python
# Data loading and basic exploration
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

# Load data
df = pd.read_csv('data/car_prices.csv')

# Basic info
print(df.head())
print(df.info())
print(df.describe())

# Data visualization
plt.figure(figsize=(10, 6))
plt.scatter(df['engine_hp'], df['msrp'], alpha=0.5)
plt.xlabel('Engine HP')
plt.ylabel('Price (MSRP)')
plt.title('Car Price vs Engine Horsepower')
plt.show()
```

## Key Learnings
- Pandas is essential for data manipulation in ML
- Data exploration is crucial before building models
- Correlation helps understand relationships between variables
- Missing values need to be handled appropriately

## Reflection
This week provided a great refresher on Python basics and introduced fundamental ML concepts. The car price dataset was interesting to explore, and I learned about the importance of data quality in ML projects.

## Next Steps
- [ ] Review linear algebra concepts for next week
- [ ] Practice more pandas operations
- [ ] Read about regression algorithms