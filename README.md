# Ice Cream Ratings Analysis

## Overview

This Python script analyzes ice cream ratings data stored in a CSV file using the pandas library. It explores various visualization techniques to understand and interpret the ratings given to different flavors of ice cream.

## Requirements

- Python 3.x
- pandas library
- numpy library
- matplotlib library

## Usage

1. Ensure you have Python installed on your system.
2. Install the required libraries by running `pip install pandas numpy matplotlib` in your terminal or command prompt.
3. Download the 'Ice Cream Ratings.csv' file and place it in the same directory as the Python script.
4. Run the script 'ice_cream_ratings_analysis.py'.

## Description

- **Reading Data:** The script reads the ice cream ratings data from the CSV file using pandas, with the 'Date' column set as the index.

![Reading Data](/screenshots/reading_data.png)

- **Exploratory Data Analysis and Visualization:**

    - **Line Plots:** The script generates line plots to visualize the ice cream ratings over time.

    ![Line Plots](/screenshots/line_plots.png)

    - **Subplots:** Multiple line plots are created as subplots to compare different aspects of the ratings.

    ![Subplots](/screenshots/subplots.png)

    - **Bar Plots:** Bar plots are used to visualize the ratings of different flavors of ice cream. Stacked and horizontal bar plots are also demonstrated.

    ![Bar Plots](/screenshots/bar_plots.png)

    - **Scatter Plot:** A scatter plot is created to visualize the relationship between texture and overall ratings.

    ![Scatter Plot](/screenshots/scatter_plot.png)

    - **Histogram:** The distribution of ratings is visualized using a histogram.

    ![Histogram](/screenshots/histogram.png)

    - **Box Plot:** A box plot is generated to show the distribution of ratings and identify any outliers.

    ![Box Plot](/screenshots/box_plot.png)

    - **Area Plot:** An area plot is created to visualize the cumulative sum of ratings over time.

    ![Area Plot](/screenshots/area_plot.png)

    - **Pie Chart:** A pie chart is generated to represent the distribution of ratings for different flavors of ice cream.

    ![Pie Chart](/screenshots/pie_chart.png)

## Output

The script produces various visualizations to analyze the ice cream ratings data and gain insights into the quality and popularity of different flavors.

## Author

[Your Name]

## License

This project is licensed under the [MIT License](LICENSE).
