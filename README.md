# Python Pie Chart
This builds on the earlier [Python Bar Chart](https://github.com/teochewthunder/python-bar-chart). Differences are highlighted below.

## Data
- Same as Python Bar Chart.

## Script
- Generate a list of Seasons from the data.
- Generate a list of Players from the data. Iterate through `data`, adding player names to a list. After that, convert the list to a dictionary, which automatically removes all duplicates, then convert back to a list, and sort.
- Request the user to enter a choice from list of Seasons.
  - Utilize a `Try-catch` to ensure only numerical data is entered.
  - If value is numerical but out of bounds, do-over.
  - If value is 0, end program.
- Request the user to enter 1 for Goals and 2 for Appearances.
  - Utilize a `Try-catch` to ensure only numerical data is entered.
  - If value is numerical but out of bounds, do-over.
  - If value is 0, end program.
- Use the selected season and stat to generate the Pie Chart.

## Chart
We use the `matplotlib` library to plot the pie chart.
- `colors` is an argument passed into the `pie()` method. It is a list that contains Hex values. The pie wedges will be colored accordingly.
- `explode` is an argument passed into the `pie()` method. It is a list that contains float values between 0 and 1. The pie wedges will be displaced from the center according to the value.
