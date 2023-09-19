<h1 align="center"> Quantium Data Analytics Job Simulation - Chip Category Retail Customer Insights and Uplift Testing </h1>

<p align="center">
  <img src="https://www.thedailymeal.com/img/gallery/the-easy-trick-to-make-your-potato-chip-bowl-look-prettier/intro-1670424312.jpg">
</p>

[Link to Quantium Job Simulation](https://www.theforage.com/virtual-internships/prototype/NkaC7knWtjSbi6aYv/Data%20Analytics)\
[Link to the Cetification](https://forage-uploads-prod.s3.amazonaws.com/completion-certificates/Quantium/NkaC7knWtjSbi6aYv_Quantium_dDsCRiLXErJmXtsZq_1695113047859_completion_certificate.pdf)\
[Link to the full code hosted on Colab](https://colab.research.google.com/drive/1_Mqvokfsx44iz-JvQEonRlbmG5M19QcX?authuser=1#scrollTo=9e559275-2332-4846-b26b-dc0eba840817)

**The program includes 3 tasks:**
- Task 1: Data Preparation and Customer Analytics
- Task 2: Experimentation and uplift testing
- Task 3: Analytics and commercial application

## [Task 1: Data preparation and customer analytics](https://github.com/EveTLynn/Data-Science-Projects/blob/main/Quatium-Retails-Analytics-Job-Simulation/Quantium%20-%20task%201%20-%20customer%20analytics.ipynb)
### 1.1. Background information
Quantium’s retail analytics team and have been approached by a client, the Category Manager for Chips, who wants to better understand the types of customers who purchase Chips and their purchasing behaviour within the region. The insights from the analysis will feed into the supermarket’s strategic plan for the chip category in the next half year.

**Main tasks**
- Examine transaction data – look for inconsistencies, missing data across the data set, outliers, correctly identified category items, numeric data across all tables. 
- Examine customer data – check for similar issues in the customer data, look for nulls and when you are happy merge the transaction and customer data together.
- Data analysis and customer segments – define the metrics – look at total sales, drivers of sales, where the highest sales are coming from etc. Explore the data, create charts and graphs as well as noting any interesting trends and/or insights.
- Deep dive into customer segments – define your recommendation from insights, determine which segments we should be targeting, if packet sizes are relative and form an overall conclusion based on your analysis.

### 1.2 Key findings
Sales plummeted in mid-August 2018 and mid-June 2019. Sales peaked for a short period before Christmas and there was no sale on the 25th of December. This may due to shops were closed on Christmas day.

![Total Sales of all store over one year](https://github.com/EveTLynn/Data-Science-Projects/blob/main/Quatium-Retails-Analytics-Job-Simulation/Charts/total%20sales%20line%20plot.png)

Older customers spend more on chips with roughly 60% of sales. Mainstream type take up the largest proportion with nearly 40% of overall sales.

![Sales pie chart](https://github.com/EveTLynn/Data-Science-Projects/blob/main/Quatium-Retails-Analytics-Job-Simulation/Charts/piesales.png)

- For the Young Singles/Couples, Midage Singles/Couples and Retirees: Mainstream type is the majority.
- Young Families amd Older Families seemed to prefer to be on budget. OLDER SINGLES/COUPLES have pretty the same sales regardless of member type.
- Budget Older Families, Mainstream Retirees, Mainstream Young Singles/Couples are 3 group with the most sale

![Sales bar chart](https://github.com/EveTLynn/Data-Science-Projects/blob/main/Quatium-Retails-Analytics-Job-Simulation/Charts/barsales.png)

Kettle wins by a big margin as customer's favorites chips. Doritos, Smiths and Pringles also had good sales. The company maybe should concentrate more on these product and drop other low-sale one such as Burger, French, Sunbites, Cheetos and CCs.

![Brand bar chart](https://github.com/EveTLynn/Data-Science-Projects/blob/main/Quatium-Retails-Analytics-Job-Simulation/Charts/brand.png)

## [Task 2: Experimentation and uplift testing](https://github.com/EveTLynn/Data-Science-Projects/blob/main/Quatium-Retails-Analytics-Job-Simulation/Task%202%20-%20Experimentation%20and%20Uplift%20Testing.ipynb)
### 2.1. Background information
The clients want to test the impact of the new trial layouts with a data driven recommendation to whether or not the trial layout should be rolled out to all their stores. We will evaluate the performance of a store trial which was performed in stores 77, 86 and 88 and examine the performance in trial vs control stores to provide a recommendation for each location based on our insight.

**Main task**
- Select control stores – explore the data and define metrics for control store selection
  - Think about what would make them a control store
  - Look at the drivers and visualise these in a graph to better determine if they are suited
  - Write a function to reduce having to re-do the analysis for each trial store:  using Pearson correlations and magnitude distance
- Assessment of the trial – this one should give you some interesting insights into each of the stores
  - Check each trial store individually in comparison with the control store to get a clear view of its overall performance.
  - We want to know if the trial stores were successful or not: test if total sales are significantly different in the trial period and if so, check if the driver of change is more purchasing customers or more purchases per customers etc.
- Collate findings – summarise your findings for each store and provide an recommendation outlining the impact on sales during the trial period.

### 2.2 Key findings
Control store is seleted by:
- Comparing Monthly Sales and Monthly Customer
- From 2018-07-01 to 2019-06-30 (before the trial period)
- Based on Pearson’s correlation and Magnitude difference

Control stores for Trial stores 77, 86 and 88 is store 233, 155 and 237 respectively

The 3 store saw a statistically significant increase in Total Sales and Number of Customers visit for at least one month during the 3 months trail period of new layout. After the trial the Sales and Number of Customers is not statistically different from the control stores.\
Here is chart of one out of 3 trial stores showing the sales increase in the trial period.

![Trial vs control store](https://github.com/EveTLynn/Data-Science-Projects/blob/main/Quatium-Retails-Analytics-Job-Simulation/Charts/sales77.png)

## [Task 3: Analytics and commercial application](https://github.com/EveTLynn/Data-Science-Projects/blob/main/Quatium-Retails-Analytics-Job-Simulation/Task%203%20-%20Analytics%20and%20commercial%20application.pdf)
- Sales before Christmas peaked at 7000 bags of chips. Company need adequate supply and may implement promotions at this period
- Budget Older Families, Mainstream Retirees, Mainstream Young Singles/Couples are the main buyers. Focus on their preferences and generate more sales
- Kettle drives the most sales. Have enough stock of Kettle and consider replace/ drop low sales brands
- All 3 trail stores experienced increase in sales and number of customers for at least one month of the trial period for new store layout
- After the trial, all trial stores’ sales and number of customers are not statistically different from control stores. Further information on other changes during the trial period is needed to dive deeper
