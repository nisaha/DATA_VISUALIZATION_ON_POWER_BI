# DATA_VISUALIZATION_ON_POWER_BI

## Business Context/Summary:

The objective of the exercise is working and managing multiple tables. As part of this exercise, I loaded the data from multiple sources and defined and managed relationships between them. I used the DAX syntax to enhance the dataset.

## Situation

I have been provided with retail data; the data are in 4 disparate files. My eventual goal is to make a high level dashboard with different cuts, and some insights. As a first step, I need to get all 4 tables in my data model and ensure the relationships between the tables are well defined for further use. I am also required to add some fields in the data - to enable the different views - Net Units, Weekday vs Weekend performance, etc.

## Tasks
1. Load all the files, one by one into the data model-Make sure the header contains the field names in all the files
2. Drop records from table ‘PinCode-Geo’ where ‘Zone’ is missing. Drop records from ‘Mod3_Raw_CityTier_v0 1’ where ‘CityTier’ is missing.
3. For the common columns between tables, make sure the relationship is present. For the table ‘Mod3_Raw_CityTier_v0 1’, make sure the ‘City’ field has a relationship with ‘City’ from ‘PinCode-Geo’ table
4. Using DAX formulas, create a new column ‘Net_Units’ as difference of ‘Units’ and ‘Cancelled_Units’ in the sale table
5. Rename ‘City’ to ‘City_Old’, create new column ‘City’ with only the city name i.e. removing the country part; from the two files ‘‘Mod3_Raw_CityTier_v0 1‘ and ‘PinCode-Geo’.
6. Create a field called ‘OrderDayOfWeek’ which should contain the day of week, e.g. ‘Monday’
7. To be able to look at weekly trends, using DAX formulas, create a field called ‘OrderWeekStart’ which contains the date for the start of the week of sale. Note that your week should be starting from Monday - Format this field to display ‘Nov 06’ for November 6th
8. Update the relationships to ensure all tables are connected as expected
9. Create different analysis/reports like - Total revenue, Total quantity, Total cancelations, number of customers, number of transactions, by Month, week, weekday, product group, city, zone, city tier etc..
10. Create Dashboard with above analysis
