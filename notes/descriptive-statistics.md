📊 Descriptive Statistics Notes
📖 What is Descriptive Statistics?

Descriptive Statistics is the branch of statistics used to collect, organize, summarize, and describe data. It helps us understand the characteristics of a dataset without drawing conclusions beyond the available data.

Objectives
Summarize data
Understand data distribution
Detect patterns
Identify outliers
Prepare data for Machine Learning
📌 Types of Data
1. Qualitative (Categorical) Data

Represents categories or labels rather than numerical values.

Examples

Gender
Color
Department
Passenger Class (Titanic)
Visualization Techniques
Frequency Distribution Table

Shows how frequently each category appears.

data['Pclass'].value_counts()
Bar Chart

Used to compare different categories.

sns.countplot(x='Pclass', data=data)
Pie Chart

Shows percentage contribution of each category.

data['Pclass'].value_counts().plot(kind='pie', autopct='%1.1f%%')
2. Quantitative (Numerical) Data

Represents measurable values.

Types
Discrete Data
Continuous Data
Visualization Techniques
Histogram

Displays the distribution of numerical values.

plt.hist(data['Age'])

Useful for understanding:

Distribution
Skewness
Frequency
Distribution Plot

Shows the probability distribution of numerical data.

sns.histplot(data['Age'], kde=True)
Box Plot

Displays

Median
Quartiles
Outliers
Spread
sns.boxplot(x=data['Age'])
Why is Visualization Important?

Visualization helps to:

Understand data quickly
Detect missing values
Find outliers
Understand feature distributions
Prepare data before Machine Learning
Key Takeaways
Descriptive Statistics summarizes data.
Frequency tables describe categorical variables.
Histograms visualize numerical distributions.
Box plots help detect outliers.
Visualization is the first step of Exploratory Data Analysis (EDA).
