# Machine Learning Zoomcamp
## 1.1 Introduction to Machine Learning
Predicting the price of car;

Machine learning to solve the problem: the best price to announce a car for selling.
What do we know about cars? year, make, mileage -> Price.
An expert can determine the price. They learn from data and extract some patterns.
Machine Learn: dataset that the model extract patterns.

**Features**: informations about the car

**Target**: what we want to predict: car price

With all the information we train a model.
The model is able to  predict the price car when given the car information;
**Machine Learning**: extracting patterns from data. Data two types: features, target. output is the Model. **Model** encapsulate all the patterns

![ML Flow](/img/predictions.png)
## 1.2 ML vs Rule-Based Systems
### Email system
Classify emails: spam or not spam
Patterns: what makes a spam message a spam?
- if sender= promotion@online.com then spam
- if title contains "tax review" and sender domain is "online.com" then spam
![Python Code Spam Email](/img/email.png)

Then new spams email don't attend to the previous rules; So adding new rules is endless. Difficult to mantain the code.

### Use Machine Learning
-  get data
- define & calculate features
- train and use the model

#### Features

Length of title > 10? true/false
- Length of body > 10? true/false
- Sender “promotions@online.com”? true/false #rules we have
- Sender “hpYOSKmL@test.com”? true/false
- Sender domain “test.com”? true/false #rules we have
- Description contains “deposit”? true/false #rules we have


## Start with rules and then use these rules as features

Analysing an email:
Check all the **features** (data): [1, 1, 0, 0, 1, 1] 

**Target** (desired output): 1

Last step: Then we train a model the output is the model.

ML: outcome is input (spam or not) | data
come out model to make predictions

## 1.3 Supervised Machine Learning

We teach the machines from examples. The model use patterns to make predictions. 
Ml part of CS and Maths, Stats

feature matrix = X
two dimension arrays.
Row observation/Columns are features

for each row we have a matrix y. we know if it is spam or not.
y=g(X)
y: one dimension array
X: two dimension of array. array of array table
g: the model

Different types:
regression: g returns a number
classification: output a category, not a number
    multiclass: muitiple different categories
    binary: spam or not spam
ranking:ordering elements

## 1.4 CRISP-DM
1. Understand the problem
1. collect the data
1. Train the model
1. use it

Cross-Industry Standard Process for Data Mining
1990 -> IBM

**Business understanging**: identify the business, problem how we can solve it. Do we actually need ML here? Define goals, measurable.way to measure sucess

**Data understanding**: sure if data available. collect data. Identify sources.

**Data preparation**: Transform the date so it can be put into a ML algorithm. Clean the data, remove noise. Buil pipelines. Convert into tabular form. X format

**Modeling**: train the model. Try different models and select the best one
which model? logistic regression, decision tree, neural network, etc...Fix data, add new feautures.

**Evaluation**: measure how well the model solve the business problems.. 'Goal', metric improved?

**Deployment**: Test the user in real users.   Roll model to all users. proper monitoring, ensure quality and maintainability.

**Iterate**: Go back to the first step. How to improve, is it good enough?

## 1.7 Introduction to NumPy
[Numpy notes](01_intro/01_intro_notes.md)

## 1.8 Linear Algebra

vector operantions

multiple a vector by a number

vector are columns

2 * [2 4 5 6 ] = [4 8 10 12]

[2 4 5 6] + [1 0 0 2] =[3 4 5 7]

### Multiplication
Vector-vector (dot product)
[2 4 5 6] * [1 0 0 2]
2*1 + 4*0 + 5*0 + 6*2 = 2+12 = 14
n
sum uivi
i=1
row
[2 4 5 6 ] [
            1  column
            0
            0
            2
            ]
