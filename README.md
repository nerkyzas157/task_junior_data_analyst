# Task for the candidates to the Junior Data Analyst position


This repository contains a sample dataset and the task description for the candidates to the Junior Data Analyst position in Inspired UM. 

The aim of the task is to carry out exploratory data analysis of the provided dataset and to present results as Jupyter notebook. 

The full task description can be found in [Task.md](Task.md) file. 


## Data Set Information:

The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (has_deposit) would be ('yes') or not ('no') subscribed.

## Attribute Information:

### Bank client data:

* age (numeric)
* job: type of job (categorical: 'admin.', 'blue-collar', 'entrepreneur', 'housemaid', 'management', 'retired', 'self-employed', 'services', 'student', 'technician', 'unemployed', 'unknown')
* marital: marital status (categorical: 'divorced', 'married', 'single', 'unknown' ; note: 'divorced' means divorced or widowed)
* education: (categorical: 'basic.4y', 'basic.6y', 'basic.9y', 'high.school', 'illiterate', 'professional.course', 'university.degree', 'unknown')
* default: has credit in default? (categorical: 'no', 'yes', 'unknown')
* housing: has housing loan? (categorical: 'no', 'yes', 'unknown')
* loan: has personal loan? (categorical: 'no', 'yes', 'unknown')

### Related with the last contact of the current campaign:
* contact: contact communication type (categorical:'cellular','telephone')
* month: last contact month of year (categorical: 'jan', 'feb', 'mar', …, 'nov', 'dec')
* day_of_week: last contact day of the week (categorical:'mon','tue','wed','thu','fri')
* duration: last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration=0 then has_deposit='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call 'has_deposit' value is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.

### Other attributes:
* campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)
* pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric, value of 999 means that client was not previously contacted)
* previous: number of contacts performed before this campaign and for this client (numeric)
* poutcome: outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success')

### Social and economic context attributes
* emp_var_rate: employment variation rate - quarterly indicator (numeric)
* cons_price_idx: consumer price index - monthly indicator (numeric)
* cons_conf_idx: consumer confidence index - monthly indicator (numeric)
* euribor3m: euribor 3 month rate - daily indicator (numeric)
* nr_employed: number of employees - quarterly indicator (numeric)

### Desired target:
* has_deposit - has the client subscribed a term deposit? (binary: 'yes', 'no')

# Source:
Dataset from : http://archive.ics.uci.edu/ml/datasets/Bank+Marketing#
Description from: https://www.kaggle.com/datasets/henriqueyamahata/bank-marketing?resource=download
