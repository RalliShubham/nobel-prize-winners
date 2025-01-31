# nobel-prize-winners
This project analyzes Nobel Prize winner data to identify patterns and answer key questions regarding award trends, gender distributions, country statistics, and multiple award winners. 

## Project Overview

This project analyzes Nobel Prize winner data to identify patterns and answer key questions regarding award trends, gender distributions, country statistics, and multiple award winners. The dataset used in this project is nobel.csv, which contains information on laureates, including their birth country, gender, award category, and year of achievement.

Objectives

The project aims to answer the following questions:

What is the most commonly awarded gender and birth country?

What decade had the highest proportion of US-born winners?

What decade and category pair had the highest proportion of female laureates?

Who was the first woman to receive a Nobel Prize, and in what category?

Which individuals or organizations have won multiple Nobel Prizes throughout the years?

Technologies Used

Python: Primary programming language for data analysis.

Pandas: Data manipulation and analysis.

NumPy: Numerical computing support.

Seaborn: Data visualization.

Matplotlib: Plotting and graphical representation.

Math Library: Support for mathematical computations.

Implementation Details

1. Identifying the Most Commonly Awarded Gender and Birth Country

Used value_counts() to determine the most frequent gender and birth country.

Stored results in variables top_gender and top_country.

2. Decade with the Highest Proportion of US-born Winners

Created a decade column by binning the year column into decades.

Filtered records for winners born in the USA.

Grouped by decade and counted occurrences.

Identified the decade with the highest count and stored it as max_decade_usa.

Visualized the trend using seaborn.

3. Identifying the Decade and Category with the Highest Proportion of Female Laureates

Created a boolean column women for filtering female winners.

Grouped data by decade and category, computing the mean proportion of female winners.

Extracted the decade-category pair with the highest proportion and stored it as max_female_dict.

Visualized trends using seaborn.

4. First Woman to Receive a Nobel Prize

Filtered data for female winners.

Sorted by year to identify the earliest laureate.

Extracted the name and category and stored them in first_woman_name and first_woman_category.

5. Identifying Individuals or Organizations with Multiple Nobel Prizes

Grouped data by laureate_id and full_name, counting prize occurrences.

Filtered records where the count was >=2.

Stored names of repeat winners in a list called repeat_list.

Results

The most commonly awarded gender is Male, and the most commonly awarded birth country is United States of America.

The decade with the highest proportion of US-born winners is 2000.

The decade-category pair with the highest proportion of female laureates was identified and stored in max_female_dict.

The first woman to win a Nobel Prize was Marie Curie in Physics.

Several individuals and organizations have won multiple Nobel Prizes, stored in repeat_list.

Visualizations

The project includes graphical representations such as:

Line charts for Nobel Prize trends over decades.

Category-wise analysis of female laureates.

Conclusion

This analysis provides insights into Nobel Prize award distributions, gender representation, and the dominance of certain countries and individuals in receiving multiple prizes. The project utilizes data science techniques and visualization tools to derive meaningful conclusions from historical award records.

How to Run

Ensure Python and required libraries (pandas, numpy, seaborn, matplotlib) are installed.

Place nobel.csv in the appropriate directory.

Run the script to generate results and visualizations.

Future Improvements

Enhance data preprocessing to handle missing values more effectively.

Explore additional patterns such as collaborations, age distributions, and trends in specific fields.

Automate data updates for real-time insights.


