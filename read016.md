# Data Science Primer 

![DataScience](https://elitedatascience.com/wp-content/uploads/2018/05/What-Goes-Into-a-Successful-Model.jpg)


## Chapter 1: Bird's Eye View

Machine learning is the practice of teaching computers how to learn patterns from data, often for making decisions or predictions.

**Key Terminology**

1. Model - a set of patterns learned from data.
2. Algorithm - a specific ML process used to train a model.
3. Training data - the dataset from which the algorithm learns the model.
4. Test data - a new dataset for reliably evaluating model performance.
5. Features - Variables (columns) in the dataset used to train the model.
6. Target variable - A specific variable you're trying to predict.
7. Observations - Data points (rows) in the dataset.



**Machine Learning Tasks**



Academic machine learning starts with and focuses on individual algorithms. However, in applied machine learning, you should first pick the right machine learning task for the job.

A **task** is a specific objective for your algorithms.

**Algorithms** can be swapped in and out, as long as you pick the right task.



### Supervised Learning

Supervised learning includes tasks for "labeled" data (i.e. you have a target variable).

In practice, it's often used as an advanced form of predictive modeling.

Each observation must be labeled with a "correct answer."

Only then can you build a predictive model because you must tell the algorithm what's "correct" while training it (hence, "supervising" it).

**Regression** is the task for modeling continuous target variables.

**Classification** is the task for modeling categorical (a.k.a. "class") target variables.


### Unsupervised Learning

Unsupervised learning includes tasks for "unlabeled" data (i.e. you do not have a target variable).


In practice, it's often used either as a form of automated data analysis or automated signal extraction.

Unlabeled data has no predetermined "correct answer."

You'll allow the algorithm to directly learn patterns from the data (without "supervision").

**Clustering** is the most common unsupervised learning task, and it's for finding groups within your data.


**Three elements of great machine learning**


1. A skilled chef (Human guidance) - First, even though we are “teaching computers to learn on their own,” human guidance plays a huge role.

2. Fresh ingredients (Clean relative data) - The second essential element is the quality of your data.

3. Don’t overcook it (Avoid overfitting) - An overfit model has “memorized” the noise in the training set, instead of learning the true underlying patterns.


**The Blueprint**

Our machine learning blueprint is designed around those 3 elements.

There are 5 core steps:
1. Exploratory Analysis

First, "get to know" the data. This step should be quick, efficient, and decisive.

2. Data Cleaning

Then, clean your data to avoid many common pitfalls. Better data beats fancier algorithms.

3. Feature Engineering

Next, help your algorithms "focus" on what's important by creating new features.

4. Algorithm Selection

Choose the best, most appropriate algorithms without wasting your time.

5. Model Training

Finally, train your models. This step is pretty formulaic once you've done the first 4.




## Exploratory Analysis

**Why explore your dataset upfront?**

* You’ll gain valuable hints for Data Cleaning (which can make or break your models).

* You’ll think of ideas for Feature Engineering (which can take your models from good to great).

* You’ll get a “feel” for the dataset, which will help you communicate results and deliver greater impact.




## Data Cleaning

**Remove Unwanted observations**


The first step to data cleaning is removing unwanted observations from your dataset.

This includes duplicate or irrelevant observations.


**Duplicate observations**


Duplicate observations most frequently arise during data collection, such as when you:

1. Combine datasets from multiple places


2. Scrape data


3. Receive data from clients/other departments



**Irrelevant observations**


Irrelevant observations are those that don’t actually fit the specific problem that you’re trying to solve.





## Feature Engineering

**What is Feature Engineering?**


Feature engineering is about creating new input features from your existing ones.

**Infuse Domain Logic**

Here you can engineer informative features according to your or others’ expertise about domain, by thinking about information you might need to isolate.

**Create Interaction Features**

You can look at each pair of features and ask yourself, “could I combine this information in any way that might be even more useful?”

**Combine Sparse Classes**

Sparse classes (in categorical features) are those that have very few total observations. They can be problematic for certain machine learning algorithms, causing models to be overfit.

* There’s no formal rule of how many each class needs.


* It also depends on the size of your dataset and the number of other features you have.


* As a rule of thumb, we recommend combining classes until each one has at least ~50 observations.


So at first, we group similar classes, and thus we have fewer unique classes but each one has more observations.

**Add Dummy Variables**

**Dummy variables** are a set of binary (0 or 1) variables that each represent a single class from a categorical feature.

Most machine learning algorithms cannot directly handle categorical features, specifically, they cannot handle text values therefore, we need to create dummy variables for our categorical features.

**Remove Unused Features**

Unused features are those that don’t make sense to pass into our machine learning algorithms. Examples include:

* ID columns

* Features that wouldn’t be available at the time of prediction

* Other text descriptions


## Algorithm Selection

And yes, just 5 for now. Instead of giving you a long list of algorithms, our goal is to explain a few essential concepts (e.g. regularization, ensembling, automatic feature selection) that will teach you why some algorithms tend to perform better than others. In applied machine learning, individual algorithms should be swapped in and out depending on which performs best for the problem and the dataset. Therefore, we will focus on intuition and practical benefits over math and theory.

**Regularization in Machine Learning**

**Lasso Regression**

* Lasso, or LASSO, stands for Least Absolute Shrinkage and Selection Operator.

* Lasso regression penalizes the absolute size of coefficients.

* Practically, this leads to coefficients that can be exactly 0.

* Thus, Lasso offers automatic feature selection because it can completely remove some features.

* the “strength” of the penalty should be tuned.

* A stronger penalty leads to more coefficients pushed to zero.


**Ridge Regression**

* Ridge regression penalizes the squared size of coefficients.

* Practically, this leads to smaller coefficients, but it doesn’t force them to 0.

* In other words, Ridge offers feature shrinkage.

* Again, the “strength” of the penalty should be tuned.

* A stronger penalty leads to coefficients pushed closer to zero.

**Elastic-Net**

* Elastic-Net penalizes a mix of both absolute and squared size.

* The ratio of the two penalty types should be tuned.

* The overall strength should also be tuned.


## Model Training

There are a few key techniques that we’ll discuss, and these have become widely-accepted best practices in the field. Again, this mini-course is meant to be a gentle introduction to data science and machine learning, so we won’t get into the nitty gritty yet. We have plenty of other tutorials for that.

It might seem like it took us a while to get here, but professional data scientists actually spend the bulk of their time on the steps leading up to this one:

* Exploring the data.

* Cleaning the data.

* Engineering new features.

this is how to set up the entire modeling process to maximize performance while safeguarding against overfitting. We will swap algorithms in and out and automatically find the best parameters for each one.

Split Dataset to train and test parts

Cross-validation is a method for getting a reliable estimate of model performance using only your training data. There are several ways to cross-validate. The most common one, 10-fold cross-validation, breaks your training data into 10 equal parts (a.k.a. folds), essentially creating 10 miniature train/test splits.