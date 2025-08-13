** Titanic Exploratory Data Analysis (EDA)

==> Project Overview
This project performs ""Exploratory Data Analysis"" on the Titanic dataset using ""Google Colab"" (web browser).  
It explores survival patterns and relationships between variables using Python libraries: ""Pandas"", ""Matplotlib"", and ""Seaborn"".

==> Objectives
- Apply ".describe()", '.info()', and '.value_counts()' to understand data structure and distributions.  
- Visualize patterns using 'sns.pairplot()' and 'sns.heatmap()'.  
- Create histograms, boxplots, and scatterplots to uncover relationships.  
- Identify key trends, correlations, and data anomalies.

1.describe():
=>Statistical summary of numerical features (mean,median,average etc...)
2.info()
=>Data types, counts, non-null values
3.value_counts():
=>Value counts for categorical feature

4. sns.pairplot()
=>What it does: Creates a grid of scatterplots for all numeric column combinations, with histograms along the diagonal.
=>For your file: Showed relationships between numeric features like Age, Fare, Pclass, SibSp, and Parch.
=>Example insight: Higher Fare values were often linked to lower Pclass (1st class passengers).

5. sns.heatmap() (correlation heatmap)
=>What it does: Displays a matrix showing correlation values between numeric columns, using colors to indicate strength/direction.
=>For your file: Revealed a positive correlation between SibSp and Parch (0.31) and a negative correlation between Pclass and Fare (-0.58).
=>Example insight: More family members on board → higher chance Parch and SibSp both increase.

6. Histograms
=>What it does: Shows the distribution (frequency) of values in a single column.
=>For your file:
 Age: Most passengers were between 20–40 years old.
Fare: Most fares were below $50, with a few extreme outliers.

7. Boxplots
=>What it does: Visualizes data spread, median, and outliers.
=>For your file:Fare had many high-value outliers.
                Age showed a fairly even spread but with some missing values (not plotted in box).

8. Scatterplots
=>What it does: Plots points for two numeric variables to see relationships or clusters.
=>For your file: Fare vs Pclass: Higher fares were clearly in Pclass 1.
                 Age vs Fare: Older passengers sometimes paid higher fares, but not always.
