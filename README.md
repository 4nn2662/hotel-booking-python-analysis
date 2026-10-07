# Hotel Booking Demand Analysis

## Project Overview

This project analyzes hotel booking data to identify patterns in booking behavior, cancellations, seasonality, and pricing. 
The analysis focuses on answering business-oriented questions using Python, Pandas, and NumPy, followed by visualizations of the most relevant findings.

## Dataset

The analysis uses the Hotel Booking Demand dataset, which contains booking information for a City Hotel and a Resort Hotel.

The dataset includes 119,390 records and 32 variables covering booking characteristics such as cancellations, lead time, arrival dates, 
length of stay, number of guests, average daily rate (ADR), market segment, special requests, and room information.

Source: [Hotel Booking Demand – Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)

## Technologies

- **Python** – data analysis and transformation
- **Pandas** – data cleaning, manipulation, aggregation, and exploratory analysis
- **NumPy** – numerical operations and handling missing values
- **Matplotlib** – visualization of the most relevant findings
- **Jupyter Notebook** – development and presentation of the analysis

## Data Cleaning and Preparation

Before performing the analysis, the dataset was inspected and prepared to ensure data quality and consistency. The main steps included:

- Identifying and handling missing values
- Investigating duplicate records
- Removing bookings with no guests
- Validating unusual values in ADR, length of stay, and number of guests
- Converting date columns to appropriate datetime formats
- Creating additional variables such as total number of guests, total nights, lead time groups, and room change indicators
- Retaining potentially valid unusual observations where there was insufficient evidence to classify them as errors

## Business Questions

The analysis addresses several business-oriented questions, including:

- What is the overall booking cancellation rate?
- Does the cancellation rate differ between City Hotel and Resort Hotel?
- How does booking lead time affect the likelihood of cancellation?
- How do booking volume and cancellation rates vary throughout the year?
- How does median ADR differ between hotel types and across months?
- Are repeated guests less likely to cancel their bookings?
- Is the number of special requests associated with cancellation behavior?
- Does the length of stay affect cancellation rates?
- Which market segments have the highest cancellation rates?
- Are room changes or parking requirements associated with cancellation behavior?

## Key Insights

- **Cancellation behavior:** 37.08% of all bookings were canceled. City Hotel had a substantially higher cancellation rate (41.79%) than Resort Hotel (27.77%).

- **Lead time:** Cancellation risk increased strongly with booking lead time, 
from 9.60% for bookings made 0–7 days in advance to 67.65% for bookings made more than one year in advance.

- **Seasonality:** Booking volume peaked in August (13,861 bookings) and July (12,644), while January recorded the lowest booking volume (5,921).

- **Pricing patterns:** Resort Hotel showed strong seasonal variation in median ADR, peaking at 188.42 in August. 
City Hotel pricing was considerably more stable throughout the year.

- **Guest engagement:** Repeated guests had a much lower cancellation rate than new guests (14.65% vs. 37.81%). 
Bookings with special requests were also associated with lower cancellation rates.

- **Booking characteristics:** Group bookings showed the highest meaningful cancellation rate among market segments (61.11%). 
Bookings requiring parking and bookings with a different assigned room type were associated with particularly low cancellation rates; 
however, these relationships should not be interpreted as causal.

## Visualizations

The project includes visualizations highlighting the most relevant findings from the analysis:

- Cancellation rate by booking lead time
- Median ADR by month and hotel type
- Booking volume by month
- Cancellation rate by number of special requests

All visualizations are available in the Jupyter Notebook included in this repository.

## Repository Structure

- `hotel_booking_analysis.ipynb` – complete data cleaning, exploratory data analysis, visualizations, and conclusions
- `README.md` – project overview and summary of the main findings
