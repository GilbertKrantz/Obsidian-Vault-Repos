# Matplotlib
## import Matplotlib.pylot
```python
import Matplotlib.pylot as plt
```

## Code
### Data Visualization

#### Histogram
Histogram is a type of graph or plot that is used to display the distribution of numerical data. It shows the frequency, or number of occurrences, of different values in a dataset. You can create it using `matplotlib.pylot` by using the `.hist()` function.
```python
data = [2, 4, 5, 7, 6, 8, 9, 12, 14, 15, 17, 19, 22, 25, 26, 28] 
# use pyplot to create a histogram 
plt.hist(data) 
# show the plot 
plt.show()
```
---

#### Bar Chart
Bar chart, also known as a bar graph, is a type of chart that uses rectangular bars to represent different values or quantities. Each bar typically represents a different category, and the length of the bar indicates the magnitude or size of the value it represents. You can create it using `matplotlib.pylot` by using the `.bar()` function and `.barh()` function to create vertical bars.
```python
# create some data to plot 
categories = ['Category 1', 'Category 2', 'Category 3'] 
values = [10, 20, 30] 
# use pyplot to create a bar chart 
plt.bar(categories, values) 
# show the plot 
plt.show()
```
---

#### Line Chart
Line charts are useful for showing the trend or pattern of a dataset over time or across different categories. They can also be used to compare multiple datasets to see how they are similar or different. You can create it using `matplotlib.pylot` by using the `.plot()` function.
```python
# create some data to plot 
categories = ['Category 1', 'Category 2', 'Category 3'] 
values = [10, 20, 30] 
# use pyplot to create a line chart 
plt.plot(categories, values) 
# show the plot 
plt.show()
```
---

#### Scatter Plot
Scatterplots are useful for showing the relationship between two variables and for visualizing the distribution of a dataset. They can also be used to identify trends and patterns in the data. You can create it using `matplotlib.pylot` by using the `.scatter()` function.
```python
# create some data to plot 
x = [1, 2, 3, 4, 5] 
y = [2, 4, 6, 8, 10] 
# use pyplot to create a scatterplot 
plt.scatter(x, y) 
# show the plot 
plt.show()
```
---

#### Boxplot
Boxplot, also known as a box-and-whisker plot, is a type of chart that uses quartiles and whiskers to represent the distribution of a dataset. It is a simple and effective way to visualize the spread and skewness of a data set, as well as to identify potential outliers. You can create it using `matplotlib.pylot` by using the `.boxplot()` function.
```python
# create some data to plot 
data = [2, 4, 5, 7, 6, 8, 9, 12, 14, 15, 17, 19, 22, 25, 26, 28] 
# use pyplot to create a boxplot 
plt.boxplot(data) 
# show the plot 
plt.show()
```
---

