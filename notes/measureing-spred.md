📉 Measures of Spread
What is Spread?

Measures of Spread describe how widely the data points are distributed around the center.

1. Range

Difference between the maximum and minimum values.

Formula

[
Range = Maximum - Minimum
]

Python
np.max(data['PL']) - np.min(data['PL'])
2. Percentiles

A percentile indicates the value below which a given percentage of observations fall.

Python
np.percentile(data['PL'], 25)
np.percentile(data['PL'], 90)
3. Quartiles

Quartiles divide the data into four equal parts.

Q1 → 25%
Q2 → Median
Q3 → 75%
4. Interquartile Range (IQR)

Measures the spread of the middle 50% of the data.

Formula

[
IQR = Q3 - Q1
]

Python
Q1 = np.percentile(data['PL'], 25)
Q3 = np.percentile(data['PL'], 75)
IQR = Q3 - Q1
5. Variance

Measures the average squared deviation from the mean.

Python
np.var(data['PL'])

Higher variance indicates greater spread.

6. Standard Deviation

Square root of variance.

Python
np.std(data['PL'])

Standard deviation is expressed in the same units as the original data.

Outlier Detection

Using the IQR method:

[
Lower\ Bound = Q1 - 1.5(IQR)
]

[
Upper\ Bound = Q3 + 1.5(IQR)
]

Values outside these bounds are considered outliers.

Machine Learning Applications

Measures of Spread are used for:

Outlier Detection
Feature Scaling
Standardization
Data Cleaning
Exploratory Data Analysis
Summary
Range measures the total spread of the data.
Percentiles indicate relative positions within the dataset.
Quartiles divide the data into four equal parts.
Interquartile Range (IQR) measures the spread of the middle 50% of the data and helps detect outliers.
Variance measures the average squared deviation from the mean.
Standard Deviation measures the average distance from the mean in the original units of the data.

These measures are essential for understanding data variability before applying Machine Learning algorithms.
