# About the Author
Kimberly Staudt is a graduate student pursuing Data Science at Mercyhurst University.\
Email:kstaud85@lakers.mercyhurst.edu\
License: None

This is a data visualization project for the course DATA 550.
This project utilizes data from the Wall Street Journal's kernal "Where it Pays to Attend College".
This project seeks to compare salaries by college type. 
Bokeh plots often are created as an html outfile. A screenshot of the output is provided. 

# Repository Contents
1.Readme \
2.College type csv file (data)\
3.Jupyter Notebook file (cleaning, plotting, visualizations)\
4.bokeh_plot.png (bokeh plot)\
5.barchart.png\
6.data1.png (first 5 observations)\
7.heatgraph.png\
8.graph1.png (kde plot)

# Table of Contents
I.Purpose\
II. About the Data\
III.Packages\
IV.Project Explanation\
V.Conclusion\
VI.Related Efforts 

# I. Purpose

The purpose of this project is to find, clean, plot, and visualize the college type data set.

# II. About the Data

The data consists of 8 columns and 1856 observations. 
Given that that n>50, where n is the sample size, the size of the data set is satisfactory. 

The rows are as following:

School Name: Name of the academic instituion observed.\
School Type: Catagorical list of the intstitutions reputation (state,party,ivy league, engineering, or liberal arts)\
Starting Median Salary: The midpoint value in the sample's distribution for those starting their careers. Half of graduates made above or below this salary.\
Mid-Career Median Salary: The midpoint value in the sample's distribution for those in the middle of their careers.\
Mid-Career 10th Percentile Salary: Those who made 10% more compared to others by mid-salary. \
Mid-Career 25th Percentile Salary: Those who made 25% more compared to others by mid-salary. \
Mid-Career 75th Percentile Salary: Those who made 75% more compared to others by mid-salary. \
Mid-Career 90th Percentile Salary: Those who made 90% more compared to others by mid-salary. 

# III. Packages

The following packages need to be installed:pandas, seaborn, regex, numpy, bokeh, and matplotlib.\
Important tools used for data visualization are pandas,numpy, seaborn,bokeh, and matplotlib.\
Regex is used to clean/scrub the data. 

# IV.Project Explanation
The following are lines and explanations for each input.

In[2] Import the packages listed above, remove warnings,import the csv file, and view the data. \
In[3] Check the type of data to make sure it's a dataframe.\
In[5] Check for any missing values.\
In[6] Since some values are missing, drop those values.\
In[7] Now that these values have been dropped, re-check for any missing values just to make sure the data is clean.\
In[8] Change strings to floats (remove: $ ,). Specify the columns that you want to change or not change, as they must be numeric.\
In[9] View the data once more. Now that it is clean, we can begin to graph.\
![alt text](https://github.com/kstaud85/dvproject2/blob/master/data1.png)\
In[10] View the number of schools by type, using value_counts().\
In[24] Use Seaborn's FacetGrid kdeplot to view univariate density.\
![alt text](https://github.com/kstaud85/dvproject2/blob/master/graph1.png)\
In[25] Likewise, use heatmap to view salary correlations. This allows us to see the relationship between starting salary and various mid-career salaries.\
![alt text](https://github.com/kstaud85/dvproject2/blob/master/heatgraph.png)\
In[26] Use plt.bar to create a barchart, where the average salarie is plotted against the school type.\
![alt text](https://github.com/kstaud85/dvproject2/blob/master/barchart.png)\
In[27] Use bokeh.chart to create a stunning visualization that plots starting salary against school type. 
![alt text](https://github.com/kstaud85/dvproject2/blob/master/bokeh_plot.png)

# V.Conclusion

In conclusion, I found school type to be correlated with the mid-salary median.\
Perhaps this is because schools like Ivy Leagues, which had higher salaries, \
had more resources and had a bias towards students whom chose lucrative fields.\
An improvement to this dataset could be adding variables such as the average unemployment rate for graduates. 

# VI. Related Efforts

This kernal currently has many attempts to reproduce it on kaggle. 






