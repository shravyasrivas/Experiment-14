

---

# Experiment 14: Data Binning and Data Formatting using Python

---

### Aim: Data Binning and Data Formatting using Python

---

### Theory

Data binning (also known as bucketing) is a data preprocessing technique used to reduce the effects of minor observation errors and transform numerical data into categorical segments. This is done by grouping a set of continuous values into a smaller number of "bins". For example, numerical prices can be binned into "Low," "Medium," and "High" categories.

Data formatting involves standardizing the structure of the dataset to ensure consistency across all entries. This includes converting data types (e.g., from integers to floats), modifying string casing (e.g., converting product names to uppercase), and rounding numerical values to a specific precision. These steps are essential for improving the accuracy of data analysis and preparing datasets for machine learning models.


---

### Command Descriptions

The following Pandas commands were used to execute binning, formatting, and structural operations:

| Command | One-Line Description |
| :--- | :--- |
| `pd.DataFrame(data)` | Initializes a tabular DataFrame structure from a Python dictionary. |
| `pd.cut()` | Segments and sorts numerical data into specific discrete bins with defined labels. |
| `df.dtypes` | Returns the data type of each column to verify if formatting is required. |
| `.astype(float)` | Casts a column's data type from its current format to a floating-point number. |
| `.str.upper()` | Converts all string characters in a selected column to uppercase for uniformity. |
| `.round(2)` | Limits the precision of numerical values by rounding them to two decimal places. |
| `.sort_values(by='X')` | Rearranges the dataset rows based on the values of a specified column in ascending order. |
| `ascending=False` | An argument used within the sort function to rearrange data in descending order. |
| `.unique()` | Extracts and displays a list of all distinct categories or values present in a column. |

---

### Functions and Logic Used

#### Categorization Logic
* **Range Definition:** Specific numerical boundaries (bins) were set to divide the "Price," "Units_Sold," and "Order_Value" columns into distinct groups.
* **Labeling:** Descriptive tags like "Low," "Medium," and "High" were applied to the numerical ranges to make the data more readable.

#### Formatting & Consistency
* **Type Conversion:** Values in the "Units_Sold" and "Distance_km" columns were converted to floats to allow for fractional representation.
* **Text Standardization:** Product names and delivery categories were standardized to uppercase to prevent case-sensitive errors during future analysis.
* **Data Organization:** The `sort_values` function was used to visualize the dataset from the lowest to highest value (and vice-versa) based on specific metrics like "Price" or "Order_Value".

---

### Conclusion

Through this experiment, I successfully implemented data binning and formatting techniques using Python. I learned how to transform complex numerical data into meaningful categories using the `pd.cut()` function, which simplifies the interpretation of data trends. Additionally, I practiced standardizing data types and string formats, which are vital steps in the data wrangling process to ensure dataset consistency and reliability.

---

