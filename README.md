#Offline Task for Data Scientists - Predicting the Success of Term Deposit Marketing Activities

##Goal

Marketing campaigns constitute a typical strategy to generate business revenue. Companies use direct marketing when targeting segments of customers by contacting them to meet a specific business goal. Marketing activities carried out through a call-center are often called telemarketing activities.

The goal of this project is to build a data driven model that finds the customers that are most likely to subscribe to a product.

##Challenge Description

The company of this exercise is a retail bank. Between May 2008 and June 2013 the bank ran marketing campaigns based on phone calls. Often, more than one contact to the same customer was required in order to assess if the targeted product – a term deposit – would be subscribed to by a customer. Term deposits are generally short-term with maturities ranging anywhere from a month to a few years. When a term deposit is purchased, the lender (the customer) understands that the money can only be withdrawn after the term has ended or by giving a predetermined number of notice days. Term deposits are an extremely safe investment and are therefore very appealing to conservative, low-risk lenders. By having the money tied up for a longer period of time, lenders generally get a higher rate with a term deposit compared with a demand deposit.

You are in charge of figuring out how the marketing campaign performed and were asked the following questions:

* What percentage of users subscribed to the term deposit?
* Based on all the information you have about the calls, can you build a model to optimize future telemarketing activities to maximize the probability of subscription?
* By how much do you think your model could improve subscription rates? How would you test that?
* Did you find any interesting pattern on how the marketing campaign performed for different segments of users? Explain.

##Requirements

Please analyze the data using either Python, R or Excel (unless you have already agreed on another language/tool with the interviewer). You have three hours to work on the task. After three hours please send your solution per email. Your solution should include a report or presentation detailing your findings as well as any kind of source code you used.

##Data

We have a table with customer data downloadable by clicking here: https://drive.google.com/drive/folders/0B3ZqJXTBGPp1bFNpeHo3eUR3QVE?usp=sharing

The input variables of the customer data are:

###Customer Attributes

* Age (Numeric)
* Job, which is the type of the customer’s job (Categorical: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown')
* Marital: The customer’s marital status (Categorical: 'divorced','married','single','unknown';) Please note: 'divorced' means divorced or widowed
* Education (Categorical:'basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.cours’, 'university.degree','unknown')
* Default: Has the customer a credit in default? (Categorical: 'no','yes','unknown')
* Housing: Has the customer a housing loan? (Categorical: 'no','yes','unknown')
* Loan: Has the customer a personal loan? (Categorical: 'no','yes','unknown')
* Attributes of the Last Contact of the Current Campaign

* Contact: Contact communication type (Categorical: 'cellular','telephone')
* Month: Last contact month of year (Categorical: 'jan', 'feb',’mar’, 'nov', 'dec')
* Day_Of_Week: Last contact day of the week (Categorical: 'mon','tue','wed','thu','fri')
* Duration: Last contact duration, in seconds (Numeric). Important note: The duration is not known before a call is performed. Would you include this variable in a predictive model? Why? If yes, how?

###Other Attributes

* Campaign: Number of contacts performed during this campaign and for this customer (Numeric, includes last contact)
* Passed_Days: Number of days that passed by after the customer was last contacted from a previous campaign (Numeric; 999 means customer was not previously contacted)
* Previous: Number of contacts performed before this campaign and for this customer (Numeric)
* Previous_Outcome: Outcome of the previous marketing campaign (Categorical: 'failure','nonexistent','success')

###Social and Economic Context Attributes

* Emp_Var_Rate: Employment variation rate - quarterly indicator (Numeric)
* Cons_Price_Index: Consumer price index - monthly indicator (Numeric)
* Cons_Conf_Index: Consumer confidence index - monthly indicator (Numeric)
* Euribor3m: Euribor 3 month rate - daily indicator (Numeric)
* Nr_Employed: Number of employees - quarterly indicator (Numeric)
* Subscription - Output variable, the desired target - has the customer subscribed to a term deposit? (Binary: 'yes','no')
