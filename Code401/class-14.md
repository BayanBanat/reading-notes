# Read: Class 14
## Data Visualization

**Reading Questions: **
1. 
**Matplotlib:**

* Matplotlib is a versatile and comprehensive plotting library in Python. It provides a wide range of options for creating static, publication-quality visualizations.
* Matplotlib is ideal for creating basic plots, such as line plots, scatter plots, bar charts, histograms, and pie charts. It offers fine-grained control over every aspect of the plot, allowing you to customize colors, markers, labels, and annotations.
Example: A line plot showing the trend of a stock's closing prices over time, with labeled x-axis ticks representing the dates.

 **Seaborn:**

* Seaborn is a statistical data visualization library built on top of Matplotlib. It focuses on providing high-level interfaces and functions for creating visually appealing statistical graphics.
* Seaborn is particularly suitable for exploring and visualizing relationships in complex datasets, statistical analysis, and visualizing distributions. It offers specialized plot types like violin plots, box plots, pair plots, and heatmaps.
Example: A seaborn scatter plot with a regression line, displaying the relationship between a car's horsepower and its fuel efficiency, with different colors representing the number of cylinders.

 **Bokeh:**

* Bokeh is a powerful library for creating interactive and visually rich visualizations in web browsers. It emphasizes interactivity and is well-suited for building interactive dashboards and exploratory data analysis.
* Bokeh allows you to create interactive plots with zooming, panning, tooltips, and other interactive features. It supports various plot types, including line plots, scatter plots, bar charts, and geographical maps.
Example: An interactive Bokeh scatter plot with tooltips, where each data point represents a city on a map, and the tooltip displays additional information about the city when hovering over it.

2. 
**Relational Plots:**

* Relational plots in Seaborn are used to visualize the relationship between two or more variables. They are particularly useful for identifying patterns, correlations, and trends in the data.
* The main function for creating relational plots in Seaborn is scatterplot(). It creates scatter plots by default but can also handle other plot types, such as line plots and regression plots.
Example use case: You can use scatterplot() to visualize the relationship between the temperature and humidity levels in different cities over time. Each point on the scatter plot represents a city, and the x and y axes represent temperature and humidity, respectively.

**Categorical Plots:**

* Categorical plots are used to display the distribution of data in different categories or groups. They help in comparing and analyzing data across different categories.
* The main functions for creating categorical plots in Seaborn include barplot(), countplot(), boxplot(), violinplot(), and pointplot().
Example use case: You can use barplot() to display the average sales of different products in a retail store. Each bar represents a product category, and the height of the bar represents the average sales volume.

**Distribution Plots:**

* Distribution plots in Seaborn are used to visualize the distribution of a single variable or compare the distributions of multiple variables.
* The main functions for creating distribution plots in Seaborn are histplot(), kdeplot(), rugplot(), and distplot() (deprecated in newer versions, replaced by histplot() and kdeplot()).
Example use case: You can use histplot() to visualize the distribution of students' exam scores. The histogram shows the frequency of scores within specific score ranges.

3. 
* Overview of Plot Types: The cheat sheet provides an overview of various plot types available in Seaborn, such as scatter plots, line plots, bar plots, histogram plots, and more. It gives developers a quick glimpse of the possibilities and helps them identify the appropriate plot type for their visualization needs.

* Data Structure Conversion: Seaborn works well with Pandas DataFrames, and the cheat sheet provides guidance on how to convert a Pandas DataFrame to the appropriate format for different plot types. This section helps developers understand the required data structure for each plot and how to transform their data accordingly.

* Customization Options: Seaborn offers a wide range of customization options to fine-tune the appearance and style of visualizations. The cheat sheet presents key customization elements such as colors, markers, line styles, axes labels, legends, and titles. Developers can quickly find the syntax and examples for customizing various aspects of their plots.

* Plotting Functions: The cheat sheet covers essential plotting functions in Seaborn, including scatter plots, line plots, bar plots, box plots, and more. For each function, it provides a brief description, syntax, and examples. This section allows developers to quickly locate the function they need and understand how to use it effectively.

* Statistical Estimation: Seaborn integrates statistical estimation functions to enhance data visualization. The cheat sheet highlights statistical estimation functionalities, such as kernel density estimation (KDE) plots, regression plots, and confidence interval plots. Developers can easily find information on how to incorporate statistical estimates into their visualizations.

* Plot Aesthetics: Seaborn focuses on creating visually appealing and informative plots. The cheat sheet provides guidance on plot aesthetics, such as choosing color palettes, adjusting figure size, setting plot styles, and adding annotations. Developers can refer to this section to enhance the visual impact of their plots.

## Things I want to know more about
Seaborn Tutorial
Bokeh Tutorial
