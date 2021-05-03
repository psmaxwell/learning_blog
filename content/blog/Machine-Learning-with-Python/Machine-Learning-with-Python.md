---
title: Machine Learning with Python
date: "2021-05-03"
description: "Hello, and welcome to Machine Learning with Python.
In this course, you’ll learn how Machine Learning is used in many key fields and industries.
For example, in the health care industry, data scientists use Machine Learning to predict
whether a human cell that is believed to be at risk of developing cancer, is either benign
or malignant.
As such, Machine learning can play a key role in determining a person’s health and welfare.
You’ll also learn about the value of decision trees and how building a good decision tree
from historical data helps doctors to prescribe the proper medicine for each of their patients.
You’ll learn how bankers use machine learning to make decisions on whether to approve loan
applications.
And you will learn how to use machine learning to do bank customer segmentation, where it
is not usually easy to run for huge volumes of varied data.
In this course, you’ll see how machine learning helps websites such as YouTube, Amazon, or
Netflix develop recommendations to their customers about various products or services, such as
which movies they might be interested in going to see or which books to buy.
There is so much that you can do with Machine Learning!
Here, you’ll learn how to use popular python libraries to build your model.
For example, given an automobile dataset, we use the sci-kit learn (sklearn) library
to estimate the Co2 emission of cars using their Engine size or Cylinders.
We can even predict what the Co2 emissions will be for a car that hasn’t even been
produced yet!
And we’ll see how the telecommunications industry can predict customer churn.
You can run and practice the code of all these samples using the built-in lab environment
in this course.
You don’t have to install anything to your computer or do anything on the cloud.
All you have to do is click a button to start the lab environment in your browser.
The code for the samples is already written using python language, in Jupyter notebooks,
and you can run it to see the results, or change it to understand the algorithms better.
So, what will you be able to achieve by taking this course?
Well, by putting in just a few hours a week over the next few weeks, you’ll get new
skills to add to your resume, such as regression, classification, clustering, sci-kit learn
and SciPy.
You’ll also get new projects that you can add to your portfolio, including cancer detection,
predicting economic trends, predicting customer churn, recommendation engines, and many more.
You’ll also get a certificate in machine learning to prove your competency, and share
it anywhere you like online or offline, such as LinkedIn profiles and social media.
So let’s get started.
"
---

### A FEW THINGS TO KNOW ABOUT THIS COURSE
* This course is self-paced. There is no instructor to follow or to rush you along - you learn on your own schedule. This also means you are going to need to be disciplined in your studies.
* You can start it at any time and you can take as long as you need to complete it. Your place in the course will be remembered and your labs will be saved. However, we strongly recommend that you don't take prolonged breaks between lessons as the mind tends to forget what it does not practice.
* You can take the course (audit) as many times as you wish.
* There is only ONE chance to pass the course, but you can make multiple attempts per question (see the Grading Scheme section for details)
* This is a hands-on course where you will gain practical skill by doing hands-on labs. We provide a a complete virtual lab environment on the cloud that you can access from anywhere as long as you have internet connection.
* We strongly recommend that you use Chrome or Firefox browser
* You can learn on mobile device if you install Cognitive Class mobile app from Apple App Store (coming soon) or Google Play Store.

### Learning Objectives
#### In this course you will learn about:
- How Statistical Modeling relates to Machine Learning and do a comparison of each.
- Real-life examples of Machine learning and how it affects society in ways you may not have guessed!
- In the labs: Use Python libraries for Machine Learning, such as scikit-learn.

#### Explore many algorithms and models:
- Popular algorithms: Regression, Classification, and Clustering
- Recommender Systems: Content-Based and Collaborative Filtering
- Popular models: Train/Test Split, Gradient Descent, and Mean Squared Error
- Get ready to do more learning than your machine!

### Syllabus
#### Module 1 - Machine Learning
- Python for Machine Learning
- Supervised vs Unsupervised

#### Module 2 - Regression
- Simple Linear Regression
- Multiple Linear Regression
- Model Evaluation in Regression Models
- Non-Linear Regression

#### Module 3 - Classification
- K-Nearest Neighbors
- Decision Trees
- Evaluation Metrics in Classification
- Logistic Regression vs Linear Regressin
- Support Vector Machine (SVM)

#### Module 4 - Clustering
- K-Means Clustering
- Hierarchical Clustering
- DBSCAN

#### Module 5 - Recommender Systems
- Content-Based Recommender Systems
- Collaborative Filtering

### ** Learning Objectives
- Machine Learning applications
- Python libraries for Machine Learning
- Supervised vs Unsupervised Learning

