# Temperature Analytics Project

This project involves analyzing the monthly average temperature data for India from 1796 to 2013. The dataset is sourced from global temperature records and has been subsetted to focus on India. The objective is to clean the data, visualize historical temperature trends, and predict future temperatures.

## Data Overview

The dataset contains the following columns:
- `dt`: Date of the temperature recording.
- `AverageTemperature`: The average temperature for the month.
- `AverageTemperatureUncertainty`: The uncertainty in the average temperature.
- `Country`: The country of the recording (India).

Key points about the dataset:
- The temperature data spans from 1796 to 2013.
- The temperature values range from around 17°C in the winter months to around 30°C in the summer months.
- The uncertainties in the temperature values generally range from 1-3°C.
- There are some missing values for average temperature and uncertainty for several months.

## Data Cleaning and Transformation

The following steps were taken to clean and transform the data:
1. **Dropping Unnecessary Columns**: Removed any columns not relevant to the analysis.
2. **Handling Missing Values**: Dropped rows with missing values for average temperature and uncertainty.
3. **Removing Duplicates**: Eliminated any duplicate entries.
4. **Standardizing Date Column**: Changed the `dt` column datatype to datetime for better consistency.
5. **Extracting Month and Year**: Extracted the month and year from the `dt` column for further analysis.
6. **Applying Pivot Function**: Used the pivot function to reorganize the data for better understanding.
7. **Forward Fill for NaNs**: Applied forward fill (`ffill`) to handle any remaining NaN values.
8. **Creating New Columns**:
   - `SummerAverage`: The average temperature for the months of April, May, and June.
   - `AnnualAverage`: The average temperature for the entire year.

## Data Visualization

Several visualizations were created to understand the temperature trends and impacts of climate change:
1. **Annual Temperature Trend**: A line graph showing the annual temperature trend in India.
2. **Monthly Average Temperature**: A bar graph showing the monthly average temperature in India.
3. **Impact of Climate Change**: A graph showing the impact of climate change, including a line graph with a 10-year rolling average to understand temperature changes over the last decade.

## Predictive Analysis

To predict future temperatures and fill in missing data, the following steps were performed:
1. **Data Preparation**: Added years that were not present in the original data for predictions.
2. **Modeling**:
   - Used train-test split for model validation.
   - Applied linear regression to predict temperatures for missing data.

## Conclusion

This project provided insights into the historical temperature trends in India and the impact of climate change over the years. The predictive analysis helped estimate future temperatures, contributing to better understanding and preparation for climate change.

## Future Work

Future improvements to this project could include:
- Incorporating more advanced predictive models.
- Analyzing the impact of other climatic factors.
- Expanding the analysis to include other regions and countries.

## Contact

For any queries or contributions, please contact [Viven](mailto:vivenbagde@gmail.com)
