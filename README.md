# Clustering: Household Electricity Consumption Dataset
This directory applies clustering and some data analysis on a dataset which contains the electric power consumption data from a household near France.
This Data was taken from [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption). With this directory, I document my portfolio examination at my university. This dataset contains **2,075,259** measurements gathered in a house located in Sceaux, France, approximately 7km from Paris, between December 2006 and November 2010, spanning a total of **47 months**.

## Notes:

1. **Active Energy Consumption Calculation:**
   - The formula `(global_active_power*1000/60 - sub_metering_1 - sub_metering_2 - sub_metering_3)` is used to compute the active energy consumed every minute (in watt-hour) in the household by electrical equipment not measured in sub-meterings 1, 2, and 3.

2. **Missing Values:**
   - The dataset contains some missing values in the measurements, accounting for nearly 1.25% of the rows.
   - All calendar timestamps are present in the dataset, but for some timestamps, the measurement values are missing.
   - A missing value is represented by the absence of a value between two consecutive semi-colon attribute separators.
   - For instance, the dataset shows missing values on April 28, 2007.

## Dataset Attributes:

1. `date`: Date in format dd/mm/yyyy.
2. `time`: Time in format hh:mm:ss.
3. `global_active_power`: Household global minute-averaged active power (in kilowatt).
4. `global_reactive_power`: Household global minute-averaged reactive power (in kilowatt).
5. `voltage`: Minute-averaged voltage (in volt).
6. `global_intensity`: Household global minute-averaged current intensity (in ampere).
7. `sub_metering_1`: Energy sub-metering No. 1 (in watt-hour of active energy). It corresponds to the kitchen, containing mainly a dishwasher, an oven, and a microwave (hot plates are not electric but gas-powered).
8. `sub_metering_2`: Energy sub-metering No. 2 (in watt-hour of active energy). It corresponds to the laundry room, containing a washing-machine, a tumble-drier, a refrigerator, and a light.
9. `sub_metering_3`: Energy sub-metering No. 3 (in watt-hour of active energy). It corresponds to an electric water-heater and an air-conditioner.

## Data Preprocessing:

- Handling missing values: Implementing appropriate strategies such as interpolation or imputation.
- Data cleaning: Removing any anomalies or inconsistencies in the dataset.
- Data transformation: Converting data types if necessary, scaling numerical features, and encoding categorical variables.

## Analysis and Modeling:

- Exploratory Data Analysis (EDA): Understanding the distributions, patterns, and relationships within the dataset.
- Feature engineering: Creating new features or transforming existing ones to enhance model performance.
- Modeling: Utilizing clustering algorithms to find patterns in the dataset.
- Evaluation: Assessing model performance using appropriate metrics and validating against test datasets.
- Interpretation: Drawing insights from the models to understand factors influencing electricity consumption.
