# Global Oil & Gas Industry Analysis (1932–2014)

## Project overview
A country-level historical analysis of oil and natural gas production, prices, economic values, exports, net exports and population indicators from 1932 to 2014.

## Repository contents
- `Oil and Gas 1932-2014.csv` – original source dataset (add this file to the repository).
- `Oil_and_Gas_1932_2014_Cleaned.csv` – cleaned dataset generated from the uploaded source.
- `Global_Oil_Gas_Analysis_1932_2014.ipynb` – documented notebook covering cleaning, EDA, statistical analysis, visualizations, feature engineering and recommendations.
- `SRS_Global_Oil_Gas_Analysis.docx` – Software Requirements Specification.
- `README.md` – project documentation.

## Dataset profile
The uploaded source file contains 15,521 rows and 41 columns before cleaning. It covers country-year observations and the period 1932–2014. The analysis is country-level, not oil-field-level.

## Analysis workflow
1. Data inspection and quality profiling
2. Duplicate removal and text standardization
3. Data type and year-range validation
4. Missing-value analysis (without treating unknown values as zero)
5. IQR-based outlier flagging
6. EDA and univariate analysis
7. Bivariate and multivariate analysis
8. Descriptive statistics and correlation
9. Time-series and comparative visualizations
10. Feature engineering, insights and recommendations

## How to run
1. Clone/download this repository.
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
3. Place the original CSV in the same directory as the notebook (or run the notebook using the cleaned CSV).
4. Launch:
   ```bash
   jupyter notebook Global_Oil_Gas_Analysis_1932_2014.ipynb
   ```

## Data handling notes
- Missing values are retained and reported; they are not blindly filled with zero.
- Exact duplicate rows are removed.
- Numeric types and year range are validated.
- Outliers are flagged for investigation, not automatically removed, because extreme country production values may be legitimate.
- All supplied columns are retained because they relate to the stated analysis scope.

## Important scope limitation
This is a country-level historical dataset. It must not be described as Abu Dhabi field-level operational data. Confirm original variable definitions and units from the dataset provider documentation before interpreting or publishing individual measures.

## Expected deliverables
Dataset, SRS document, complete documented Jupyter Notebook and this README.
