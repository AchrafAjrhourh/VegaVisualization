# Description: 
A repository containing a dataset of abalone physical measurements, sex, and age, along with data visualizations using Vega-Lite to explore patterns and trends.

# Abstract:
This repository focuses on the analysis of abalone physical measurements and age. The dataset consists of 4177 rows and 9 columns, containing data on abalone sex, length, diameter, height, whole weight, shucked weight, viscera weight, shell weight, and rings (which represent age). The objective is to gain insights into the relationships between the physical measurements and the age of abalones, potentially identifying patterns or trends.

Two primary tasks are performed on the dataset using Vega-Lite for visualization:

Compare the distributions of physical measurements (length, diameter, height, whole weight, shucked weight, viscera weight, and shell weight) between male and female abalones. This is done by creating separate histograms for each physical measurement column based on sex.
Investigate the relationship between the age of abalones (represented by rings) and their physical measurements. This is accomplished by creating scatterplots for each physical measurement column with the Rings column on the y-axis.
These visualizations can help provide a better understanding of the dataset and lead to further analysis in the field of marine biology, specifically in the study of abalone growth patterns and factors affecting their physical development.

## Visualization 1 - Part 1: Distribution of Shell Lengths by Sex
The first visualization is a bar chart that shows the distribution of shell lengths for different sexes of abalones. The X-axis represents the shell length (in mm), the Y-axis represents the count of abalones, and the color represents the sex (M: Male, F: Female, I: Infant).

![alt text](https://github.com/AchrafAjrhourh/VegaVisualization/blob/master/Assets/V1-P1.png)

To create this visualization, we used the following encodings in the Vega Lite code:

x: Length (ordinal, binned)

y: Count of abalones (quantitative, aggregated using count)

color: Sex (nominal)

## Visualization 1 Part 2: Relationship between Whole Weight and Shucked Weight by Sex
The second visualization is a scatter plot that displays the relationship between the whole weight and shucked weight of abalones for each sex. The X-axis represents the whole weight (in grams), the Y-axis represents the shucked weight (in grams), and the color represents the sex (M: Male, F: Female, I: Infant).

![alt text](https://github.com/AchrafAjrhourh/VegaVisualization/blob/master/Assets/V1-P2.png)

To create this visualization, we used the following encodings in the Vega Lite code:

x: Whole weight (quantitative)

y: Shucked weight (quantitative)

color: Sex (nominal)

### Combined Visualizations
I've  combined both visualizations into a single Vega Lite code that creates a vertically stacked layout. This code can be found in the **visualizations1.vl.json** file.
