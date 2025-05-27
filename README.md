# Exploratory-Data-Analysis-Titanic
Exploratory Data Analysis (EDA) on the Titanic dataset including data cleaning, handling missing values, encoding categorical features, outlier detection, and insightful visualizations to understand patterns and trends. This section focuses on understanding the dataset through statistical summaries and visual techniques to identify trends, patterns, and anomalies.

# Generate Summary Statistics
We used .describe() to compute key statistics for all numeric features:

- Mean, Median, Standard Deviation to understand central tendency and spread.
- Minimum and Maximum values to detect the range and potential outliers.

Example:
Age: Mean ~29.7, Median ~28.
Fare: Median ~14.45, but Max >500 — suggesting skewness.

# Visualize Distributions with Histograms & Boxplots
To explore data visually:
Histograms were used to observe the shape of data distributions.
- Age is slightly right-skewed.
- Fare is highly skewed due to a few very high values.

Boxplots were used to detect outliers.
- Outliers were clearly visible in Fare and Age.

For Parch, only dots appeared instead of a full box — this occurs when most values are concentrated at a few distinct points (e.g., 0, 1).

# Analyze Feature Relationships
Two key visual tools were used:

Pairplot:
- Showed scatterplots for all numeric feature pairs.
- Helped identify trends and clustering based on the Survived label.

Correlation Heatmap:
- Displayed strength of linear relationships between variables.
- Strong negative correlation between Fare and Pclass (as expected: higher classes paid more).
- Weak correlation between Age and Survived.

# Identify Patterns, Trends, or Anomalies
From visuals and statistics, we inferred:

Age: Most passengers were young adults (20–40), some outliers >70.
Fare: Majority paid less than 100; high outliers indicate wealthy passengers.
SibSp & Parch: Most passengers traveled alone or with small families.

Survival Insights:
- Younger passengers and those paying higher fares had better survival rates.
- Small families (1–2 members) showed higher survival probability.
