# DS5500-HW3

# Problem 1:
Imported all necessary python packages and required data sources and performed necessary preprocessing. Below we obtained visualizations 
of states that take in the most federal funding revenue.

![1](/pic1.JPG)

![2](/pic7.JPG)

We can see from the graph that california, texas, new york, illinois, florida have the highest federal funding revenues. We can also say
that california and texas have very high values when compared to other states.

Below graph gives the state values for most federal funding per student

![3](/pic2.JPG)

district of columbia and alaska spend more federal funding than other states, we obtained this value by dividing total available 
federal funding by total number of states.

# Problem 2:
Visualize the relationship between school districts’ total revenue and expenditures.

We have extracted required total revenue and total expenditure, in the below plot we can see expenditure and revenue distribution graph
![1](/pic3.JPG)

Which states have the most debt per student?
![2](/pic4.JPG)

![2](/pic5.JPG)

In the above graphs and tables we can see that north dakota and district of columbia have the highest debt per student

# Problem 3:
Write and explain a function for processing a single column of “blurred” metrics into usable numeric values.

Here, we have written a function that processes a column in the dataset that converts blurred values to usable values.
We wrote multiple conditions with if and else if conditions to process this column. Lower limit and upper limit for this column are
0 and 100, hence, range of this column is 0-100.

for less than, LT condition, we take the value as ((int(value.split('LT')[1])-1)+0)/2
for greater than, GT condition, we take the value as ((int(value.split('GT')[1])+1)+100)/2
for less than equal to, LE condition, we take the value as ((int(value.split('LE')[1]))+0)/2
for greater than equal to, GE condition, we take the value as ((int(value.split('GE')[1]))+100)/2

if 'PS' or nan is present then we use the value of nan

Use it to process and then visualize the distribution of a performance metric of your choice.

Here, we have used 'MAM_MTH00PCTPROF_1516' column to visualize distribution of performance metric of our choice. This metric gives out the values for performance percentage in mathematics for the year 2015-2016. Below graph gives out the values.

![2](/pic9.JPG)

# Problem 4:

You are tasked with cutting 15% of the U.S. federal budget currently being spent on funding school districts.
How much money is this?

Total funding revenue amounts to 55602739138, budget cuts are supposed to be 15% which accounts to 8340411300. Amount of revenue remaining is 47262328267.299995

(You should produce a table of LEA IDs and the dollar amount by which their federal funding will be cut –
you do not need print the entire table.)
Table of LEA ID's is as follows:

![2](/pic6.JPG)


# Problem 5:

Provide a statement for your supervisor justifying your decisions on which school districts will lose funding.

Reducing equal amount of funding from each of the districts would not be wise, as there are districts that have excess fundings. We would have to cut 15% of federal funding, so we would have to identify districts that have enough surplus amount and pull this amount from surplus districts. We need to cut funding from districts with enough surplus until cutting reaches 8340411300.







!
