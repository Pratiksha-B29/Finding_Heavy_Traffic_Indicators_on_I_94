# Indicators of Heavy Traffic on I-94

## Project Overview 
In this project, we analyze a dataset about the westbound traffic on the I-94 Interstate highway to identify potential indicators of heavy traffic. These indicators could include weather conditions, time of day, or day of the week. Our goal is to determine what factors influence traffic volume and provide meaningful insights into traffic patterns.

The dataset contains 48,204 rows and 9 columns of hourly traffic and weather data, ranging from October 2012 to September 2018, and is free of null values. Traffic data was recorded by a station located midway between Minneapolis and Saint Paul, specifically for westbound traffic.

## Dataset 
- **Source:** The dataset was made available by John Hogue and can be downloaded from the UCI Machine Learning Repository.

- **Rows:** 48,204

- **Columns:** 9 (including traffic volume, weather data, and timestamp)

- **Time Period:** 2012-10-02 to 2018-09-30

- **No Missing Data:** All values are present and usable for analysis.

## Steps Involved

**1. Introducing the Dataset**
- Overview of dataset structure and contents.

- Key details: Traffic data was collected from 2012 to 2018 and focused on westbound traffic near a station between Minneapolis and Saint Paul.


**2. Analyzing Traffic Volume**
- Started by analyzing the distribution of the traffic_volume column. Traffic volume ranges from 0 to 7,280 cars per hour, with an average of 3,260 cars.

- Observed that 25% of the time, the traffic volume was below 1,193 cars, likely during the night or construction periods, while 25% of the time, it exceeded 4,933 cars.

**3.Traffic Volume: Day vs. Night:**
- We isolated and compared traffic volume during the day and night.

- Daytime Traffic: Traffic volume is left-skewed, with high traffic most of the time (75% of the time, over 4,252 cars per hour).

- Nighttime Traffic: Traffic volume is right-skewed, with low traffic most of the time (75% of the time, under 2,819 cars per hour).

- From this, we focused our further analysis on daytime traffic.

**4. Time Indicators:**
- Analyzed how traffic volume changes based on:
  - Month: Traffic is heavier during warm months (March–October) compared to cold months (November–February). July typically shows heavy traffic except for 2016, when road construction caused a dip.

  - Day of the Week: Traffic is higher on business days (Monday to Friday), particularly from Tuesday to Friday, with volumes often exceeding 5,000 cars. Weekends typically have lighter traffic.

  - Time of Day: Rush hours (around 7 AM and 4 PM) show the heaviest traffic, often exceeding 6,000 cars on business days.
 
**5. Weather Indicators :**
- We examined the correlation between traffic volume and weather conditions. The only slightly positive correlation was with temperature (+0.13), suggesting temperature isn’t a strong indicator of heavy traffic.

- We also grouped the data by weather types:
  - Shower snow, light rain and snow, and proximity thunderstorms with drizzle showed traffic volumes exceeding 5,000 cars on average.
 
## Key Findings
**Time Indicators:**

**Month:**  Heavier traffic in warm months (March–October) than cold months (November–February).

**Day of the Week:**  Heavier traffic on business days (Monday to Friday) than on weekends.

**Time of Day:** Rush hours around 7 AM and 4 PM have the highest traffic volume during business days.

**Weather Indicators:** 

- Shower snow

- Light rain and snow

-  Proximity thunderstorm with drizzle

## Conclusion
In this project, we identified two key types of indicators that contribute to heavy traffic on the I-94 westbound:

**Time Indicators:**

- Heavy traffic during warm months.

- Heavy traffic on business days.

- Rush hours (7 AM and 4 PM) during business days see the highest traffic volumes.

**Weather Indicators:**

- Bad weather such as shower snow, light rain and snow, and proximity thunderstorms with drizzle also result in higher traffic volumes, possibly because more people prefer driving in such conditions.

## Tools & Libraries Used
- Python (Pandas, NumPy, Matplotlib, Seaborn)

- Jupyter Notebook

## Contact

[Email](@pratikshabj77@gmail.com)

[LinkedIn](https://www.linkedin.com/in/pratikshabajpai29/)










