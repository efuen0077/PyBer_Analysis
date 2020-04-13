# PyBer_Analysis
This is my work from week 5 of the Data Analytics Bootcamp.

## Challenge

### Background
You’ve been asked by your CEO to create an overall snapshot of the ride-sharing data. In addition to your scatter and pie charts, she would like to see a summary table of key metrics of the ride-sharing data by city type, and a multiple-line graph that shows the average fare for each week by each city type.

### Objectives
The goals for this challenge are for you to:

    Use Pandas functions like groupby, pivot, resample, and reset_index on a DataFrame.
    Use Pandas methods and attributes on a DataFrame or Series.
    Create a new DataFrame from multiple groupby() Series.
    Format columns of a DataFrame.
    Create a multiple-line graph.
    Annotate and apply styling to the chart.

### Instructions:

#### Part 1: Create PyBer Summary DataFrame

##### Create a summary DataFrame that showcases the following for each city type:

    Total Rides
    Total Drivers
    Total Fares
    Average Fare per Ride
    Average Fare per Driver
#### SUMMARY DATAFRAME

[final_summary_df.zip](https://github.com/efuen0077/PyBer_Analysis/files/4463976/final_summary_df.zip)

[PyBer-Challenge.ipynb.zip](https://github.com/efuen0077/PyBer_Analysis/files/4463977/PyBer-Challenge.ipynb.zip)

### Analysis for Part I:


#### Part 2: Create a Multiple-Line Plot for the Sum of the Fares for Each City Type
    Plot the sum of the fares for each city type.
    
    After merging the DataFrames, do the following:

    1. Rename columns {'city': 'City', 'date':'Date','fare':'Fare', 'ride_id': 'Ride Id','driver_count': 'No. Drivers', 'type':'City Type'}.
    2. Set the index to the Date column.
    3. Create a new DataFrame for fares and include only the Date, City Type, and Fare columns using the copy() method on the merged DataFrame.
    4. Drop the extra Date column.
    5. Set the index to the datetime data type.
    6. Check the DataFrame using the info() method to make sure the index is a datetime data type.
    7. Calculate the sum() of fares by the type of city and date using groupby() to create a new DataFrame.
    8. Reset the index, which is needed for Step 10.
    9. Create a pivot table DataFrame with the Date as the index and columns = 'City Type' with the Fare for each Date in each row. Note: There will be NaNs in some rows, which will be taken care of when you sum based on the date.
    10. Create a new DataFrame from the pivot table DataFrame on the given dates '2019-01-01':'2019-04-28' using loc .
    11. Create a new DataFrame by setting the DataFrame you created in Step 11 with resample() in weekly bins, and calculate the sum() of the fares for each week.
    
    Using the object-oriented interface method, plot the DataFrame you created in Step 12 using the df.plot() function. Things to consider with your plotting:
        Import the style from Matplotlib.
        Use the graph style fivethirtyeight.
        Add a title.
        Add x- and y-axes labels according to the final figure.
        Save the figure to the “analysis” folder.
        Make the figure size large enough so it’s not too small.
#### Plot of DataFrame --> Fares by City Type

###### Complete Code for this challenge
[PyBer-Challenge.ipynb 2.zip](https://github.com/efuen0077/PyBer_Analysis/files/4467837/PyBer-Challenge.ipynb.2.zip)

###### Line Chart
![Fares_by_City_Type](https://user-images.githubusercontent.com/62089134/79089252-58b2c300-7cfa-11ea-87a7-7ff90824903d.png)

### Analysis for Part II:

