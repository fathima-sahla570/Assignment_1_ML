Approach to the Assignment
Step 1: Load the Dataset & Perform Basic EDA 
Load the dataset using pandas

Display the first few rows to understand the structure.

Check for missing values and duplicates

Get summary statistics using .describe()

Plot histogram & box plot for price per sqft to understand its distribution.

Step 2: Detect & Remove Outliers (Q2 - 4 Marks)
(a) Mean & Standard Deviation Method
Calculate mean and standard deviation of price per sqft.

Identify outliers: Values outside (mean ± 3*std dev)

Remove outliers using trimming or imputation (mean/median).

(b) Percentile Method
Compute 5th percentile (Q5) and 95th percentile (Q95).

Remove values below Q5 and above Q95.

(c) IQR Method (Interquartile Range Method)
Compute Q1 (25th percentile) and Q3 (75th percentile).

Compute IQR = Q3 - Q1.

Define outliers: Values below (Q1 - 1.5IQR) or above (Q3 + 1.5IQR).

Remove or cap these outliers.

(d) Z-Score Method
Compute the Z-score for each value.

Remove data points with |Z-score| > 3.

Step 3: Box Plot to Compare Methods 
Create box plots for the original and cleaned datasets.

Identify which method best removes outliers while preserving data distribution.

Step 4: Histplot & Transformations
Draw a histplot to check normality of price per sqft.

Calculate skewness and kurtosis before transformation.

Apply transformations (Log, Square Root, Box-Cox) if necessary.

Recalculate skewness and kurtosis after transformation.

Step 5: Correlation & Heatmap 
Compute correlation matrix for numerical variables.

Visualize using a seaborn heatmap.

Step 6: Scatter Plot
Create scatter plots between key numerical variables.

Identify relationships between variables












