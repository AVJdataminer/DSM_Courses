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
#### Missing Values

#### Outliers
---
# EDA
#### Stats Review/distributions
---

### Feature Selection & Feature Eng
#### Dimension Reduction

### Data Preprocessing for Modeling
---
# Modeling Methods

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


#### Supervised
#### Unsupervised
#### Special topics
- Recommender Systems
	- Types and use cases
- Time Series & forecasting

## Model Evaluation

# Practical Application
#### Python, Jupyter and Colab

#### Dash Boards (Dask, plotly)

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
eyJoaXN0b3J5IjpbLTExNDE4NTQ3MjgsLTEyOTQwNzk1MDAsLT
QyNTExMjY5MSwxOTQwOTYzMTYxLC0xNzM3MjM2NTE5XX0=
-->