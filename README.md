# Capstone Project 1 - Intro and Column Description

In this capstone project, we will analyze GPS data from drivers who work for a machinery repair business. The data comes from a GPS vendor’s system – “InTouch GPS”. 

There are 214 drivers are part of the dataset, with their names replaced by a randomly generated code. The data is for 1 month, September 2016. 

Below are the column names and information: 

- **Name** – This is the name of the driver we are measuring. 
- **Overall** – This is the “Overall score”, which is calculated by the GPS system. This formula is designed to help calculate who is driving the most aggressively, wasting the most fuel with idle time, and so on.
- **Miles** – Total number of miles the driver drove in the time period. 
- **Duration** – Duration of driving in Hours : Minutes format. 
- **Highway %** - Percentage of time the user drove on the highway. This feature was not turned on for a number of months, including the sample. 
- **City %** - Percentage of time the user drove on in the city. This feature was not turned on for a number of months, including the sample.
- **Idle Time** – This is the total amount of time spent idle, in Hours : Minutes format. The definition of idle time is: any time the engine is spent running while the truck is not moving. The truck has to be parked for over 3 minutes for the idle time to engage - this should cut down on heavy traffic situations skewing idle time higher. 
- **Idling %** - Percentage of driving time the technician spent idling. 
- **Idling Score** – Score that the GPS vendor calculates to help measure how much the technician is idling. The formula is proprietary but seems to balance idling percentage, idling duration, and total miles and time driving. A high score is  good - imagine getting a high score on a test. A low score means that the driver is idling more often. 
- **Speeding Score** – Score that the GPS vendor calculates 
- 	**Highway and City % Fields** – These measure the percentage of time the driver spent speeding, and by how much. Example, if they had a 3% in the Highway 1-5 % that means they were speeding by 1-5 miles per hour 3% of the time they were driving on the highway. This measurement was only turned on for a few months in the larger dataset – in this particular sample of the data, it is all zero.
- **Acceleration** - This is the number of rapid acceleration events recorded by the device in the timeframe. Rapid acceleration events are an increase in speed of 6 miles per hour, per second, or greater. 
-**Braking** - This is the number of hard braking events recorded by the device in the timeframe. Hard Braking is defined as a decrease in speed of 8 miles per hour, per second, or greater. 
- **Aggression Score**- This is the proprietary calculation ranking that combines acceleration, braking, and total amount of driving. A high score is  good - imagine getting a high score on a test. A low score means that the driver is more aggressive. 

## Files
- **cap1dataclean.ipynb**  - This is the file for the data wrangling / cleaning assignment.
- **capstone1datastory.ipynb** - This file is for the EDA assignment.
- **Behavior09012016.csv** - This is the dataset for the initial analysis.
