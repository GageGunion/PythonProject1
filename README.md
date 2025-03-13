<h1>Python Project - Carly's Clipers</h1>

<h2>Description</h2>
This is a project from codeacademy I completed that is focusing on the use of for loops to list some data from a salon business using Python. This project starts by listing the haircut styles and pricing and then takes the average of the prices. A list of new prices is then created. The reveune is calculated for the number of each haircut listed in the variable last_week. The average daily reveune is also calculated as well as a list of haircuts under thirty dollars.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Python</b> 

<h2>Program walk-through:</h2>

<p align="center">
Project Promt: <br/>
<img src="https://imgur.com/ag6MATd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
</p>

```commandline
hairstyles = ["bouffant", "pixie", "dreadlocks", "crew", "bowl", "bob", "mohawk", "flattop"]

prices = [30, 25, 40, 20, 20, 35, 50, 35]

last_week = [2, 3, 5, 8, 4, 4, 6, 2]
total_price = 0

for price in prices:
  total_price += price

average_price = total_price / len(prices)
print("Average Haircut Price: " + str(average_price));

new_prices = [price - 5 for price in prices]
print(new_prices);

total_revenue = 0
 
for i in range(len(hairstyles)):
  total_revenue += prices[i] * last_week[i]
  print("Total Revenue: " + str(total_revenue));
  
average_daily_revenue = total_revenue / 7
print(average_daily_revenue);

cuts_under_30 = [ 
hairstyles[i]
for i in range(len(hairstyles)) 
if new_prices[i] < 30
]

print(cuts_under_30);


```
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