#### Intro to Machine Learning
Machine learning is the subfield of computer science that gives "computers the ability
to learn without being explicitly programmed.”
First, how do you think Netflix and Amazon recommend videos, movies, and TV shows to its users?
They **use Machine Learning to produce suggestions that you might enjoy!**
This is similar to how your friends might recommend a television show to you, based
on their knowledge of the types of shows you like to watch.
How do you think banks make a decision when approving a loan application?
They **use machine learning to predict the probability of default for each applicant, and then approve or refuse the loan application based on that probability.**
**Telecommunication companies use their customers’ demographic data to segment them, or predict if they will unsubscribe from their company the next month.**
There are many other applications of machine learning that we see every day in our daily life, such as chatbots, logging into our phones or even computer games using face recognition Each of these use different machine learning techniques and algorithms.So, let’s quickly examine a few of the more popular techniques.**The Regression/Estimation technique is used for predicting a continuous value**, for example,predicting things like the price of a house based on its characteristics, or to estimate the Co2 emission from a car’s engine.
**A Classification technique is used for Predicting the class or category of a case,** for example,if a cell is benign or malignant, or whether or not a customer will churn.
**Clustering groups of similar cases**, for example, can find similar patients, or can be used for customer segmentation in the banking field.**Association technique is used for finding items or events that often co-occur**, for example,grocery items that are usually bought together by a particular customer.
**Anomaly detection is used to discover abnormal and unusual cases**, for example, it is used for credit card fraud detection.
**Sequence mining is used for predicting the next event**, for instance, the click-stream in websites.Dimension reduction is used to reduce the size of data.
And finally, recommendation systems; this associates people's preferences with others who have similar tastes, and recommends new items to them, such as books or movies.
We will cover some of these techniques in the next videos.By this point, I’m quite sure this question has crossed your mind, “What is the difference
between these buzzwords that we keep hearing these days, such as Artificial intelligence(or AI), Machine Learning and Deep Learning?”
Well, let me explain what is different between them.In brief, **AI tries to make computers intelligent in order to mimic the cognitive functions of humans**.So, **Artificial Intelligence is a general field with a broad scope including: Computer Vision,Language Processing, Creativity, and Summarization.Machine Learning is the branch of AI that covers the statistical part of artificial intelligence**.It teaches the computer to solve problems by looking at hundreds or thousands of examples,learning from them, and then using that experience to solve the same problem in new situations.And **Deep Learning is a very special field of Machine Learning where computers can actually learn and make intelligent decisions on their own.Deep learning involves a deeper level of automation in comparison with most machine learning algorithms.**Now that we’ve completed the introduction to Machine Learning, subsequent videos will focus on reviewing two main components: First, you’ll be learning about the purposeof Machine Learning and where it can be applied in the real world; and Second, you’ll get a general overview of Machine Learning topics, such as supervised vs unsupervised learning, model evaluation and various Machine Learning algorithms.So now that you have a sense with what’s in store on this journey, let’s continue our exploration of Machine Learning!

#### Python for Machine Learning
 we’ll talk about **how to use python for machine learning**.**Python is a popular and powerful general-purpose programming language that recently emerged as the preferred language among data scientists**.You can write your machine learning algorithm using python, and it works very well. However, **there are a lot of modules and libraries already implemented in python that can make your life much easier**.We try to introduce the Python packages in this course and use it in the labs to give you better hands-on experience.The first package is **Numpy, which is a math library to work with n-dimensional arrays in Python.It enables you to do computation efficiently and effectively.It is better than regular python because of it’s amazing capabilities.**For example, **for working with arrays, dictionaries, functions, datatypes, and working with images,you need to know Numpy**.**SciPy is a collection of numerical algorithms and domain-specific toolboxes, including signal processing, optimization, statistics and much more.SciPy is a good library for scientific and high-performance computation**.**Matplotlib is a very popular plotting package that provides 2D plotting as well as 3D plotting**.Basic Knowledge about these 3 packages, which are built on top of python, is a good asset for data scientists who want to work with real world problems.If you are not familiar with these packages, I recommend that you take the “Data Analysis with Python” course first.This course covers most of the useful topics in these packages.**Pandas library, is a very high-level python library that provides high-performance, easy to use data structures.It has many functions for data importing, manipulation and analysis.In particular, it offers data structures and operations for manipulating numerical tables and time series**.**scikit-learn is a collection of algorithms and tools for machine learning**, which is our focus here, and which you’ll learn to use with in this course.As we’ll be using scikit-learn quite a bit, in the labs, let me explain more about it and show you why it is so popular among data scientists.**Scikit-learn is a free machine learning library for the Python programming language.It has most of the classification, regression and clustering algorithms, and it’s designed to work with the Python numerical and scientific libraries, NumPy and SciPy.Also, it includes very good documentation**.On top of that, implementing machine learning models with scikit learn is really easy, with a few lines of python code.**Most of the tasks that need to be done in a machine learning pipeline are implemented already in scikit learn, including, pre-processing of data, feature selection, feature extraction,train/test splitting, defining the algorithms, fitting models, tuning parameters, prediction,evaluation, and exporting the model.Let me show you an example of how scikit learn looks like when you use this library**.You don’t have to understand the code for now, but just see how easily you can build a model with just a few lines of code.Basically, Machine learning algorithms benefit from standardization of the data set.If there are some outliers, or different scales fields in your data set, you have to fix them.The preprocessing package of scikit learn provides several **common utility functions and transformer classes to change raw feature vectors into a suitable form of vector for modeling**.You have to split your dataset into train and test sets to train your model, and then test the model’s accuracy separately.**Scikit learn can split arrays or matrices into random train and test subsets for you,in one line of code**.Then, you can setup your algorithm.For example, you can build a classifier using a support vector classification algorithm.We call our estimator instance clf, and initialize its parameters.Now, you can train your model with the train set.By passing our training set to the fit method, the clf model learns to classify unknown cases.Then, we can use our test set to run predictions.And, the result tells us what the class of each unknown value is.Also, you can use different metrics to evaluate your model accuracy, for example, using a confusion matrix to show the results.And finally, you save your model.You may find all or some of these machine learning terms confusing, but don’t worry,we will talk about all of these topics in the following videos.The most important point to remember is that the entire process of a Machine Learning task can be done simply in a few lines of code, using scikit learn.Please notice that, though it is possible, it would not be that easy if you want to do all of this using Numpy or Scipy packages.And of course, it needs much more coding if you use pure python programming to implement all of these tasks.