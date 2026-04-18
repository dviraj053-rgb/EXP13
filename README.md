# EXP13
Aim:
To process a dataset and handle missing values effectively.
Theory:
In data science, missing values are typically represented as NaN (Not a Number). Managing these missing entries is an essential preprocessing step, as they can distort analysis, lower model performance, and even cause algorithms to fail.
One common approach is to replace missing values with statistical estimates such as the mean (average), median (middle value), or a constant like 0. Another important step is correcting inconsistencies in the data—for example, standardizing date formats or ensuring consistent text capitalization (e.g., converting "cse" to "CSE") to maintain data integrity.
Key functions used in handling missing data include:


isna(): Returns a Boolean DataFrame indicating missing values.


notna(): Opposite of isna(), identifying non-missing values.


sum(): When combined with isna(), counts missing values in each column.


sum(axis=1): Counts missing values across each row.


dropna(): Removes rows or columns containing missing values.


fillna(value): Replaces NaN values with a specified value, such as a constant or calculated statistic.


replace(old, new): Substitutes specific placeholders (e.g., "-") with NaN values.


to_numeric(): Converts data to numeric format, assigning NaN to invalid entries when errors='coerce' is used.


mean(): Computes the average, often used for filling missing numerical data.


median(): Finds the middle value, useful when data contains outliers.


str.upper(): Converts text data to uppercase for consistency.


pd.to_datetime(): Standardizes different date formats into a uniform datetime format.


Conclusion:
This program highlights that data wrangling is a step-by-step process. By replacing inconsistent placeholders with NaN, filling missing values using statistical methods, and standardizing text and date formats, raw data can be transformed into a clean and structured form suitable for accurate analysis.
