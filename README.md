# Credit_Risk_Analysis***Overview of our model:***
The lead data scientist, Jill, has asked me  to create the same development environment that she is using. This step will help you run the code smoothly without conflicts.
Broadly speaking, machine learning can be divided into three learning categories: 
Supervised.
Unsupervised.
deep. 
For our purposes, I will  only discuss supervised and unsupervised learning
Jill, the  data scientist boss, asks me to research the difference between regression and classification models, then report back to her. Here is what I  find out.
Jill now believes that I am  ready to try r hand at solving a classification problem with machine learning. The first model you will use is logistic my regression, a popular classification model. 
She explains that despite its name, logistic regression is actually not a regression model. It is a classification model. With logistic regression, it is possible to try to answer questions such as whether a credit card holder is likely to miss a payment in the next month.
Now that I have gotten my feet wet with logistic regression, Jill believes that it's time to implement a model with a real dataset. In the next step, I  will follow the familiar pattern as you instantiate a model, train it, create predictions, then validate the model.


Jill informs me  that a good data scientist not only understands the how  is but the whys. She explains that understanding how a model works helps a data scientist assess a machine learning model's strengths, weaknesses, and how best to use it. She asks me to look into how a logistic regression model works.

When i protest that I have not  taken a math class in years, she reassures me  that while math is indeed helpful to know, many basic underlying ideas in machine learning can be grasped without a graduate degree in math.

It is not enough to use a machine learning model to create predictions. The model must answer an important question:
how well does it perform? I have showed Jill that accuracy score is one way of assessing a classification model's performance. That is, what percentage of predictions does it get right?

Jill explains that there are other ways to validate a classification model, and asks me  to look into them. This is where the statistical rubber meets the road.


Jill and me agreed  that metrics such as sensitivity and precision can be a bit confusing at first. 
So we decided we will return to a real-world dataset to deepen your understanding.
Now that we 're becoming comfortable with using logistic regression and evaluati its results, Jill suggests that you learn about another powerful classification model: support vector machines. Although the name is possibly a little intimidating, you'll be able to bring much of your previous knowledge into using a support vector machine in practice.

While many datasets contain categorical features (e.g., M or F), machine learning algorithms typically only work with numerical data. Categorical and text data must therefore be converted to numerical data for use in machine learning—which is what we'll do in this section.


Every machine learning task can be performed by out-of-the-box solutions, meaning libraries written by other programmers. Sometimes you have to roll up your sleeves and write your own custom code!
And clean the data before analysis .
One of the tasks involved in data preparation for machine learning is to convert textual data into numerical data.


Now that we have prepared the data, you will put the random forest classifier model to practice, then evaluate the results.

Bootstrap aggregation, or "bagging," is an ensemble learning technique that combines weak learners into a strong learner. In fact, you have already seen a model that uses bootstrap aggregation as part of its algorithm: the random forest model.

Decision trees are prone to overfitting, meaning that the algorithm's predictions are excessively tailored to the specific dataset. When there's overfitting, a model's performance will suffer when it encounters a new dataset. One way to try to overcome this problem is with bootstrap aggregation. Let's look at how it works in more detail.
We did a  great work so far. Well done! Before setting free to tackle our machine learning project , however, we like to demonstrate a family of resampling techniques designed to deal with class imbalance.

Class imbalance is a common problem in classification. It occurs when one class is much larger than the other class. For example, if you work for a credit card company and want to detect fraudulent transactions, you will deal with many more non-fraudulent transactions than fraudulent ones. In this case, the non-fraudulent class is much larger than the fraudulent class.

Under myself and Jill's tutelage, we will introduce  three techniques to address class imbalance: 
Oversampling.
 Undersampling.
 And  a Combination approach of oversampling and undersampling. 

The Results :
Its important to point out that  the improvements seem to be modest, incremental improvements are usually more realistic than drastic ones. 
small improvements, in tandem with other tweaks, can add up to make a significant difference. For now, however, I used  SMOTEENN, an approach to resampling that combines aspects of both oversampling and undersampling.
Below is a summary of all the six models results 

 MODEL	Accuracy	Precision	Recall
EASY ENSEMBLE	68%	0.88	0.37
Balanced Random forest	68%	0.88	0.37
COMBINATION OVER AND UNDER 	63%	0.01	0.68
Smote undersampling	53%	0.01	0.53
Smote over sampling	64%	0.01	0.56
Naïve Raandom Oversampling	55%	0.01	0.53
![image](https://user-images.githubusercontent.com/89116297/170838922-4f6e2b02-f467-4f3d-b0ed-041a2b8ddf58.png)


Summary :
I personally recommend depending on the analysis run above the easy ensemble classifier with accuracy of 68% and 0.88 precision and recall of 0.37 in high risk  &   1.0 and 1.0  low risk .
