# Israeli Credit Card Expenditures

## Project Overview
This project analyzes Israeli credit card expenditures using time series data. A key part of the analysis involves converting dates from the Gregorian calendar to the Jewish calendar to align with specific analysis goals. This project includes extensive data manipulation, visualization, and potentially model building to explore spending trends and patterns across different periods and categories.

## Files
- `israeli_credit_card_expenditures.ipynb`: The Jupyter Notebook containing the analysis. It includes data preprocessing steps, date transformations, exploratory data analysis (EDA), and modeling efforts.

## Key Features
- **Date Manipulation**: The data originally comes with Gregorian dates. To gain insights from a cultural and religious perspective, these dates were converted to the Jewish calendar scale.
- **Time Series Analysis**: The notebook applies several techniques for exploring patterns in the time series data, helping to uncover seasonality, trends, and other cyclical behaviors in consumer spending.
- **Expenditure Categories**: Breakdown and analysis of credit card expenditures across various categories to detect which sectors drive the most spending over time.

## Prerequisites
Ensure that you have the following libraries installed to run the notebook:

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- LunarCalendar (or a library to manage Hebrew dates)
- scikit-learn (for modeling)
- hijri-converter (if managing other types of calendars)

Install the dependencies using:
```bash
pip install -r requirements.txt
```

## Analysis Process

### Data Preprocessing:
- Handling missing values and any data inconsistencies.
- The key manipulation involves converting Gregorian calendar dates to the Jewish calendar for better alignment with holiday periods and religious observances that might affect spending patterns.
- This is particularly important to identify seasonal effects that coincide with major Jewish holidays.

### Exploratory Data Analysis (EDA):
- Visualization of spending patterns using matplotlib and seaborn to uncover major trends.
- Breakdown of expenditures by category, time period, and other relevant factors.
- Identification of potential outliers or unusual spending spikes that may correspond to specific holidays or events.

### Date Transformation:
- Special focus is given to converting the Gregorian calendar to the Jewish calendar. This step involves adjusting for different start points of months and years, ensuring that the analysis reflects the Hebrew year cycle.
- Techniques like `pd.to_datetime` followed by calendar transformations (e.g., using libraries like `LunarCalendar` or manual adjustments) are used to map Gregorian dates accurately to the Hebrew calendar.

### Modeling (If Applicable):
- Depending on the dataset, predictive models or time series forecasting may be employed.
- This could include forecasting future expenditures or identifying which factors are most predictive of certain spending behaviors.

## Insights

- **Holiday Spending**: The impact of Jewish holidays on spending patterns is a significant focus. For example, do expenditures increase during Passover or Sukkot? How does the shift in holiday dates each year (due to the lunar nature of the Jewish calendar) affect overall trends?
- **Spending Categories**: Which categories see the most spending, and how do they fluctuate over time? Are there noticeable shifts before and after specific holidays?
- **Time Series Trends**: Uncover seasonality or cyclical patterns in credit card expenditures using decomposition or other time series methods.

## Results and Conclusions

This section can summarize the results of the analysis, including:
- **Key Trends**: Highlight significant findings such as increases in certain expenditure categories during Jewish holidays.
- **Seasonality**: Discuss whether certain times of the year (e.g., before or after specific holidays) lead to spikes or dips in spending.
- **Predictive Modeling**: (If applicable) Highlight the accuracy of any forecasts made and the features that had the most predictive power.

## Future Work

Potential areas to expand the project could include:
- **Additional Calendar Systems**: Expanding the analysis to other calendars (e.g., Islamic or other lunar calendars) for comparison.
- **Deeper Modeling**: Applying more advanced machine learning models for deeper forecasting of expenditures.
- **Category-Specific Insights**: Further breakdown of expenditure trends within more granular subcategories.


