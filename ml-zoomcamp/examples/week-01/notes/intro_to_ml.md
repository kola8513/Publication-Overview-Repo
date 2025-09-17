# Week 1 Notes: Introduction to Machine Learning

**Date**: September 2024  
**Week**: 1

## 📚 Key Concepts

### Machine Learning Overview
- **Definition**: Field of study that gives computers the ability to learn without being explicitly programmed
- **Importance**: Enables data-driven decision making and automation
- **Applications**: Recommendation systems, fraud detection, image recognition, NLP

### Types of Machine Learning
1. **Supervised Learning**
   - Uses labeled training data
   - Goal: predict outcomes for new data
   - Examples: classification, regression

2. **Unsupervised Learning**
   - Works with unlabeled data
   - Goal: discover hidden patterns
   - Examples: clustering, dimensionality reduction

3. **Reinforcement Learning**
   - Learns through interaction with environment
   - Goal: maximize cumulative reward
   - Examples: game playing, robotics

### ML Project Workflow
1. **Problem Definition** - What are we trying to solve?
2. **Data Collection** - Gather relevant data
3. **Data Exploration** - Understand the data
4. **Data Preparation** - Clean and transform data
5. **Model Selection** - Choose appropriate algorithm
6. **Model Training** - Fit model to data
7. **Model Evaluation** - Assess performance
8. **Model Deployment** - Put model into production

## 🔍 Code Examples

```python
# Basic data exploration workflow
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

# Load and explore data
df = pd.read_csv('data.csv')
print(f"Dataset shape: {df.shape}")
print(f"Missing values: {df.isnull().sum().sum()}")

# Basic statistics
print(df.describe())

# Visualizations
plt.figure(figsize=(12, 4))
plt.subplot(1, 2, 1)
df['target'].hist()
plt.title('Target Distribution')

plt.subplot(1, 2, 2)
df.corr()['target'].plot(kind='bar')
plt.title('Feature Correlations with Target')
plt.tight_layout()
plt.show()
```

```python
# Simple linear regression example
from sklearn.linear_model import LinearRegression
from sklearn.model_selection import train_test_split
from sklearn.metrics import mean_squared_error, r2_score

# Prepare data
X = df[['feature1', 'feature2']]
y = df['target']

# Split data
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)

# Train model
model = LinearRegression()
model.fit(X_train, y_train)

# Make predictions
y_pred = model.predict(X_test)

# Evaluate
mse = mean_squared_error(y_test, y_pred)
r2 = r2_score(y_test, y_pred)
print(f"MSE: {mse:.2f}")
print(f"R² Score: {r2:.2f}")
```

## 📊 Important Libraries

### Core Libraries
- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computing
- **matplotlib**: Basic plotting
- **seaborn**: Statistical visualizations

### ML Libraries
- **scikit-learn**: General-purpose ML library
- **tensorflow**: Deep learning
- **pytorch**: Deep learning (alternative)
- **xgboost**: Gradient boosting

## 🎯 Practice Exercises
- [✅] Set up Python environment with Anaconda
- [✅] Complete car price dataset exploration
- [✅] Practice pandas data manipulation
- [✅] Create basic visualizations

## 🔗 Additional Resources
- [Kaggle Learn - Intro to Machine Learning](https://www.kaggle.com/learn/intro-to-machine-learning)
- [Scikit-learn User Guide](https://scikit-learn.org/stable/user_guide.html)
- [Python Data Science Handbook](https://jakevdp.github.io/PythonDataScienceHandbook/)

## 💭 Personal Insights
- Data quality is crucial for ML success
- Understanding the problem domain is as important as technical skills
- Visualization helps uncover patterns that aren't obvious in raw numbers
- The 80/20 rule applies: 80% data preparation, 20% modeling

## ❓ Questions for Review
1. When should I use supervised vs unsupervised learning?
2. How do I know if my model is overfitting?
3. What's the best way to handle missing data?

## 📝 Next Steps
- [ ] Study linear algebra for ML (vectors, matrices)
- [ ] Learn about regression algorithms in detail
- [ ] Practice feature engineering techniques
- [ ] Review statistics fundamentals