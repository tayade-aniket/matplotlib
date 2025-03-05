# What is Matplotlib
Visualizing data helps us understand and share information more effectively. In Python Matplotlib is one of the best tools for creating visualizations. It’s powerful, flexible, and lets you make many types of plots, from simple line charts to advanced animations. This tutorial will guide you step by step through using Matplotlib.

# Introduction to Matplotlib
Matplotlib is a powerful and versatile open-source plotting library for Python, designed to help users visualize data in a variety of formats. Developed by John D. Hunter in 2003, it enables users to graphically represent data, facilitating easier analysis and understanding. If you want to convert your boring data into interactive plots and graphs, Matplotlib is the tool for you.

## Setting Up Matplotlib
Before using Matplotlib, ensure you have it installed. You can install it using pip:

```bash
    pip install matplotlib
```

Once installed, you can import it into your Python script:

```bash
    import matplotlib.pyplot as plt
```

### Essential Role of Pyplot in Matplotlib
Pyplot is a submodule of the Matplotlib library in Python providing a beginner-friendly tool for creating visualizations with minimal code. It helps transform dull data into engaging and interactive plots, making it easier to analyze and draw meaningful insights for informed decision-making.

```bash
    matplotlib.pyplot.plot()
```

### Creating Different Types of Plots

#### 1. Line Graph
Line graphs are commonly used to visualize trends over time or relationships between variables. We’ll learn how to create visually appealing line graphs to represent such data.

#### 2. Bar chart
A bar plot or bar chart is a graph that represents the category of data with rectangular bars with lengths and heights that is proportional to the values which they represent. The bar plots can be plotted horizontally or vertically. A bar chart describes the comparisons between the discrete categories. It can be created using the bar() method.

#### 3. Plotting Histogram
Histogram is basically used to represent data in the form of some groups. It is a type of bar plot where the X-axis represents the bin ranges while the Y-axis gives information about frequency. To create a histogram the first step is to create a bin of the ranges, then distribute the whole range of the values into a series of intervals, and count the values which fall into each of the intervals. Bins are clearly identified as consecutive, non-overlapping intervals of variables.

#### 4. Scatter Plot
Scatter plots are ideal for visualizing the relationship between two continuous variables. We’ll see how scatter plots help identify patterns, correlations, or clusters within data points.

#### 5. Pie Chart
Pie Chart is a circular statistical plot that can display only one series of data. The area of the chart is the total percentage of the given data. The area of slices of the pie represents the percentage of the parts of the data. The slices of pie are called wedges. The area of the wedge is determined by the length of the arc of the wedge.

#### 6. Stack Plot
Stackplot is used to create stacked area plots. It is a great way to visualize the contributions of multiple categories over time or across other continuous variables. In a stackplot, the areas representing different groups are stacked on top of each other, which allows you to see both individual and cumulative data.

#### 7. Stem Plot
A stem plot, also known as a stem-and-leaf plot, is a type of plot used to display data along a number line. Stem plots are particularly useful for visualizing discrete data sets, where the values are represented as “stems” extending from a baseline, with data points indicated as “leaves” along the stems. let’s understand the components of a typical stem plot:

* Stems: The stems represent the main values of the data and are typically drawn vertically along the y-axis.
* Leaves: The leaves correspond to the individual data points and are plotted horizontally along the stems.
* Baseline: The baseline serves as the reference line along which the stems are drawn.

#### 8. Box Plot
A box plot, also known as a box-and-whisker plot, provides a visual summary of the distribution of a dataset. It represents key statistical measures such as the median, quartiles, and potential outliers in a concise and intuitive manner. Box plots are particularly useful for comparing distributions across different groups or identifying anomalies in the data.

#### 9. Error Plot
Error plots display the variability or uncertainty associated with each data point in a dataset. They are commonly used in scientific research, engineering, and statistical analysis to visualize measurement errors, confidence intervals, standard deviations, or other statistical properties of the data. By incorporating error bars into plots, we can convey not only the central tendency of the data but also the range of possible values around each point.

#### 10. Violin Plot
A violin plot is a method of visualizing the distribution of numerical data and its probability density. It is similar to a box plot but provides additional insights into the data’s distribution by incorporating a kernel density estimation (KDE) plot mirrored on each side. This allows for a more comprehensive understanding of the data’s central tendency, spread, and shape.

#### 11. 3D Plots in Matplotlib
Sometimes, data visualization requires a three-dimensional perspective. We’ll delve into creating 3D plots to visualize complex relationships and structures within multidimensional datasets.

# Matplotlib – Axes Class
Matplotlib is one of the Python packages which is used for data visualization. You can use the NumPy library to convert data into an array and numerical mathematics extension of Python. Matplotlib library is used for making 2D plots from data in arrays.

## Axes class
Axes is the most basic and flexible unit for creating sub-plots. Axes allow placement of plots at any location in the figure. A given figure can contain many axes, but a given axes object can only be in one figure. The axes contain two axis objects 2D as well as, three-axis objects in the case of 3D. Let’s look at some basic functions of this class.

### axes() function
axes() function creates axes object with argument, where argument is a list of 4 elements [left, bottom, width, height]. Let us now take a brief look to understand the axes() function.

```bash
    axes([left, bottom, width, height])
```

### add_axes() function
Alternatively, you can also add the axes object to the figure by calling the add_axes() method. It returns the axes object and adds axes at position [left, bottom, width, height] where all quantities are in fractions of figure width and height.

```bash
    add_axes([left, bottom, width, height])
```

### ax.legend() function
Adding legend to the plot figure can be done by calling the legend() function of the axes class. It consists of three arguments.

```bash
    ax.legend(handles, labels, loc)
```

### ax.plot() function
plot() function of the axes class plots the values of one array versus another as line or marker.

```bash
Syntax :  plt.plot(X, Y, ‘CLM’)


Parameters:

    X is x-axis.

    Y is y-axis.

    ‘CLM’ stands for Color, Line and Marker.
```

#### Note: Line can be of different styles such as dotted line (':'), dashed line ('—'), solid line ('-') and many more.

### Marker codes

| Characters |  Description     |
|:-----------|:----------------:|
| ‘.’        | Point Marker     | 
| ‘o’        | Circle Marker    | 
| ‘+’        | Plus Marker      | 
| ‘s’        | Square Marker    | 
| ‘D’        | Diamond  Marker  | 
| ‘H’        | Hexagon  Marker  | 
