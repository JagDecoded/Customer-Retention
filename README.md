# Customer Retention


Retention - The action of absorbing and continuing to hold a substance. ~ Google Dictionary

Customer retention is the ability of a business to retain customers.

Doing customer retention analysis can help businesses keep an eye on customer's habits and behavior, and also can help make better strategy to increase sales.

Customer Retention analysis can be done by grouping customers with similarities (Cohort group) and observing their behavior with respect to regular interval of time. This is just a way. 

### Problem:

We have an Order Table with the schema(id, user_id, total, created). We have to analyze the data for customer retention (Week-wise) and represent the data visually for better representation. 

### Plan of attack 

__STEP 1 :__ Create *Cohort Group* By grouping customers who made their first purchase in a similar time interval. For us, it's there FIRST PURCHASE WEEK.

__STEP 2:__ Create period column to assign the order date a week group. So to know who placed order in what week.

__STEP 3:__ Group Data By *Cohort Group* and then *Period Group* to understand how many of the same *Cohort Group* placed order in other *Period Group*

__STEP 4:__ Keep customer group behavior for the next 10 weeks from their first purchase week. 


We Trying to build something like this first then visualize:

![Customer Retention](https://i.imgur.com/6nfchMZ.png)


### File Reference

__order data.xlsx__ input data

__Customer Retention Alanlysis.ipynb__ Code file (Jupyter Notebook)

__retention.csv__ Output file 

__user retention.png__ Heat map for our data 


![Customer Retention graph from Week 1- Week 10](https://github.com/JagDecoded/Customer-Retention/blob/master/user%20retention.png)
