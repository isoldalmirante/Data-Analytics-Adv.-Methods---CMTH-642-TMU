**Assignments completed for the Data Analytics Advanced Methods course Spring/Summer 2023**

**Course Description**
This course builds on the previous Basic Methods course and covers more advanced concepts including classification and clustering algorithms, decision trees, linear and logistic regression, 
time series analysis, and text analytics. The course will provide applied knowledge on how to analyze large scale network data produced through social media. In this context topics include 
network community detection, techniques for link analysis, information propagation on the web and information analysis of social media.

**Learn how to:**

- Manage advanced data cleansing to prepare the data for analysis.
- Perform statistical comparisons by hypothesis testing.
- Explore how to practically analyze large scale network data with the use of models for network structure and evolution.
- Optimize the structures and dynamics of self-organizing networks such as the Web.
- Differentiate between parametric and non-parametric statistical testing.
- Recognize feature selection techniques for use in modeling.
- Contextualize and leverage small world phenomena.
- Know how to build statistical learning models for clustering, classification, and regression to represent domains under study using R and Python.
- Identify available problem-solving approaches and methods.
- Develop an overall understanding of experimental design in data science projects.
- Recognize the dimensionality reduction techniques for big datasets.

**Assignment 1**

At the outset of the exercise, I read a CSV file from the provided URL, storing the data in a dataframe called Forest and checking the first six lines. 
Then, I determined the number of observations in the dataset and created subsets for burned areas and rain greater than zero. However, when attempting 
to compute the number of observations with both conditions true, I encountered an issue with the intersect function, resulting in a NULL output. 
Moving forward, I selected the month, day, and area columns for observations with burned area greater than zero and identified the top five largest fires. 
I reordered the factor levels of the month column, added a column indicating whether a fire occurred in each observation, and calculated the mean area, wind, 
temperature, and relative humidity per month. Lastly, I visualized the number of observations in each month and the number of observations with burned area 
greater than zero in each month, creating bar plots with ggplot2.

**Assignment 2**

In this assignment, I began by importing necessary libraries and reading the CSV file from the provided URL using pandas. After saving the data into a dataframe 
called Forest, I checked the first five records. Then, I calculated the total number of observations and identified observations with significant fires and rain. 
Subsequently, I displayed the columns month, day, and area for all observations with a significant fire. Additionally, I determined the five largest fires based
on the area. For these records, I extracted corresponding values of month, temp, RH, wind, rain, and area. Next, I reordered the factor levels of the month column 
from Jan to Dec. Following this, I added a new column indicating whether a fire occurred for each observation based on the area values. Moreover, I calculated the 
mean area, wind, temperature, and relative humidity per month. Finally, I visualized the number of observations in each month and the number of observations with 
burned area greater than zero in each month using bar plots with seaborn and matplotlib.

**Assignment 3**

In this assignment, I began by importing the necessary libraries and reading the red and white wine datasets from their respective URLs. 
After adding a new column to each dataset to distinguish between red and white wines, I concatenated them vertically to create a combined dataset called wine_data_all.
Subsequently, I addressed various questions regarding data exploration and preprocessing. I checked the data types of the attributes, looked for missing values (which were not found),
calculated the correlation between attributes, and plotted the frequency distribution of wine quality.
Next, I reduced the levels of wine quality ratings to two categories: "Pass" and "Fail". Then, I normalized the numeric attributes using the provided formula.
Afterward, I split the dataset into training and test sets and applied logistic regression and K-nearest neighbors (KNN) algorithms to predict wine quality. 
For both algorithms, I evaluated their performances using accuracy, precision, and recall metrics.
Finally, I displayed two confusion matrices to further evaluate the performances of logistic regression and KNN. Each step was followed by a concise explanation 
of the results obtained, providing a clear understanding of the models' performances and the evaluation metrics used.
