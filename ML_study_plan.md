# Data Science Study Plan 
  

## Study Plan Introduction 
This study guide is designed to help you efficiently and effectively acquire the knowledge and skills you need to break into the field of data science. Whether you are software engineer or a program manager this guide will put you on the proven path of foundational knowledge to get started in a career in data science. Shorter topics will be covered in detail and more advanced topics will leverage several online resources to provide a more in-depth look. It is easy to get excited by the latest development in computer vision or a new machine learning model such as the Facebook Prophet model, however, before you can get hired and use these tools in your daily work you need to develop the foundational knowledge in the field of data science. It is the foundational algorithms like Logistic Regression and Random Forest as well as a solid project process that hiring managers are looking for in filling data science roles.

## Introduction to Data Science
If you have been on your data science learning journey for a bit then you may be familiar with the content here and probably want to skip ahead to the next section.

Data science is the integration of is the integration of Statistics, Machine Learning, and Deep Learning with a bit of business analyst and management methods thrown in.

 - [ ] Add image of how AI, ML, etc fit together.

### Data Science Life Cycle
The work of a data scientist is often changing based on the business needs or the phase of the project they are working in. Most large well developed data science teams in organizations have established processes for the develpment and execution of data driven projects. However. less centralized teams and individual contributors still need a process to manage all the steps in a data science project. In the next section you begin to learn how to implement a data project in a business context that will yield meaningful and reliable results.

## The Data Science Method
To be successful, you must have all the prerequisite core knowledge of machine learning algorithms, programming abilities, and also be passionate about becoming a professional data scientist. The biggest difference between people that are successful in data science roles and those that are not is their ability to effectively frame data science projects and communicate project outcomes. Sometimes, this is referred to as data storytelling, however, that only describes part of the process involved in sharing your findings and results. You need to work to develop the entire framework for the narrative of your data science project to communicate the project as a story.

