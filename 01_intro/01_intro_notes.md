# Machine Learning Zoomcamp
## 1.1 Introduction to Machine Learning 🚀
Predicting the price of a car:

Machine learning can solve the problem of determining the best price to announce a car for selling.
What do we know about cars? Year, make, mileage -> Price.
An expert can determine the price by learning from data and extracting patterns.
Machine Learning: using a dataset to allow the model to extract patterns.

**Features**: information about the car

**Target**: what we want to predict: car price

With all the information, we train a model.
The model is able to predict the car price when given the car information.
**Machine Learning**: extracting patterns from data. Data has two types: features and target. The output is the Model. **Model** encapsulates all the patterns.

![ML Flow](/img/predictions.png)

## 1.2 ML vs Rule-Based Systems ⚖️
### Email System 📧
Classify emails: spam or not spam
Patterns: what makes a spam message a spam?
- if sender = promotion@online.com then spam
- if title contains "tax review" and sender domain is "online.com" then spam

![Python Code Spam Email](/img/email.png)

New spam emails don't adhere to the previous rules, so adding new rules is endless and difficult to maintain the code.

### Use Machine Learning
- Get data
- Define & calculate features
- Train and use the model

#### Features

- Length of title > 10? true/false
- Length of body > 10? true/false
- Sender “promotions@online.com”? true/false
- Sender “hpYOSKmL@test.com”? true/false
- Sender domain “test.com”? true/false
- Description contains “deposit”? true/false

## Start with rules and then use these rules as features

Analyzing an email:
Check all the **features** (data): [1, 1, 0, 0, 1, 1]

**Target** (desired output): 1

Last step: Train a model; the output is the model.

ML: outcome is input (spam or not) | data
Outcome model to make predictions

## 1.3 Supervised Machine Learning 🎓

We teach the machines from examples. The model uses patterns to make predictions.
ML is part of CS, Maths, and Stats.

Feature matrix = X
Two-dimensional arrays.
Rows are observations/Columns are features.

For each row, we have a matrix y. We know if it is spam or not.
y = g(X)
y: one-dimensional array
X: two-dimensional array. Array of arrays (table)
g: the model

Different types:
- Regression: g returns a number
- Classification: output a category, not a number
    - Multiclass: multiple different categories
    - Binary: spam or not spam
- Ranking: ordering elements

## 1.4 CRISP-DM 📊
1. Understand the problem
2. Collect the data
3. Train the model
4. Use it

Cross-Industry Standard Process for Data Mining
1990 -> IBM

**Business Understanding**: Identify the business problem and how we can solve it. Do we actually need ML here? Define goals and measurable ways to measure success.

**Data Understanding**: Ensure data is available. Collect data. Identify sources.

**Data Preparation**: Transform the data so it can be put into an ML algorithm. Clean the data, remove noise. Build pipelines. Convert into tabular form (X format).

**Modeling**: Train the model. Try different models and select the best one. Which model? Logistic regression, decision tree, neural network, etc. Fix data, add new features.

**Evaluation**: Measure how well the model solves the business problems. 'Goal', metric improved?

**Deployment**: Test the model with real users. Roll out the model to all users. Proper monitoring, ensure quality and maintainability.

**Iterate**: Go back to the first step. How to improve, is it good enough?

## 1.7 Introduction to NumPy 📐
[Numpy notes](01_intro/01_intro_notes.md)

## 1.8 Linear Algebra ➗

Vector operations

Multiply a vector by a number

Vectors are columns

2 * [2 4 5 6] = [4 8 10 12]

[2 4 5 6] + [1 0 0 2] = [3 4 5 7]

### Multiplication
Vector-vector (dot product)
[2 4 5 6] * [1 0 0 2]
2*1 + 4*0 + 5*0 + 6*2 = 2+12 = 14

```
[2 4 5 6] 
[1 0 0 2]
```
