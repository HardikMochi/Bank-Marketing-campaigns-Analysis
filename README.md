<h1><center>Bank Marketing campaign</center></h1>
Marketing campaigns are characterized by focusing on the customer needs and their overall satisfaction. Nevertheless, there are different variables that determine whether a marketing campaign will be successful or not. Some important aspects of a marketing campaign are as follows: 

<b>Segment of the Population</b>: To which segment of the population is the marketing campaign going to address and why? This aspect of the marketing campaign is extremely important since it will tell to which part of the population should most likely receive the message of the marketing campaign. 

<b>Distribution channel to reach the customer's place</b>: Implementing the most effective strategy in order to get the most out of this marketing campaign. What segment of the population should we address? Which instrument should we use to get our message out? (Ex: Telephones, Radio, TV, Social Media Etc.) 

<b>Promotional Strategy</b>: This is the way the strategy is going to be implemented and how are potential clients going to be address. This should be the last part of the marketing campaign analysis since there has to be an in-depth analysis of previous campaigns (If possible) in order to learn from previous mistakes and to determine how to make the marketing campaign much more effective.

There has been a revenue decline for the bank and they would like to know what actions to take. After investigation, it was found that the root cause is that their clients are not depositing as frequently as before. Term deposits allow banks to hold onto a deposit for a specific amount of time, so banks can lend more and thus make more profits. In addition, banks also hold better chance to persuade term deposit clients into buying other products such as funds or insurance to further increase their revenues.

## Tecnologies Used:
<details>
<a name="Technologies_Used"></a>
<summary>Show/Hide</summary>
<br>
    
* <strong>Python</strong>
* <strong>Pandas</strong>
* <strong>Numpy</strong>
* <strong>Matplotlib</strong>
* <strong>Seaborn</strong>
* <strong>Scikit-Learn</strong>
</details>


## Data Description
<details>
<a name="Data Description"></a>
<summary>Show/Hide</summary>
<br>
<h5 align="center">Dataset Description</h5>
<p align="center">
  <img src="https://github.com/HardikMochi/Bank/blob/main/Image/1.PNG" width=600>
</p>
 We can see that variables 1 to 16 can be used for modelling. 
 
Variable '**id**' is Identifier column. It has a unique value for every sample in the dataset and cannot be used for modelling.

Variable <b>term_deposit_subscribed</b> is Target/y column. It has binary values and we need to learn to predict this variable given our above 16 variables as features.
</details>




## Exploratory data analysis:
<details>
<a name="Exploratory data analysis"></a>
<summary>Show/Hide</summary>
<br>
We did following steps to explore the data set:

1. Brief Look at the Dataset
2. See the dataset shape.
3. Target Distribution.
4. See the variables datatypes.
5. See the number of missing/null values.
6. See the number of unique values in each variable. 


### **Analyzing Each Variable & their relationships**
There are two types of features that we have:

1. Categorical
2. Numerical

Also our target is Binary

For each feature type  perform two types of analysis:

1. Univariate: Analyze 1 feature at a time

2. Bivariate: Analyze the relationship of that feature with target variable, i.e. 'term_deposit_subscribed'

using EDA we can find the answer of the following Question.

<b>Q. Do married people have more chances of subscribing to a term deposit ?</b>
<p>
  <img src="https://github.com/HardikMochi/Bank/blob/main/Image/2.PNG" width=600>
</p>

The data tells us quite a different story than our initial thought process, single people are the more likely to subscribe to a term deposit.

**Q. Do people with a higher bank balance more likely subscribe to term deposit than people with low balance ?**
<p>
  <img src="https://github.com/HardikMochi/Bank/blob/main/Image/3.PNG" width=600>
</p>
If you see the plot above median balance of customers not subscribing to a term deposit is around 400 whereas median balance of customers subscribing to a term deposit is 800. 

**Q. Does the length of the call made to the customers tell us anything about their chances of subscribing ?**

<p align="center">
  <img src="https://github.com/HardikMochi/Bank/blob/main/Image/4.PNG" width=600 height=300>
</p>

From the plot above median last_call_duration made to the customers not subscribing to a term deposit is around 150 seconds. Median last_call_duration made to the customers subscribing to a term deposit is around 450 seconds.
</details>

### Model Devlopment:
<details open>
<summary>Show/Hide</summary>
<br>

I did data split into Train and Validation data . I also chose Stratified 5-fold has a my choice for cross validating.

For the majority of models I created, I applied hyperparameter tuning.


<h5 align="center">Table Comparing Best Models</h5>
<p align="center">
  <img src="https://github.com/HardikMochi/Bank/blob/main/Image/model.PNG" width=500 height=250>
</p>

from the above table conclude that Gradient Boosting algorithm give the best result. I chose the LightGBM model as my best model because it give best result also

Faster training speed campare to other Gradient Boosting algorithm
higher efficiency.
Lower memory usage.

I have saved all the models using the pickle library's dump function and stored them in the Models folder.
</details>

## Importance Features

<h5 align="center">Importance Features</h5>
<p align="center">
  <img src="https://github.com/HardikMochi/Bank/blob/main/Image/important feature.PNG">
</p>
<b>From the above Feature Importance chart last contact duration,Balance, day of the month, client age ('age'), number of client contacts during the current marketing campaign ('campaign'),and days since prev campaign contact are the imporatant features that drive the decision of the customer to purchase the term deposit or not.</b>




