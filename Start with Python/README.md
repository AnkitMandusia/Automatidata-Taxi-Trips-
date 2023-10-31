# Automatidata Project : Get Started with Python

Welcome to the Automatidata Project!

## Project Background
Automatidata is in the earliest stages of the TLC project. The primary tasks include building a dataframe for the TLC dataset, examining the data types of each column, and gathering descriptive statistics. The purpose of this project is to prepare the New York City Taxi and Limousine Commission (TLC) data for analysis and generate initial insights.

## Specific Project Deliverables
- Complete the questions in the Course 2 PACE strategy document.
- Answer the questions in the Jupyter notebook project file.
- Complete coding prep work on the project's Jupyter notebook.
- Summarize the column data types.
- Communicate important findings to DeShawn and Luana in the form of an executive summary.

## PACE Stages
This project follows the PACE (Plan, Analyze, Construct, Execute) framework:

### PACE: Plan
- Task 1: Understand the Situation
  - Prepare to understand and organize the provided taxi cab information.
- Task 2: Analyze
  - Create a pandas dataframe for data learning, future exploratory data analysis (EDA), and statistical activities.

### PACE: Analyze
- Task 2a: Build Dataframe
  - Create a pandas dataframe for data learning and future analysis.
- Task 2b: Understand the Data - Inspect the Data
  - View and inspect summary information about the dataframe.
- Task 2c: Understand the Data - Investigate the Variables
  - Sort and interpret the data table for two variables: trip_distance and total_amount.

## Important Findings
- Data Types: The dataset consists of various data types, including non-numeric and datetime fields. There are no null values.
- Variable Distributions: The distribution of fare_amount and trip_distance contains noteworthy points. For fare_amount, the maximum value is significantly higher than the 25-75 percent range, and there are negative values. For trip_distance, most rides are between 1-3 miles, but some are over 33 miles.
- Payment Types: The dataset includes multiple payment types, with credit card payments (payment_type=1) being the most common. The average tip for credit card payments is approximately 2.73, while cash payments have an average tip of 0.0.
- Vendor IDs: Vendor ID 2 is more prevalent in the dataset compared to Vendor ID 1. The mean total amount for both vendors is similar.
- Passenger Counts: Passenger count varies from 0 to 6, with most rides having one passenger. The average tip amount varies slightly based on the passenger count, with one passenger rides having the highest average tip.

## Next Steps
The project lays the foundation for further data analysis and modeling. The variables trip_distance and total_amount are likely to be important for predicting taxi ride fares. Future steps involve more in-depth analysis, hypothesis testing, and statistical methods.

For more detailed information, explore the project files and Jupyter notebook.

---

**Dependencies:** Python, Pandas, Numpy

**Data Source:** TLC dataset

**Acknowledgments:** Automatidata, New York City TLC
