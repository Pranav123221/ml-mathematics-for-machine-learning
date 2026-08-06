.
📈 Measures of Central Tendency
What is Central Tendency?

Measures of Central Tendency describe the center or typical value of a dataset.

The three main measures are:

Mean
Median
Mode
1. Mean

The arithmetic average of all observations.

Formula

[
\text{Mean}=\frac{\sum x}{n}
]

Python
np.mean(data['SW'])
Advantages
Uses all observations
Easy to calculate
Disadvantages
Sensitive to outliers
2. Median

The middle value after sorting the data.

Python
np.median(data['SW'])
Advantages
Not affected by outliers
Suitable for skewed data
3. Mode

The most frequently occurring value.

Python
data['Species'].mode()
Advantages
Useful for categorical variables
Easy to interpret
Comparison
Measure	Outlier Sensitive	Best Used For
Mean	✅ Yes	Normally Distributed Data
Median	❌ No	Skewed Data
Mode	❌ No	Categorical Data
Machine Learning Applications
Missing value imputation
Exploratory Data Analysis
Feature Engineering
Data preprocessing
Key Takeaways
Mean uses every observation.
Median is robust against outliers.
Mode identifies the most frequent value.
Choosing the right measure depends on the data distribution.
