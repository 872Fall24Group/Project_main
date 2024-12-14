# <California Pollution, Social Vulnerability, and Healthcare Analysis>
# Summary
This repository explores the relationship between air quality and social vulnerability in California. The primary goal is to analyze whether communities exposed to higher pollution levels have less access to healthcare and insurance. Using datasets from 2000 and 2022, the project evaluates trends and shifts in pollution exposure, poverty, and minority population distribution to investigate environmental justice concerns.
# Investigators
- ENVIR 872 Final Project
- **Weilin Wang, Emily Yang, Sujay Dhanagare**
# Keywords
- Air Quality
- Social Vulnerability
- Environmental Justice
- PM2.5 Pollution
- California County

# Database Information
The data used in this analysis includes:
1. **PM2.5 Concentration Data**:
   - **Source**: Environmental Protection Agency (EPA)
   - **Years**: 2000, 2022
   - **Description**: County-level daily mean PM2.5 levels in micrograms per cubic meter (μg/m³), aggregated to yearly averages.
2. **Social Vulnerability Index (SVI) Data**:
   - **Source**: Centers for Disease Control and Prevention (CDC)
   - **Description**: Socioeconomic and demographic indicators, including poverty rates, minority population percentages, and health insurance coverage.
Data was accessed in December 2024 from public portals:
- [EPA Outdoor Air Quality Data](https://www.epa.gov/outdoor-air-quality-data)
- [CDC SVI Data](https://www.atsdr.cdc.gov/place-health/php/svi/svi-data-documentation-download.html)
# Folder Structure, File Formats, and Naming Conventions
## Folder Structure
- **data/**: Contains raw and processed datasets (`.csv`)
- **scripts/**: R scripts for data cleaning, wrangling, analysis, and visualization (`.R`)
- **results/**: Output files, graphs, and summary statistics (`.png`, `.csv`)
## File Formats
- Data: `.csv` files
- Scripts: `.R` files
- Outputs: `.png` (visualizations), `.csv` (processed data)
## Naming Conventions
- Files are named descriptively with prefixes indicating their type:
  - `raw_`: Raw datasets
  - `processed_`: Processed datasets
  - `script_`: R scripts
  
# Metadata

## Data Columns
| Column Name                   | Data Type | Description                                          |
|-------------------------------|-----------|------------------------------------------------------|
| County FIPS Code              | Character | Unique identifier for counties                      |
| County                        | Character | Name of the county                                  |
| Percent_Below_150_Poverty     | Numeric   | % population below 150% poverty line (2022)         |
| Percent_Uninsured             | Numeric   | % population without health insurance (2022)        |
| Minority_Percentage           | Numeric   | % minority population (non-white)                  |
| yearly_avg_PM25_2000          | Numeric   | Yearly average PM2.5 (2000)                         |
| yearly_avg_PM25_2022          | Numeric   | Yearly average PM2.5 (2022)                         |
| Percent_Below_Poverty_2000    | Numeric   | % population below 100% poverty line (2000)         |
# Scripts and Code
## Included Scripts
- **data_wrangling.R**: Combines and cleans EPA and CDC datasets.
- **analysis_2000.R**: Conducts correlation and regression analysis for 2000 data.
- **analysis_2022.R**: Similar analysis for 2022 data, including PM2.5 trends.
- **comparison_analysis.R**: Examines changes between 2000 and 2022 using paired comparisons.
- **visualizations.R**: Generates graphs for trends and regression results.

US EPAUS EPA
Air Data: Air Quality Data Collected at Outdoor Monitors Across the US | US EPA
This site provides air quality data collected at outdoor monitors across the United States, Puerto Rico, and the U. S. Virgin Islands. Users can download, output, view or visualize the data.
Jul 9th, 2014 (273 kB)
https://www.epa.gov/outdoor-air-quality-data

Place and Health - Geospatial Research, Analysis, and Services Program (GRASP)Place and Health - Geospatial Research, Analysis, and Services Program (GRASP)
SVI Data & Documentation Download
Download the Social Vulnerability Index (SVI) data.