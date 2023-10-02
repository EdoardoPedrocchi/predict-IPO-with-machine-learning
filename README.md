# predict-IPO-with-machine-learning

when a company decides to make an IPO is a crucial moment.
success or failure? life or death?

what if it were possible to develop a machine learning model that could predict what will happen after the IPO?

i tried to create it. could i have succeeded?

## BEFORE START

this is a build in public project.
what it means?
I'm at the start of my journey and i want to improve my skill constantly.
I created a first model with various strengths and weaknesses and as time goes by I will improve my skills by creating an ever better models.
Each model created will remain published in this repository to document my growth and the growth of this project.

WHY THIS PROJECT?

1. improve my coding skill in R
2. improve my data science and machine learning skill
3. improve my data visualization and data storytelling skill
4. apply the financial analysis skills learned during my studies
5. more important: understand if it is possible to predict success or failure of a company IPO

technology used: r, r studio 

so if you are interested in more information about the project, want to contribute or want to give me advice, please contact me.

ok, I'm done. we can start

## THE PROCESS USED

1. analyze the dataset : data exploration and statistical analysis
2. data visualization of the dataset
3. critical points
4. train and test the models
5. confront the results
6. conclusion

## THE FIRST MODEL

### 1.analyze the dataset

the dataset is composed using only data from the financial statements of companies that succeeded or failed in their IPOs.

this means that I have excluded relevant data such as the macroeconomic situation, the sector of the company, the situation of the financial market

why?

the aim of this first model is not to be the most accurate ever, but to see whether one can predict IPO performance from the company's financial statement alone.

a model comprising more variables and aiming for a much more accurate prediction will be developed later.
so: STAY TUNED.

the dataset contains the analysis of 11 companies(rows), for each companies are reported 8 variables(columns) that are calculated only using the company financial statement.

the variables used are:

- D/E
- EBITDA/revenue
- net profit margin
- current ratio
- times interest earned
- ROA
- ROE
- IPO(only 1= success IP= or 0= IPO filed)

values are only rations because it do not make sense to use integers values for companies of sizes and ages.

there are other 4 companies used as test set.

### 2.Data visualization

SOON

## 3.critical points

before start there are two problems of this project

1. **small dataset:**

 The data used are few to train a
machine learning model. 

why?

the process to find them is so long...they will be added over time

1. **few variables:** 

the training dataset excludes many fundamental variables such as the macroeconomic situation, the stock market situation, the sector in which the company operates, etc.

why?

the objective of this model is precisely try to predict IPOs using only financial statement data. in the future, a model will be created that includes more variables

## 4.train and test  the models

the models trained for this first project are two: logistic regression and random forest

**LOGISTIC REGRESSION**

**Advantages**

- Easy to interpret:
- Fast training and suitable for
small to medium-sized datasets.
- A good when the relationship is linear or linear in the log transformation.

**Disadvantages:**

- Not for modeling complex or non-linear
- Sensitive to outliers in the data.
- Requires the assumption of
linearity

**RANDOM FOREST**

**Advantages:**

- Good with complex and non-linear
data.
- Can handle both numerical and categorical data
- Reduces the risk of overfitting compared to a single decision tree.
- Provides feature importance(useful for
variable selection).

**Disadvantages:**

- require more time for training compared to simpler models (like
logistic regression).
- Less interpretable compared to linear
models( like logistic regression.)

## 5.confront the results

logistic regression’s accuracy = 50%

random forest’s accuracy = 100%

so random forest work better for this type of prediction.

according to random forest : ROE, times interests earned, current ratio are the variables most significant for the prediction

## 6.conclusion

predict  success or failure of a company IPO si possbile with machine learning but more analysis are needed:

use other models
add more data
add more variables
more trials on treshold

do you want to view a cool presentation of the project? [see my presentation](https://github.com/EdoardoPedrocchi/predict-IPO-with-machine-learning/blob/main/IPO_final.pdf)

would you like to see the dataset used? [click here](https://github.com/EdoardoPedrocchi/predict-IPO-with-machine-learning/blob/main/dataset)

would you see the code? [click here](https://github.com/EdoardoPedrocchi/predict-IPO-with-machine-learning/blob/main/code)

would you also like to try out the model?
please do so, but mention and contact me!
