# Data Science Study Plan

## The Data Science Method
How to approach a data science problem in an organized and outcomes oriented manner.

**[The Data Science Method](https://medium.com/@aiden.dataminer/the-data-science-method-dsm-a-framework-on-how-to-take-your-data-science-projects-to-the-next-91f9fd81e5d1)**

1.  [Problem Identification](https://medium.com/@aiden.dataminer/the-data-science-method-problem-identification-6ffcda1e5152)
2.  [Data Wrangling](https://medium.com/@aiden.dataminer/the-data-science-method-dsm-data-collection-organization-and-definitions-d19b6ff141c4)
3.  [Exploratory Data Analysis](https://medium.com/@aiden.dataminer/the-data-science-method-dsm-exploratory-data-analysis-bc84d4d8d3f9)
4.  [Pre-processing and Training Data Development](https://link.medium.com/i5yDUwZi9W)
5.  [Modeling](https://medium.com/@aiden.dataminer/the-data-science-method-dsm-modeling-56b4233cad1b)
6.  [Documentation](https://medium.com/@aiden.dataminer/the-data-science-method-dsm-documentation-c92c28bd45e6)

### An example guided case study

---
# Data Wrangling
## Missing Values
Learn advanced identification and imputation methods for missing values with this [Data Camp Course](https://www.datacamp.com/courses/dealing-with-missing-data-in-python/?tap_a=5644-dce66f&tap_s=644217-4bb8b9)

## Outliers
Another foundational issue in data cleaning is how to handle outliers. According to  [Wikipedia](https://en.wikipedia.org/wiki/Outlier "https://en.wikipedia.org/wiki/Outlier"):

> An outlier is an observation point that is distant from other observations.

Understanding what being "distant from other observations" means is easy if we think in a two-dimensional space. For example, if we had a dataset of the net worth of the 7 billion people on earth, then the net worth of the richest 1,000 people would be visible outliers as they are way higher than the rest.

In general, we get outliers in the data in 2 ways:

1.  An error in the data collection process may create outliers. Take, for example, a "Salary" column in an Excel workbook where the values are stored in thousands. If we mistakenly type 100,000 instead of 100, we created an outlier due to error. That is more broadly called "measurement error."
2.  Sometimes, the processes that generate the data produce extreme and rare values which can be regarded as true outliers. In this case, the abnormal data is not due to measurement error but to the extreme nature of the observation itself. These cases should be rare.

In this checkpoint, we'll cover:

-   Why we "don't like" outliers
-   How to detect outliers
-   How to treat outliers

Before proceeding further, let's highlight that outliers are defined for continuous variables and not for categorical ones. All discussion in this checkpoint, then, applies only to continuous variables.

### Do we really "not like" outliers?

Outliers can contain valuable information and should not be discarded without close consideration of what is causing them. However, for data science models and applications, we often "don't like" outliers because:

-   They skew the descriptive statistics of the data. For example, consider one of the most commonly used descriptive statistics—the mean. This value can be severely skewed by outliers.
    
-   Some machine learning models are sensitive to extreme values. In order to get more accurate estimates, we need to eliminate those values from our dataset.

To see the effects of outliers, watch the gif below and see how an outlier influences the relationship between the data points (The orange line represents the relationship between the data points):

That being said, some tasks in data science are  _all about_  the outliers. For example, in anomaly detection the main goal is to identify anomalies—which are often outliers themselves! This area of data science, however, is outside the scope of this course.

### Outlier detection

Detecting outliers, of course, is the first step to understanding how to handle them. But, just as with many of our previous tasks, there is no absolute to define what constitutes an outlier. When we talk about outliers, we should make sure that they are  **rare**  and have  **extreme**  values. Defining just  _how_  rare and  _how_  extreme they are is a judgment call that depends on the task at hand. In light of that, there are some commonly used thresholds for defining outliers.

Usually, we will use standard deviation to define the outliers. Values that reside outside the range of  **(mean - T_standard deviation, mean + T_standard deviation)**  are considered outliers. Here  **T** stands for threshold. Depending on the case, it's common to set the threshold to 1.5, 2, 3, or 5. But, as mentioned earlier, the exact threshold value varies depending on the project in question.

There are two main methods of outlier detection:

1.  Visualize the variables using boxplots and histograms.
2.  Use statistical techniques such as Z-scores, Tukey's method

### How to treat outliers

We've detected the outliers—now what? We need to do something with them so that they do not affect the reliability of our analysis. Broadly speaking, there are 3 approaches we can take in handling outliers:

  

1. We can **drop the outliers** from our dataset.

  

2. We can **cap the values of the outliers** by assigning them new values.

  

3. We can **transform** the outliers into something harmless for our analysis.

  

Let's go over each approach in turn.

  

### Dropping outliers from the dataset

  

Dropping the observations with extreme values is probably the easiest way of handling outliers. But, consider our discussion from the previous checkpoint about dropping missing values. By excluding any observations from the dataset, we effectively lose information. This the same case for dropping outliers, especially in small datasets. However, some situations may justify dropping the outliers from the dataset:
* If we know that the outliers stem from measurement error or a problem in the data collection process, we should drop them.
* If dropping the outliers doesn't make any meaningful change in the following phases of analysis, we can drop them. However, we need to replicate our analysis both with the outliers and without them to confirm this.
* If dropping the outliers makes a meaningful change in the following phases, but we can't find a proper way of handling them otherwise, we can drop them from our dataset.

### Limiting the values of the outliers

The main problem with the outliers stems from their extreme magnitudes. If we can cap the values of the outliers, their effects on our analysis would be limited. One common way of limiting the outlier values is called **winsorization**. Winsorization can be applied in *one-way* or *two-way* techniques. In one-way winsorization, we either limit the lowest end of the value distribution or the highest end. In two-way winsorization, we set limits on both the lowest end and the highest end.

The idea in winsorization is to set the values of the extreme points to the value of a specified percentile. For example, we may set the values of the highest end of the distribution to the value of the 95th percentile. Similarly, we can set the values of the lowest end to the value of the 5th percentile.

We can winsorize a variable using SciPy's `winsorize()` method. We give a tuple of values as a parameter to this method where the 1st element of the tuple is the lowest percentile and the 2nd element is the highest percentile in the two-way winsorization. If we want to apply one-way percentile, we can set the corresponding element in this tuple to zero (0).


---
# EDA
## Math and Stats

-   [Khan Academy Introduction to Matrices](https://www.khanacademy.org/math/precalculus/precalc-matrices)  
-   [Khan Academy Linear Algebra](https://www.khanacademy.org/math/linear-algebra)  
-   [Khan Academy Multivariable Calculus](https://www.khanacademy.org/math/multivariable-calculus)  
-   [Khan Academy Statistics and Probability](https://www.khanacademy.org/math/statistics-probability)  
-   [3blue1brown YouTube Channel](https://www.youtube.com/channel/UCYO_jab_esuFRV4b17AJtAw) 
-   [Math for Machine Learning on Coursera](https://bit.ly/courseraMathForML) 

[Statistical Thinking in Python part 1](https://www.datacamp.com/courses/statistical-thinking-in-python-part-1/?tap_a=5644-dce66f&tap_s=644217-4bb8b9)

[Statistical Thinking in Python part 2](https://www.datacamp.com/courses/statistical-thinking-in-python-part-2/?tap_a=5644-dce66f&tap_s=644217-4bb8b9)

---

### [Feature Selection & Dimension Reduction ](https://hub.packtpub.com/4-ways-implement-feature-selection-python-machine-learning/)

### [Automated Feature Engineering](https://github.com/Featuretools/predict-customer-churn/blob/master/churn/3.%20Feature%20Engineering.ipynb)


---
# Modeling Methods
As you may be aware there are countless types of machine learning model types and more variations are being added al time.  To be succesful as a data science professional you need to first learn the most broadly appropriate and applied methods and later you can delve into more specific solutions.

## Supervised Learning
[Classification, kNN, Cross-validation, Dimensionality Reduction](https://matterhorn.dce.harvard.edu/engage/player/watch.html?id=c322c0d5-9cf9-4deb-b59f-d6741064ba8a)

[This useful resource offers great advice about when different classification methods ought to be used.](http://blog.echen.me/2011/04/27/choosing-a-machine-learning-classifier/)

The modeling methods listed below are covered in detail [in this playlist.](https://www.r-bloggers.com/in-depth-introduction-to-machine-learning-in-15-hours-of-expert-videos/) The lectures are solid and the text they reference is excellent as well. Don't be detered byy the code examples being in R, there are plenty of Python coding examples out there, the main point is to gain the statistical concepts and insights.

Linear Regression

Lasso Regression

Decision Trees

Random Forest 

SVM

KNN

## Unsupervised Learning

K means clustering

PCA


##  [Which machine learning model should you try first?](https://medium.com/@aiden.dataminer/which-machine-learning-model-should-you-try-first-e35579f15924)

Determining when to use what type of model can be a daunting task for an aspiring or early career data scientist. Although this can be a data driven decision it is often a practical balance between statistically appropriate and business acceptance and comfort.

Recently, I received an email from an aspiring data scientist asking a common question in data science.  _How do I know when to use which model?_  The data scientist that sent the question provided more context and had a good approach in mind, but I’d like to answer this question for everyone just starting out in data science.

> How do I know when to use which machine learning model?

This is one of those it depends on everything questions; but here is my approach strongly rooted in the elegance of simplicity.

> _“Make everything as simple as possible but not simpler.” — Albert Einstein_

### **Diagram of the first model selection**

![](https://miro.medium.com/max/3300/1*WBaYR8qUT1K53h87PmJppw.png)

### **Why Random Forest, Logistic, Lasso and Linear Regression?**

Starting with the Multi-Class response variable, Random Forest is well suited to highly correlated features and easy to interpret and understand. In addition, the easy extraction of relative feature importances provides the user a preliminary view of features with strong predictive power for the response variable. Logistic regression is even easier to understand and highly efficient in terms of model run time and provides the simplest approach when model performance is good for the classification in hand. Although multi-class logistic regression is feasible, implementing Random Forest in a multi-class situation is more commonly accepted.

Now, looking at the numeric response side starting with multiple linear regression as the simplest option, however, it is likely to suffer from over-fitting, thus we introduce Lasso regression. Lasso regression through L1-regularization is able to ‘automatically’ complete feature selection for the user by pushing all unimportant feature coefficients to zero. Finally, if the data has many (more than 20) features and some of them are correlated with each other, applying a random forest regression is an easy to understand modeling method usual performing well in non-ideal situations, such as the assumptions for linear regression being unmet.

### Design Your Own Decision Framework

You can design your own decision framework based on the algorithms you prefer and your project constraints following these questions:

1.  Is your response variable numeric or categorical?
2.  How many features are in the data?
3.  Do the features have a high likelihood of collinearity?
4.  What is the importance of interpretability to the model outcome?
5.  What will be the application of the model?

### Be Decisive, Not Exhaustive

No matter which model you start with the idea is to balance the constraints of efficiency in implementation, level of understanding required, and overall model performance. It is a best practice to test a couple algorithms and compare their performances, and by a couple I mean two to three with a max of five. You should compare models that leverage different aspects of the features and modeling performance. Don’t compare a decision tree model to a random forest model and expect vastly different results. Hyperparameter tuning is great, but it is also time-consuming and often only yields slight increases in model performance metrics.

### Move on to More Feature Engineering

Feature engineering is more likely to improve model performance than hyperparameter tuning, so consider where your time is best spent and develop more features if your models aren’t performing as you would like.


## Model Evaluation

# Practical Application
### If you want some help getting setup in [Python and Jupyter Notebooks](https://aidenvjohnson.com/wp-content/uploads/2020/05/Intro_python-1.html)

- [ ] Dash Boards (Dask, plotly)

## Big Data - Spark
Businesses rely on numbers to guide decision making and to exploit their competitive advantages whenever possible.

As a result, companies have always leveraged state of the art computing technology to understand as much data as possible. Even though it’s a relatively new term, “big data” simply refers to a desire to glean relevant information from the most data. 

The sheer amount of data available is staggering, as data generation exponentially expands. In 2013, Science Daily [reported](https://www.sciencedaily.com/releases/2013/05/130522085217.htm) that 90% of all data ever created in history has been generated in the last two years; IBM followed up a year later with a reminder that each year we generate 10 times more data than the prior year. Today, IBM reports that 2.5 quintillion (2.5 x 1018) bytes of data are generated each day. As more devices - particularly internet-of-things devices — come online, and more and more people gain internet access, the data generated daily will only increase.
For a data scientist, the availability of big data is both enticing and daunting. To better comprehend big data, most companies will describe it in the context of the “3 Vs”: volume, velocity, and variety:

* **Volume:** Data comes from a variety of sources, including social media, transaction data, internet-of-things data, and sensor data. Storing this data used to be challenging — even prohibitive — but the availability of distributed storage systems such as Hadoop has reduced this barrier and allowed more data to be stored for longer periods of time.

* **Velocity:** Data often streams into the system at a very high rate, especially when considering point-of-sale transaction data, social media content, and sensor data. Effective utilization of the data requires that it be processed and acted upon in a timely fashion.

* **Variety:** Today, data scientists utilize more unique data types and formats than ever. These include structured data in databases, unstructured text, streaming sensor data, images, audio, stock ticker data, and many others. Big data tools allow data scientists to use varied formats together and identify common signal and information.
 

## Why does big data matter?

  

Data is only valuable insofar as you extract insight from it, and the big data side of data science is about bringing your data science skill set to bear on extracting actionable insights from these myriad data sources. Big data can be analyzed to uncover ways to reduce costs and time, improve product design, make smarter decisions, and answer all sorts of questions. It's behind many state-of-the-art business techniques including:

  

* cybersecurity

* predicting tool or device failure before it happens

* optimizing delivery routes

* providing personalized offers or recommendations

* real-time language translation


## Big Data with Spark

Adding big data to your toolkit means that you go from working on a dataset hosted on a single system to working with distributed datasets. The best means to work with distributed, massive datasets is within a distributed computing framework. Distributed computing brings significant challenges — How do you synchronize the code across many processors? What happens if a single processor fails? How do you roll up results when execution concludes?

Apache Spark aims to solve many of these challenges. Spark simplifies the tasks that bedevil developers when working on distributed computing including resource scheduling, job execution, communication between nodes, and so on. Spark was developed from the beginning to work with machine learning algorithms, which means it has been optimized for high-performance in situations where data is accessed multiple times over many iterations.

Spark is the leading open source distributed analytics platform. Its [project page](https://spark.apache.org/powered-by.html) lists almost 100 companies using Spark in production, and there are almost 400 active developers contributing to the codebase on GitHub.

Spark can run in standalone local mode with all processes inside a single Java Virtual Machine, or in standalone cluster mode. Data scientists interact with Spark via APIs in several languages. Spark supports 4 programming languages: Java, Scala, Python, and R. We’ll use Python in our examples for this course.

Spark uses a data representation called the Resilient Distributed Dataset (RDD). This is a data type very similar to the dataframe you know from Pandas but optimized to be distributed across multiple computers, residing in memory across all of them. Once an RDD has been created, by using Spark methods and functions, you interact with this distributed dataset as if it existed only on a single device. As an end developer, you don’t know — or need to know — how the RDD is actually allocated. Spark frees you from those details and allows you to focus on what is important to you — analyzing a dataset.
#### Deep Learning - when is it needed or benefit/cost comparison











<!--stackedit_data:
eyJoaXN0b3J5IjpbMTMzNzg5NDIzNSwtMTE4ODg1MzcxMCwtMz
k2OTM5MDExLC0xMjcxMjg0MDgxLDU5NTA1Njg4NiwzMTgyNjA3
MTUsOTM4OTc2MTUxLC0xMjIyODY4MDA0LC05MTA2NzcyMjIsNz
I5MjMxNzExLDIxMTY0MzU0MTMsLTEyOTQwNzk1MDAsLTQyNTEx
MjY5MSwxOTQwOTYzMTYxLC0xNzM3MjM2NTE5XX0=
-->