# -Gayathri-Venugopalan-_-S2-
                SIGAI Recruitment Task
Objective
Analyze the given car price prediction dataset and use different preprocessing techniques to enhance it.
 
 Explanation
 
 Downloaded car price prediction dataset from Kaggle and saved it as a CSV file.
Imported pandas and numpy, two Python libraries to work with the dataset.
Pandas library works well for numeric, alphabets, and heterogenous types of data simultaneously while numpy library works better with only numeric data, has efficient storage, and fastly performs mathematical operations on array-based matrix-based numeric values.
The dataset is named dataset.csv. it can be loaded and analyzed using pandas.
The head() function displays the first few rows of the dataset providing a preview of its structure. The describe() function provides statistical information such as count, mean, standard deviation, quartiles, minimum and maximum values for each numerical column in the dataset.
Plotting graphical comparisons and analysis
Utilized pyplot module from the matplotlib library to plot the 4 different graphical comparisons and analyze them. For this imported matplotlib.pyplot as plt. First plotted Histogram. It is the graphical representation of grouped frequency distribution with continuous classes. It is an area diagram and can be defined as a set of rectangles with bases along with the intervals between class boundaries and areas proportional to frequencies in the corresponding classes.
Here production year and frequency is plotted.
Secondly bar graph is plotted. A bar graph is a graph that represents the category of data with rectangular bars with lengths and heights propotional to the values which they represent. A bar chart describes the comparisons between the discrete categories. One of the axis of the plot represents the specific categories being compared, while the other axis represents the measured values corresponding to those categories. Here it is plotted between price and fuel type.
Thirdly box plot is created. It is to display the summary of the set of data values having properties like minimum, first quartile, median, third quartile and maximum. In the box plot, a box is created from the first quartile to the third quartile, a vertical line is also there which goes through the box at the median. Here x-axis denotes the data to be plotted while the y-axis shows the frequency distribution. Cylinders are given in the x-axis.
Lastly, a scatter plot is created. Scatter plots are used to observe the relationship between variables and use dots to represent the relationship between them. Here cylinders and airbags are plotted in a scatter plot.
Checked for null values.
The isnull().sum() function returns the count of null values in each column. By using dropna() we can remove rows with null values. Since the rows and columns of the dataset before and after removing null values are same, the dataset does not contain any null values.

Standardization

Here Standardization is used. Standardization rescales the feature of the dataset to have zero mean and unit variance.It transforms the dataset in such a way that it has a mean of 0 and a standard deviation of 1. It does not have a specific range of features. It is suitable when the distribution of data is not necessarily Gaussian or when the scale of the feature varies significantly.
It is calculated by using X_standard=(X_mean)/std_dev
Here sklearn.preprocessing module is used to apply standardization. 
StandardScalar function from sklearn.preprocessing is used to apply standardization from the dataset. By applying standardization, the values of the selected columns will have a mean of 0 and a standard deviation 1. This helps to make the feature more comparable and suitable for machine learning algorithms that require standardized input. 

Displaying correlation matrix
 
 The corr() function computes the pairwise correlation between the columns of the dataset.dataset.corr() is stored in the variable correlation matrix and it is printed.
The correlation matrix will show the correlation coefficients between each pair of columns in the dataset. The values range from -1 to 1 where -1 represents a strong negative correlation, 1 represents a strong positive correlation and 0 represents no correlation.