The Data Science Method (DSM) serves to identify the context of your data science story. Starting with the end in mind is one way to glean some guidance — you must know where you are headed in order to take the appropriate steps along the way. This can be difficult depending on the complexity of your data and the business needs being requested for the project. Let’s consider the [scientific method](https://www.khanacademy.org/science/high-school-biology/hs-biology-foundations/hs-biology-and-the-scientific-method/a/the-science-of-biology) as a framework, as it provides clear steps that are taken along an experimental path.

Based on the scientific method, I have developed the Data Science Method (DSM) as a way to improve data science project outcomes and take your work to the next level. The DSM is detailed below.

----------

**The Data Science Method**

1.  Problem Identification
2.  Data Wrangling
3.  Exploratory Data Analysis
4.  Pre-processing and Training Data Development
5.  Modeling
6.  Documentation

The DSM steps can be applied to nearly every data science or machine learning project, as it serves as a guide map for what actions you need to take. The benefits of following this approach include, but are not limited to: reducing the likelihood of needing to backtrack in your work to solve a data problem, identifying key data issues early, gauging expectations of the project outcomes appropriately, forcing yourself as the data science professional to be very clear about the goal of the project and how the data does or does not support that goal. The DSM steps and other frameworks have been developed by seasoned professionals because they have extensive experience managing projects that forced them to acknowledge when they overlooked a crucial consideration earlier in the analysis. The DSM is most helpful for aspiring data scientists because it allows you to leverage the experience of professionals that came before you.

Structured thinking is a common and well-articulated tool used in all types of industries. Thus, the DSM supports an organized approach to solving a business problem with data, and it also supports the essential communication component of articulating project outcomes to your client. As you work through the five steps of the DSM, you will build a deeper understanding of your data, the problem, and how the data can be leveraged to meet your client’s expectations and solve the problem.


The next few sections describe each step of the DSM with concrete examples of the methods for clear understanding of the steps. The methods covered are not exhaustive, but merely a starting place. Later sections in this book cover additional methods, such as data imputation for missing values under data wrangling.
 ---

### DSM - Problem Identification
Problem identification is the very first, essential step to a well-positioned data science project.

Start by identifying the goal of the data science project. Ask the question: Is this an exploratory project or a predictive modeling project? If the answer is exploratory, then less planning may be needed at the outset to ensure interesting and meaningful outcomes. You might have questions about how you can tell if a project is exploratory or predictive,  so let’s work through some examples. You may be given a data set for a project and asked questions such as:

-   Process the data — what are the important findings you can glean?
-   What can you tell me about sales in the last year?
-   What type of customers do we have?

All of the above three questions indicate that you are working on an exploratory data project — you’re not explicitly predicting any response variable to apply to a future dataset. For the first question, you have the potential to spend countless days looking at the data a thousand different ways. In order to apply some necessary bounds to the analysis, you can reframe the open-ended question into a few more specific questions that are actionable using  [SMART principles](https://player.vimeo.com/video/350841599?autoplay=1&loop=0&autopause=0). The other two questions are equally difficult to answer without following structured thinking and framing the context, criteria for success, and stakeholders. It helps to identify what the expected use of the final product is. For an exploratory project, try to hypothesize the kind of findings that are of value  _before_  you get started. Let’s work on rephrasing the three questions above to be actionable.

Original question: Process the data and tell us what important findings you can glean.

Revised question: What are the summary statistics of this data set and what do we know about the context of the data that we can investigate further for business impact?

Original question: What can you tell me about sales in the last year?

Revised question: What is the most common product we sell, and how much did we sell every quarter over the last year?

Original question: What type of customers do we have?

Revised question: What are the average ages, incomes, and home locations of our customers?

As you look at the differences between the original question and the revised question, you can hopefully see that the revised questions are now problem statements that you can use data science analysis to answer. Developing revised questions might take some effort on your part — you might need to return to the stakeholders for feedback before fully identifying the problem and the core focus of the analysis. Be sure to ask yourself if the data you have access to supports the question you’re trying to answer. If it doesn’t, ask!!

If your goal is to evaluate the variable correlations and multi-dimensional interactions of the data set, then the initial motivations of the data science project must be more firmly defined.

Outlined below is a step-by-step approach to Problem Identification, the first step in the DSM. Defining each one of these bullets at the project outset will guide your project to a fruitful outcome.

**Problem Identification Steps:**

1.  Problem statement formation
2.  Context
3.  Criteria for success
4.  Scope of solution space
5.  Constraints
6.  Stakeholders
7.  Data sources

Here is a list of general questions to help you get started in defining the above-listed steps for problem identification.

-   Is the goal of this project exploratory or predictive?
-   Identify what the completed model will be used for and/or the expected outcome of the exploratory work — consider supervised or unsupervised methods.
-   Does the data you have access to answer #2 above, or do you need more or different data?
-   What is the data timeline and/or temporal scale of interest?
-   What is the modeling response variable? How is it described and defined?
-   Is this a classification or regression problem?
-   What deliverables will be provided after this modeling project?

As you develop answers to these questions and the steps outlined in problem identification, you will not only gain a focused trajectory of work, but you also will get at the key details needed for model documentation. Further, you will connect your data analysis to a business need, which may have motivated the work in the first place. If you clearly define your data science work, you will have a framework for successful implementation that works within any industry.

#### Problem Identification Example 
 1. Define the question specific to modeling activities
e.g. Predict device failures

2. Identify the data needed and or available:
e.g. Daily aggregated telemetry device failure data

3.  Define the data Timeframe:
e.g. 01/01/2015–11/02/2015

4. Describe the Modeling Response:
e.g. Binary, 0 or 1, non-failure = 0, failure = 1

5. Unsupervised or Supervised Classification or Regression Model:
e.g. Supervised Classification

6. Identify What Deliverables will be generated:
e.g. PDF outlining modeling process from data exploration to best model results.


### DSM - Data Wrangling
**Data Wrangling Steps:**

Data wrangling consists of four high-level steps that should be applied in any data science project.

1.  **Data Collection**
2.  **Data Organization**
3.  **Data Definition**
4.  **Data Cleaning**

**DATA COLLECTION**

Data Collection can vary depending on the scope of the project and the data available. Assuming we have completed Problem Identification, Step 1 in the DSM, then ask yourself if the data you have can answer the question of interest. In some cases, writing website scrapers, scouring for census data and search through other web sites for available data can be a time-consuming but necessary task. Perhaps you have data provided by your client, in that case, you may receive access to an S3 bucket or a SQL database each with many tables or files of data or you could be given a single CSV file. Regardless of the situation, you will likely need to spend some time locating your data.

Once you have procured the datasets you need you’ll want to load them into a friendly format such as a data frame. Additionally, collating all your data sources into a single data frame for analysis will make your project much easier going forward. Depending on the relationship of your data pieces and how they tie together you may need to apply some methods from step 4. Data Cleaning, before you’re ready to concatenate the pieces together into a single data frame.

Collating your data sources at this early point in the workflow allows for clean data processing and easy adjustments in methods at later stages in the work.

----------

**DATA ORGANIZATION - DIRECTORY STRUCTURE**

Directory organization is one of those things that you may not think of much when you’re just starting out in data science but as you get into multiple iterations of the same model having a well-structured environment for your model outputs and potentially intermediate steps and data visualizations is paramount. Containerized approaches may reduce the need for this and highly structured work environments also don’t require an additional organizational directory. The key is to keep things organized, clean, and dated and/or versioned.

![](https://miro.medium.com/max/30/1*h-meTEPnSsoGwc-Hhz6a7A.png?q=20)

![](https://miro.medium.com/max/317/1*h-meTEPnSsoGwc-Hhz6a7A.png)

Here is an example of a simple modeling directory.

It’s clearly lacking creativity with the higher folder names, but what it lacks in creativity it gains in simplicity. The date and time stamps help to provide a simple way to identify previous model iterations. Adding a more descriptive name to each modeling folder is good to such as; RandomForest_500, or RCN_3layers.

As you start to develop more advanced methods you may need a more complex structure. Another common method for project organization in Python is by using the  [cookiecutter python package](https://drivendata.github.io/cookiecutter-data-science/)  to generate the file structure for a new project. Below is what the structure looks like.

![](https://miro.medium.com/max/27/1*MpwB4_5jl9lsrYhgBjMF2g.png?q=20)

![](https://miro.medium.com/max/883/1*MpwB4_5jl9lsrYhgBjMF2g.png)

[https://drivendata.github.io/cookiecutter-data-science/](https://drivendata.github.io/cookiecutter-data-science/)

If you come from a computer science background you may already be familiar with the concept of version control, Git, and Github. Learning how to effectively use Git and repositories is a core skill for all data scientists. More junior data scientists should spend some time reviewing the concepts of version control and expect any established data science team they join to be using it daily.

----------

**DATA DEFINITION**

Data definitions are often a  neglected  piece of a data science project. Sometimes this is considered a model documentation component, however, it is both a documentation as well as a development piece. The process of developing data definitions prior to model development informs the data science practitioner at a glance about their development dataset. The data scientist can quickly review the data dictionary as necessary during the modeling process to refresh their understanding of specific components. The other benefit is in communication with the client during the review of intermediate steps or model reviews. When the data definitions are clear and in writing everyone in the exchange is on the same page about what the data features represent.

The data definition should contain the following items by column:

1.  Column Name
2.  Data Type (numeric, categorical, timestamp, etc)
3.  Description of Column
4.  Count or percent per unique values or codes (including NA)
5.  The range of values or codes

One example of data definitions is what  [kaggle](https://www.kaggle.com/spscientist/students-performance-in-exams)  has on their datasets pages about each downloadable dataset. Below is the header for the table on student’s exam performance with some important data descriptors identified.

![](https://miro.medium.com/max/30/1*j1fHigZCVVQqihY66uU1Qw.png?q=20)

![](https://miro.medium.com/max/761/1*j1fHigZCVVQqihY66uU1Qw.png)

Example of data definition — from kaggle.com

Here is another example where the variable called ‘NETW30’ is described in detail in the sentence above the table. The table defines each column by the unique codes found in that column, the particular description each code represents as well as the count and percent of each unique code in the column. Based on the description we can infer this is a categorical data column that represents the results of a prior statistical model which may have multiplicative error considerations which are good to be aware of.

![](https://miro.medium.com/max/30/1*CGbxsV-J7pmOGOv5BMACmQ.png?q=20)

![](https://miro.medium.com/max/959/1*CGbxsV-J7pmOGOv5BMACmQ.png)

An example data definition table for one column called NETW30.

----------

**DATA CLEANING**

Data Cleaning can be a time-consuming process and can have serious implications for spurious results if not done properly before beginning the modeling project.

The most common types of data cleaning steps are:

1.  Handling missing, null,  and NA data
2.  Removing duplicates

As we mentioned in step 1 perhaps you need to combine two data frames from different sources into a single data frame. This requires unifying the formatting and filling in gaps of overlap with NA or other thoughtful fillers such as 0 or 1 when applicable.

The first step in this process is to identify how many NA values are in your data set. This can be done by printing out the ``df.info()`  to get the data type for each column. One may also want to run additional analyses to ensure there are no mask values such as '-9999' or values such as 'none', these missing values will be missed by ``is.null()`, this scenario can be identified by running ``value_counts()`  for each column in your data frame. Once we determine the different missing or NA values in the data we need to handle them appropriately. Reviewing the percentage of missing observations aids in determining the best step forward.

Follow these steps:

1.  Review the percentage of observations missing per column
2.  Drop, Impute, or Replace missing values

If less than one percent of the data column is missing then it can be dropped. For percentages larger than one percent each column would need to be reviewed in detail to determine the appropriate handling method. The main consideration is how impactful will the NA approach be on the overall distribution of the data. Dropping the entire row with a missing value rather than simply a missing observation is the best way to fairly drop NA values from a data frame.

_Drop duplicate rows and columns_

Next, we need to check for duplicate rows and columns. Duplicate rows could be legitimate values depending on your data and how it was collected or the magnitude of variation that is expected in your data. The only time you should delete duplicate rows is if you are confident they are repeated measures of the same observation and that it has negative consequences for your expected statistical modeling method. Your prior work on data definitions will inform you of any duplicate columns. Duplicate columns are common when multiple data sources are combined to create the model development dataset. These may not have the same column name, but if the columns’ rows are identical to another column, one of them should be removed.

### DSM - Exploratory Data Analysis (EDA)

Step number three in the Data Science Method (DSM) assumes that both steps  [one](https://medium.com/datadriveninvestor/the-data-science-method-dsm-a-framework-on-how-to-take-your-data-science-projects-to-the-next-91f9fd81e5d1)  and  [two](https://medium.com/@aiden.dataminer/the-data-science-method-dsm-data-collection-organization-and-definitions-d19b6ff141c4)  have already been completed. At this point in your data science project, you have a well-structured and defined hypothesis or problem description. The model development data set is up and ready to be explored, and your early data cleaning steps are already completed. At a minimum, you have one column per variable and have a clear understanding of your response variable.

Based on step two in the DSM you have already reviewed the following items about each variable in your data:

1.  Column Name
2.  Data Type (numeric, categorical, timestamp, etc)
3.  Description of Column
4.  Count or percent per unique values or codes (including NA)
5.  The range of values or codes

There are many sub-steps in a proper exploratory data analysis (EDA) workflow. Depending on your familiarity with your data and the complexity of the data and the problem you are solving the scale of the EDA necessary may change. Generally, the exploratory analysis workflow can be broken down into four critical steps:

1.  **Build data profile tables and plots**
2.  **Explore data relationships**
3.  **Identification and creation of features**

----------

1. DATA PROFILES — PLOTS AND TABLES

_Reviewing summary statistics_

Summary statistics can be evaluated via a summary statistics table and by checking the individual variable distribution plots. Both will indicate the spread of your data. Depending on the distribution, you may be able to infer the mean from distribution plots; however, the summary table is the best way to review this value. Compare the example summary statistics table and the histogram plots for reference.

#summary stats table transposed for df  
df.describe().T

![](https://miro.medium.com/max/60/1*qRoPSnAT1ZPJWfepHv-9Fw.png?q=20)

![](https://miro.medium.com/max/808/1*qRoPSnAT1ZPJWfepHv-9Fw.png)

Summary Statistics Table

#histograms for each variable in df  
hist = df.hist(bins=10,figsize =(10,10))

![](https://miro.medium.com/max/60/1*4jeeEvIoLOyTm27rM5PlMw.png?q=20)

![](https://miro.medium.com/max/994/1*4jeeEvIoLOyTm27rM5PlMw.png)

Histogram plots of each variable in the data frame

Categorical variables require a slightly different approach to review the overall number of each unique value per variable and compare them to each other. The example data we are using for these figures do not contain categorical variables; however, below is an example workflow for categorical variables:

#select categorical variables only  
df_cat = dataset.select_dtypes(include = 'object').copy()#get counts of each variable value  
df_cat.ColumnName.value_counts()#count plot for one variable  
sns.countplot(data = df_cat, x = 'ColumnName')

_Reviewing for Outliers and Anamolies_

Boxplots are a quick way to identify outliers or anomalous observations. Considering these values within the context of your data is important. There may be situations where the so-called outliers or extreme values are the observations of the most interest. For example, if we review the air quality dataset used in the example summary table and histograms we see that several observations beyond the upper whisker; however, these extreme values are observations where the concentration of the particle in question probably exceeds the healthy limit. Similarly, when we review the humidity data, we have a few data points falling outside the upper limit. We want to consider if those values are data collection errors (which is very likely for anything above 100%) and then remove those observations.

#create a boxplot for every column in df  
boxplot = df.boxplot(grid=False, vert=False,fontsize=15)

![](https://miro.medium.com/max/60/1*ROe1IE0TCSeBjCJI-aHcGw.png?q=20)

![](https://miro.medium.com/max/562/1*ROe1IE0TCSeBjCJI-aHcGw.png)

Boxplot of each variable in the data frame

----------

2. DATA RELATIONSHIPS

Investigating variable relationships through covariance matrices and other analysis methods is essential for not only evaluating the planned modeling strategy but also allows you to understand your data further. Below, we calculated the correlation coefficients for each variable in the data frame and then fed those correlations into a heatmap for ease of interpretation.

![](https://miro.medium.com/max/60/1*y14HU1jpCg-ZHkH1wVcj3A.png?q=20)

![](https://miro.medium.com/max/717/1*y14HU1jpCg-ZHkH1wVcj3A.png)

Pearson Correlation Heatmap

#create the correlation matrix heat map  
plt.figure(figsize=(14,12))  
sns.heatmap(df.corr(),linewidths=.1,cmap="YlGnBu", annot=True)  
plt.yticks(rotation=0);

A glance at the correlation heatmap (Figure X) shows how strongly correlated the different air pollution metrics are with each other, with values between 0.98 and 1. Logically, we know they will be highly correlated, and that is not of concern here. But, if we weren’t expecting that and we’re planning to treat them as independent variables in our modeling process, we would violate co-linearity rules and would need to consider using a modeling technique such as a Random Forest or a decision tree, which is not negatively impacted by high variable correlations.

_Pair plots_

Another way to evaluate the variable distributions against each other is with the  [seaborn pair](https://seaborn.pydata.org/generated/seaborn.pairplot.html)  plots function.

![](https://miro.medium.com/max/60/1*kMSVp41Rf5vuqgxoETbMVg.png?q=20)

![](https://miro.medium.com/max/743/1*kMSVp41Rf5vuqgxoETbMVg.png)

#pair plots  
g = sns.pairplot(df)

----------

3. IDENTIFYING AND CREATING FEATURES

Variables and features are almost synonymous. The primary difference tends to be the context in which they are used; in machine learning, it is common practice to identify predictive features in your data whereas in parametric statistics, features are often referred to as variables and variables can include the response variable which you predict with your model.

The goal of identifying features is to use your exploratory work to isolate features that will be most helpful in constructing a predictive model. In addition to recognizing those features, it often behooves one to create additional features for inclusion in your predictive modeling work.

Once you have identified the critical features for your model development, you may realize you need to create additional features to augment your original data. You can do this through the development of combining features or revaluing them to emphasize specific relationships. Additional features can also be created through Principal Components Analysis or Clustering.

Building a [Principle Components Analysis (PCA)](https://en.wikipedia.org/wiki/Principal_component_analysis)  is a useful way to apply a dimension reduction application to identify which features contain the most amount of variation within your development dataset. The predictive model can be constructed on the principal components themselves as features, resulting in feature reduction. Feature reduction is helpful when your data set has too many features to choose from, and you need a more automated way to reduce the number of input features for modeling. There are different flavors of dimension reduction methods based on multi-dimensional scaling, such as  [Principal Coordinate Analysis](https://en.wikipedia.org/wiki/Multidimensional_scaling#Types). Lasso regression is another tool for a semi-automated feature selection approach. Review these methods to determine the best strategy for your project.

Clustering (e.g. K-means clustering) is an excellent exploratory analysis method for creating additional features which in this case would be the clusters themselves. The clusters can be used in conjunction with additional features if you find them to be valid after review.

### DSM - Data Preprocessing
Pre-processing is the concept of standardizing your model development dataset. This is applied in situations where you have differences in the magnitude of numeric features and situations where you have categorical and continuous variables. This would also be the juncture where other numeric translation would be applied to meet some scientific assumptions about the feature, such as accounting for atmospheric attenuation in satellite imagery data.

Here are the general steps in pre-processing and training data development:

1.  **Create dummy or indicator features for categorical variables**
2.  **Standardize the magnitude of numeric features**
3.  **Split into testing and training datasets**

----------

1.  **Create dummy or indicator features for categorical variables**

Although some machine learning algorithms can interpret multi-level categorical variables, many machine learning models cannot handle categorical variables unless they are converted to dummy variables. I hate that term, ‘dummy variables’. Specifically, the variable is converted into a series of boolean variables for each level of a categorical feature. I first learned this concept as an indicator variable, as it indicates the presence or absence of something. For example, below we have the vehicle data set with three categorical columns; specifically, Manufacturer, Model, and vehicle type. We need to create an indicator column of each level of the manufacturer.

![](https://miro.medium.com/max/60/1*y2lFEEFFyp6cyTQaCyC8Bw.png?q=20)

![](https://miro.medium.com/max/390/1*y2lFEEFFyp6cyTQaCyC8Bw.png)

An original data frame with categorical features

First, we select all the columns that are categorical which are those with the data type = ‘object’, creating a data frame subset named ‘dfo’. Next, we concatenate the original data frame  `df`  while dropping those columns selected in the dfo,  `df.drop(dfo,axis=1)`, with the  `pandas.get_dummies(dfo)`  command, creating only indicator columns for the selected object data type columns and collating it with other numeric data frame columns.

![](https://miro.medium.com/max/60/1*BNIG77Kc6sg0y6OcSmI4Fw.png?q=20)

![](https://miro.medium.com/max/543/1*BNIG77Kc6sg0y6OcSmI4Fw.png)

Dummies now added to the data frame with column name such as ‘Manufacturer_’

We perform this conversion regardless of the type of machine learning model we plan on developing because it allows a standardized data set for model development and further data manipulation should our planned approach not provide excellent results in the first pass. Pre-processing is the concept of standardizing your model development dataset.

----------

**2. Standardize the magnitude of numeric features**

This is applied in situations where you have differences in the magnitude of numeric features. This would also be the juncture where other numeric translation would be applied to meet some scientific assumptions about the feature, such as accounting for atmospheric attenuation in satellite imagery data. However, you do not pass your dummy aka indicator features to the scaler; they do not need to be scaled as they as are boolean representations of categorical features.

> Many machine learning algorithms objective functions are based on the assumption that the variables have mean of zero and have variance in the same order of magnitude of one, think L1 and L2 regularization. If the development features are not standardized then the larger magnitude features may dominate the objective function and further may spuriously reduce the impact of other features in the model.

Here is an example, the below data is also from the automobile sales dataset. You can see from the distribution plots for each feature that they vary in magnitude.

![](https://miro.medium.com/max/60/1*viPzBC23avFeO3KVzjceBw.png?q=20)

![](https://miro.medium.com/max/1043/1*viPzBC23avFeO3KVzjceBw.png)

Numeric Features of differing magnitudes

When applying a scaler transformation we must save the scaler and apply the same transformation to the testing data subset. Therefore we apply it in two steps, first defining the scaler based on the mean and standard deviation of the training data and then applying that scaler to each the training and testing sets.

----------

**3. Split the data into training and testing subsets**

Implementing a data subset approach with a train and test split with a 70/30 or 80/20 split is the general rule for an effective holdout test data for model validation. Review the code snippets and the other considerations below on splitting the model development data set into training and testing subsets.

----------

**Other Considerations in training data development**

If you have time series data be sure to consider how to appropriately split your data into training and testing data for your optimal model outcome. Most likely you’re looking to forecast, and your testing subset should probably consist of the time most recent to the expected forecast or for the same period in a different year, or something logical for your particular data. An example of date specified splitting function is provided here:

Additionally, if your data needs to be stratified during the testing and training data split, such as in our example if we considered European carmakers to be different strata then American carmakers we would have included the argument  `stratify=country`  in the train_test_split command.

### DSM - Modeling
Early practitioners and those less familiar with data science often think data scientists spend their entire day training machine learning models and tuning those models. However, we know that effective data science is the process of converting business problems into thoughtfully designed data problems where thorough problem identification work and data understanding is achieved before any model development work takes place. Modeling is the step that allows leveraging your data to make predictive insights and usually provides the most value in a data science project.

Let’s review the primary steps applied in Modeling.

1.  Fit the model with the training data
2.  Review the model performances — Iterate over models and parameters
3.  Identify the final model

----------

#### Fit the model with the training data

In the previous DSM step, we discussed the importance of creating a training and testing split of your model development dataset. Additionally, you should have a clear understanding of what you’re hoping to predict. The data type of your response variable along with a strong understanding of the features will guide you in determining which type of model to fit.

If your response variable is continuous, e.g. temperature or sales price, a numeric value that has a distribution closer to Gaussian than Bernoulli, than you will apply a regression type of model; otherwise a supervised classification model should be used.

**Which type of model?**

Continuous (Numeric) Response → Regression Model

Categorical Response (Labeled data) → Supervised Classification Model

Start with the simplest model for ease of understanding and communication. then as you build two or three model types to compare add more complex modeling methods.

Continuous Response → Regression Model → Multiple Linear Regression

Categorical Response → Supervised Classification Model → Logistic Regression

Let’s get busy applying this model. Even if you’re using a more advanced machine learning algorithm such as a Random Forest start with the out of the box implementation. Don’t worry about model hyperparameter tuning just yet. The first iteration of fitting the model with training data would look like the code box below implementing the sklearn library to apply a random forest regression.

from sklearn.ensemble import RandomForestRegressorregressor = RandomForestRegressor(random_state=0, n_estimators=200)regressor.fit(X_train, y_train)regressor.score(X_test, y_test)

After fitting the model we score the model to review the performance as well as predict the holdout test set to review the blind model performance.

----------

#### Review the model performances — Iterate over models and parameters

The code box below demonstrates the step of creating predictions on the testing data set using the model you developed in the previous step.

  
y_pred = regressor.predict(X_test)from sklearn.metrics import mean_squared_errorfrom math import sqrtrmse = sqrt(mean_squared_error(y_test, y_pred))rmse

Now let’s say we review our model performance and it’s weak, we discuss model performance metrics later on in the third section of the article. We have identified the need to do some model hyperparameter tuning to improve our model predictions.

_Model Hyperparameter Tuning_

-   When → the simplest model wasn’t a good solution and this more complex model doesn't meet performance requirements,
-   Why → improve the model accuracy compared to the generic out of the box flavor,
-   How → Grid Search, Random Search or Bayesian Optimization.

Here is an example of performing a grid search optimization to identify the best settings for the hyperparameters in the Random Forest Regression model. Notice we first create a grid of values for each one of the hyperparameters to test.

from sklearn.ensemble import RandomForestRegressor  
from sklearn.model_selection import GridSearchCVparam_grid = {"n_estimators": [200, 500],  
 "max_depth": [3, None],  
 "max_features": [1, 3, 5, 10],  
 "min_samples_split": [2, 5, 10],  
 "min_samples_leaf": [1, 3, 10],  
 "bootstrap": [True, False]}model = RandomForestRegressor(random_state=0)grid = GridSearchCV(estimator=model, param_grid=param_grid, n_jobs=-1)grid.fit(X_train, y_train)print(grid.best_score_)print(grid.best_params_)

Running this hyperparameter optimization will take some time to run compared to the plain out of the box application. However, you’re likely going to improve the model performance such that the added compute time will be worth the result.

#### Identify the final model

Model performance metrics are again dependent on whether you’re working in a regression universe or a supervised classification universe. Here is a list of commonly used model performance metrics for your reference.

![](https://miro.medium.com/max/60/1*tZxa-pG48yAHfgiIbH_3lQ.png?q=20)

![](https://miro.medium.com/max/552/1*tZxa-pG48yAHfgiIbH_3lQ.png)

List of typical model metrics

Which model performance metric to use may be a decision to be made in the project identification step. Defining the criteria for success of your model as a Mean Absolute Error ≤40 is a clear criterion for determining model success and completion. Based on the table below we would choose the Random Forest Regression model as the ‘Final Model’. The mean absolute error is less than the simple regression model and within our criteria for success.

![](https://miro.medium.com/max/60/1*uktSI2lFUN344fGrVG7miQ.png?q=20)

![](https://miro.medium.com/max/440/1*uktSI2lFUN344fGrVG7miQ.png)

Compare two model performances

**When choosing a final model also consider how often this model will need to be re-run and the processing time increase versus model performance increase. Additional considerations include interpretability and the associated buy-in by the stakeholders.**

### DSM - Documentation
- [ ] Add introduction or overview  to this step
####  Reviewing Results

y_pred = model.predict(x_test)  
print(explained_variance_score(y_test, y_pred))  
0.92

When reviewing your data science project results you are first looking at how the predictive model performed from a mathematical standpoint, but also from the business insights perspective. For example, if we want to guide the management on how to price a product, we can build a model on comparable products and predict the new product price based on our model. The predicted result is the ‘expected price’ for the new product. In the code block above we built a model with an R-squared value of 92%, which provides evidence that the model is predicting well on our test hold out data set. Given the model is performing well we can now use the same model to predict our new product with the same features associated with it as those used in the model training.

predicted_price = model.predict(new_product)  
print ("The expected price is $%s " % ')  
The expected price is $88.72

Similarly, if we are looking to forecast maintenance in order to prevent manufacturing downtime we have to start with reviewing sensor data for anomalies in the equipment. An anomaly is an event of the sensor failing over some time horizon. This is considered an anomaly because the majority of the time-series sensor data show reasonable values, and it is not until the sensor fails that maintenance event is indicated. Often the sensor will return zero when everything is running smoothly.

![](https://miro.medium.com/max/60/1*f5ydhOk9e8-Rhg31pu9uhQ.png?q=20)

![](https://miro.medium.com/max/502/1*f5ydhOk9e8-Rhg31pu9uhQ.png)

Sensor data stream where anything other than zero indicates a failure

In this sensor example, we have eight failure events at the beginning of our time-series, which from a manufacturing perspective could cause a big disruption and it would be ideal if those failures could be forecast and preventive maintenance be applied before that event occurs to avoid manufacturing downtime. Therefore our data science modeling should be oriented toward effectively forecasting the failure events across the temporal dimension. This is different than building a model to effectively predict failures from non-failures, where the separation between the training and testing data set could be random.

When reviewing the results consider the key factors you identified in the problem identification step and develop data visualizations to communicate the relationship between the key factors and your predicted outcome from the lens of the business problem and recommended action.

#### Presenting and sharing your findings (data storytelling)

This is the most important part of your entire data science project. Doing diligent and thoughtful model development only matters if your models get used. Unfortunately, it is all too common for a data science project to never get put into action, even after weeks of work. Your goal should be to convert your audience into believers of a better future given your recommendation is implemented. This starts by stating the current state of reality per the problem identification step. Once you establish the current state, guide your audience to the future state of rainbows and butterflies, or higher revenues and lower costs. This concept was identified by  [Nancy Duarte](https://www.ted.com/speakers/nancy_duarte)  as the secret structure of great talks. Nancy is an expert in presentation design and I highly recommend you watch her Ted talk. One of the most effective ways to communicate a future the audience is interested in is by tailoring the presentation to their perspective. This brings us to our first step in developing a persuasive data story; identify your audience and adapt your presentation in style and form. This might result in changing the medium you use to communicate, from Jupyter Notebook to Slidedecks. So let’s review the key components:

-   identify the audience and adapt to the appropriate level of detail
-   build a narrative around the status quo versus the fabulous future
-   communicate your recommendations as established by your data science project.

For more in-depth information check out the  [HBR Guide to Persuasive Presentations](https://amzn.to/2REbs5l).

----------

#### Finalizing code

The primary purpose of the finalizing code step is to ensure that the reuse of your code by you or others is not burdensome. In most developed data science teams you will work in a version control environment such as Git where your code is merged into branches alongside other data scientists and engineers. This is a great place for the team to share code as commonly used scripts or utilities can be shared readily by the team. However, even if you are working independently it is good practice to save your code using Git and to create flexible functions and scripts that can be written once and used again and again throughout your work. Make sure to provide some documentation or comments within each function or script describing the dependencies, inputs, outputs, and possible todos. Adding a short description or a detailed name to a Jupyter notebook can help leverage it later for a different project or to share it with a colleague and please clean up any extraneous or non-functioning code.

Finalizing your modeling code may also involve moving the model to production or serializing the model for later access. Putting your model in production varies substantially depending on your organization’s infrastructure and you will want to communicate with the data engineers and solutions architects about what additional scripts they may need to get the model production-ready.

----------

### Finalize model documentation

This is the time and place to corral the data science modeling project into a succinct document that gives the details of what you built and how well it performed.

Create a document called the Model Report. Here is the general layout to give you an idea of where start.

#### Minimum Model Documentation Example 
 1. Define the question specific to modeling activities
	- e.g. Predict device failures

2. Identify the data needed and or available:
 
	 - e.g. Daily aggregated telemetry device failure data

3.  Define the data Timeframe:
	- e.g. 01/01/2015–11/02/2015

4. Describe the Modeling Response:
	- e.g. Binary, 0 or 1, non-failure = 0, failure = 1

5. Unsupervised or Supervised Classification or Regression Model:
	- e.g. Supervised Classification

6. Identify What Deliverables will be generated:
	- e.g. PDF outlining modeling process from data exploration to best model results.
7. Data Preprocessing steps of note
	-   e.g. dropped duplicate rows
	-   e.g. created PCA for dimension reduction

8. Model Description

-   Input data size and features
-   Model Algorithm and Parameters
-   Model iterations can be discussed here if they are not saved out separately

9. Model Performance Metrics

-   Accuracy, R², RMSE, Confusion Matrix, Precision & Recall, AUC/ROC

10. Model Findings that may be interesting to decision makers
-   Feature importances
-  Volume of missing data
- Surprising correlations
#### Next Steps to communicate with stakeholders
-  Ready for production - yes/no?
-  Further feature engineering may be needed
-  Test new hyperparameters or different modeling methods
----------
Phew, that’s all folks! You’ve now seen all the steps involved in the data science project following the Data Science Method framework. Adopt and adapt as you see fit. Happy Modeling!

---
# Data Wrangling
This section provides more detail on some topics covered previously in the Data Science Method sections. 

## Missing Values
Learn advanced identification and imputation methods for missing values with this [Data Camp Course.](https://www.datacamp.com/courses/dealing-with-missing-data-in-python/?tap_a=5644-dce66f&tap_s=644217-4bb8b9)


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
## Data Visualization

- [ ] Which plots for which purpose or situation


[x]Balanced or unbalanced data --> [x]SMOTE or under sampling (ada sync) or bootstrapping to oversample

[x]Bar charts

[]Near miss for under sampling

[]Unbalanced response treated with stratifications

[]Word Count - bigram, trigrams

[]Bee swarm

[]Inferential statistics to confirm statistically unbalanced

[x]Scatter matrix

[x]Pearson correlation coefficients heat map

[x]Paired plot

[]Bi-plots

[]Histograms or Distribution plots

[x]Boxplots

[x]Outliers [1.5 * IQR, or extreme value analysis, Z-score 3 std] - frequency of words

[]Hypothesis testing with a/b like testing for same mean

[]Time series or line graphs
- [ ] Online Resource for learning Python data vis
- [ ] Online resource for R data vis 

## Math and Statistics for Data Scientists
Developing a proper understanding of the math and statistics behind data science algorithms will help you better understand when which modeling methods are most appropriate.

-   [Khan Academy Introduction to Matrices](https://www.khanacademy.org/math/precalculus/precalc-matrices)  
-   [Khan Academy Linear Algebra](https://www.khanacademy.org/math/linear-algebra)  
-   [Khan Academy Multivariable Calculus](https://www.khanacademy.org/math/multivariable-calculus)  
-   [Khan Academy Statistics and Probability](https://www.khanacademy.org/math/statistics-probability)  
-   [3blue1brown YouTube Channel](https://www.youtube.com/channel/UCYO_jab_esuFRV4b17AJtAw) 
-   [Math for Machine Learning on Coursera](https://bit.ly/courseraMathForML) 

[Statistical Thinking in Python part 1](https://www.datacamp.com/courses/statistical-thinking-in-python-part-1/?tap_a=5644-dce66f&tap_s=644217-4bb8b9)

[Statistical Thinking in Python part 2](https://www.datacamp.com/courses/statistical-thinking-in-python-part-2/?tap_a=5644-dce66f&tap_s=644217-4bb8b9)

---
# Feature Selection

Feature Selection Methods

[]N-grams optimization

[]Remove low variance features

[x]Remove features with Multi-colinearity

[]? Ridge can handle multicollinearity ?

[]Recursive Feature elimination within a particular model.

[]Stability selection methods

[]Select K-best features sklearn

[]Robust Scaler

[]Sklearn TSNE

[x]PCA/SVD

[x]PCA—>feature importance plot

[x]RF or other model feature importance output with Gini coefficient

[x]Lasso Regression -> L1 Regularization, penalty term is in the cost function reducing the coefs to zero.

[x]Chi-square Significance testing

### [Feature Selection & Dimension Reduction ](https://hub.packtpub.com/4-ways-implement-feature-selection-python-machine-learning/)

### [Automated Feature Engineering](https://github.com/Featuretools/predict-customer-churn/blob/master/churn/3.%20Feature%20Engineering.ipynb)



# Model Prep Steps

[]Build dummies

[]Cross validation (Training & testing split)

[]K-fold validation - segments of datasets, can be done within training set.
[]Grid search optimization on train data only

---
# Modeling Methods
As you may be aware there are countless types of machine learning model types and more variations are being added al time.  To be succesful as a data science professional you need to first learn the most broadly appropriate and applied methods and later you can delve into more specific solutions.

## Supervised Learning
[Classification, kNN, Cross-validation, Dimensionality Reduction](https://matterhorn.dce.harvard.edu/engage/player/watch.html?id=c322c0d5-9cf9-4deb-b59f-d6741064ba8a)

[This useful resource offers great advice about when different classification methods ought to be used.](http://blog.echen.me/2011/04/27/choosing-a-machine-learning-classifier/)

The modeling methods listed below are covered in detail [in this playlist.](https://www.r-bloggers.com/in-depth-introduction-to-machine-learning-in-15-hours-of-expert-videos/) The lectures are solid and the text they reference is excellent as well. Don't be detered byy the code examples being in R, there are plenty of Python coding examples out there, the main point is to gain the statistical concepts and insights.

[Linear Regression](https://docs.google.com/document/d/e/2PACX-1vQxEWaK8ZJJJBaX3prBT7WvZhPlXg146roKwFyw0RKEXLRDcFdxLZPC9ibwfZZOffN_le3Uc8h8oMC7/pub)

[Lasso Regression](https://docs.google.com/document/d/e/2PACX-1vTgO2Fykp7R1xB5VSxgCQ0R_iOi_nNEBHqGsN0VOiiGCkXNkfGqXHDpZCT0kW3wsZSJbVr0fvtuCFIz/pub)

Decision Trees

Random Forest 

SVM

KNN

## Unsupervised Learning

K means clustering

PCA


##  Decide Which Model to Try First

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

# Model Metrics

Model Evaluation\Interpretation

[x]Precision-False Pos emphasizes

[x]Recall - True Negs emphasis

[]F1-score-> Harmonic mean of precision and recall

[]F-beta -> calculate precision and recall for each class

[x]Confusion Matrix - classification report

[]Log loss

[x]AUC/ROC — 1 versus many for this case

[x]Accuracy Score

- [ ]  Model evaluation metrics in detail

# Practical Application
### If you want some help getting setup in [Python and Jupyter Notebooks](https://aidenvjohnson.com/wp-content/uploads/2020/05/Intro_python-1.html)

## Big Data 
Even though it’s a relatively new term, “big data” simply refers to a desire to glean relevant information from the most data. 

The sheer amount of data available is staggering, as data generation exponentially expands. In 2013, Science Daily [reported](https://www.sciencedaily.com/releases/2013/05/130522085217.htm) that 90% of all data ever created in history has been generated in the last two years; IBM followed up a year later with a reminder that each year we generate 10 times more data than the prior year. Today, IBM reports that 2.5 quintillion (2.5 x 1018) bytes of data are generated each day. As more devices - particularly internet-of-things devices — come online, and more and more people gain internet access, the data generated daily will only increase.
For a data scientist, the availability of big data is both enticing and daunting. To better comprehend big data, most companies will describe it in the context of the “3 Vs”: volume, velocity, and variety:

* **Volume:** Data comes from a variety of sources, including social media, transaction data, internet-of-things data, and sensor data. Storing this data used to be challenging — even prohibitive — but the availability of distributed storage systems such as Hadoop has reduced this barrier and allowed more data to be stored for longer periods of time.

* **Velocity:** Data often streams into the system at a very high rate, especially when considering point-of-sale transaction data, social media content, and sensor data. Effective utilization of the data requires that it be processed and acted upon in a timely fashion.

* **Variety:** Today, data scientists utilize more unique data types and formats than ever. These include structured data in databases, unstructured text, streaming sensor data, images, audio, stock ticker data, and many others. Big data tools allow data scientists to use varied formats together and identify common signal and information.
 

## Big Data with Spark

Adding big data to your toolkit means that you go from working on a dataset hosted on a single system to working with distributed datasets. The best means to work with distributed, massive datasets is within a distributed computing framework. Distributed computing brings significant challenges — How do you synchronize the code across many processors? What happens if a single processor fails? How do you roll up results when execution concludes?

Apache Spark aims to solve many of these challenges. Spark simplifies the tasks that bedevil developers when working on distributed computing including resource scheduling, job execution, communication between nodes, and so on. Spark was developed from the beginning to work with machine learning algorithms, which means it has been optimized for high-performance in situations where data is accessed multiple times over many iterations.

Spark is the leading open source distributed analytics platform. Its [project page](https://spark.apache.org/powered-by.html) lists almost 100 companies using Spark in production, and there are almost 400 active developers contributing to the codebase on GitHub.

Spark can run in standalone local mode with all processes inside a single Java Virtual Machine, or in standalone cluster mode. Data scientists interact with Spark via APIs in several languages. Spark supports 4 programming languages: Java, Scala, Python, and R. We’ll use Python in our examples for this course.

Spark uses a data representation called the Resilient Distributed Dataset (RDD). This is a data type very similar to the dataframe you know from Pandas but optimized to be distributed across multiple computers, residing in memory across all of them. Once an RDD has been created, by using Spark methods and functions, you interact with this distributed dataset as if it existed only on a single device. As an end developer, you don’t know — or need to know — how the RDD is actually allocated. Spark frees you from those details and allows you to focus on what is important to you — analyzing a dataset.

## Advanced topics
Consider learning more about these topicsas well.
- [ ] Recommendation Systems
- [ ] Time Series methods
- [ ] Dash Boards (Dask, plotly)
- [ ] Deep Learning - when is it needed or benefit/cost comparison












<!--stackedit_data:
eyJoaXN0b3J5IjpbLTg2MDQzODAyLC0xNTA4Njg0MzcxLC00OT
UxMTA1NzgsMTc1NTk3NzM5MCwtMTU5NDE5MTk4MCwtMTU4NTE5
MjcwMiwyMDA4MTQzNjQ4LC0yODIwMzEyNDcsNDkwNjEyMDI4LC
0xNDk2ODk5NDMxLC05NjI5Nzk3LDE5NDc1MDg2MzMsMTMzNzg5
NDIzNSwtMTE4ODg1MzcxMCwtMzk2OTM5MDExLC0xMjcxMjg0MD
gxLDU5NTA1Njg4NiwzMTgyNjA3MTUsOTM4OTc2MTUxLC0xMjIy
ODY4MDA0XX0=
-->