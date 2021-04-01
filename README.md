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

## Hypothesis Generation
<details>
<a name="Hypothesis Generation"></a>
<summary>Show/Hide</summary>
<br>
  1. Are younger customers more likely to subscribe to a term deposit as compared to old customers ?

 2. Are people with a higher bank balance more likely subscribe to term deposit than people with low balance ?

 3. Does a married person have higher chances to subscribe to a term deposit compared to a single or divorced person ? 

 4.  Does the length of the call made to the customers tell us anything about their chances of subscribing ?
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

using EDA we can find the answer of the initial hypothesis.

<b>Q. Do married people have more chances of subscribing to a term deposit ?</b>
<p>
  <img src="https://github.com/HardikMochi/Bank/blob/main/Image/2.PNG" width=600>
</p>

The data tells us quite a different story than our initial thought process, single people are the more likely to subscribe to a term deposit.

**Q. Do people with a higher bank balance more likely subscribe to term deposit than people with low balance ?**
<p>
  <img src="https://github.com/HardikMochi/Bank/blob/main/Image/3.PNG" width=600>
</p>
If you see the plot above median balance of customers not subscribing to a term deposit is around 400 whereas median balance of customers subscribing to a term deposit is 800. This definitely supports our initial hypothesis.
</details>


