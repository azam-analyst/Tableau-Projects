## Sales Lead Data Analysis 

This is a project done to analyse and visualize sales lead performance data of the inbound sales teams of a company whithin health tech industry. The company provides B2B trainning platform to the fitness experts/trainners to interact with their clients and provide tutorials and lesson on the same platform. The service is provided on subscription basis.

# Business Problem:

The manager wants to have an indepth analysis of the performance of sales teams across four countries in Europe. There is a requirememnt of two dashboards. One with a general quarterly performance overview and another one with the visualization of sales team performance that can be use by sales teams to track their sales records. Th business problems are as following-

1. Create an overview dashboard that can be used by the manager to monitor performance of the whole team during the month and report on the performance at the end of the month. Business metrices shall be aggregated to justify the performance as team from the countries they are working. Make general overview from different charts used in the dashboard. 

2. Create a dashboard that allows salespeople to see updates when they make a sale.Create relevent KPIs which can be tracked to mesure sales lead performances of the teams and of the sales reps individually.

3. Make assumtions whre necessary with managerial recommendations on the scope of improvement that could lead to better sales rep performance eventually more customer acquisition.


## Monthly overview dashboard
Data Analysis procedures:
1. The dataset was in xlsx format and was imported in Tableau Desktop for analysis. 
2. Sales KPIs were  with Tableau calculated fields to mesure performance: # of leads created,# of leads won,lead flow, lead conversion rate, average sales cycle time.
3. Overall the the lead creation increased in a very good extent in March thus showing a upward trend in the performance of the teams. 
4. Lead flow was the highest in UK meaning UK sales reps were in discussion with highest number of clients

KPI calculation in Tableau:
# of leads created:
In order to track the number of leads created a new caluclate field was created as following:

COUNT(IF [Lead State]="CONTACTED" THEN [Lead Id] END)

# of Leads won:
COUNT(IF [Lead State]="WON" THEN [Lead Id] END)

Lead conversion rate:
The KPI is created to track the conversion rate which calculates the percentage of leads won compared to the percentage of leads created.

Tableau field:
[# of Leads Won]/[# of Leads Created]

Avergae Sales Cycle time:
The sales cycle time measures the time between lead creation and lead winning date. The more less the cycle time the more efficient are the sales team on winning leads thus creating profitability.

Tableau Field:
DATEDIFF('day',[Lead Creation Date],[Lead Winning Date])

Lead Flow:
The number of leads the sales team are working. This KPI field can be created by counting the number of 'In Dialogue' fields on Lead State column.
Tableau calculated field:
COUNT(IF [Lead State]="In Dialogue" THEN [Lead Id] END)

# Final Dashboard:

6. <img width="802" alt="Sales Lead Dashboard" src="https://user-images.githubusercontent.com/96620728/174909369-7afe1235-a26a-4e85-80d4-2fc2208885c2.png">

## Sales lead performance dashboard:

From the dashboard dynamic filters can be used to track each team and each sales rep performance based on the states of the leads and KPis used to track the performance. Overall in the month of March the sales reps performance was at peak with highest number of leads won compared to february and January.

<img width="802" alt="Sales Team Performance Dashboard" src="https://user-images.githubusercontent.com/96620728/174909599-f8c19057-3aba-4446-b147-eaac96ab7c47.png">

Assumptions and recommendations for improvement on sales lead performances:

#Sales cycle time:
The sales cycle time which referes to the timeframe between a sales lead creation and sales lead winning was highest for Sales rep 5,sales rep 2 from Team 2 of UK.
High sales cycle time is an indication where sales reps spending too much time on individual clients or the clients are not being communicated effectively.

Assuming possible reasons:.
* Wrong target customers who might not were good fit for the product.
* Ineffective way of product presentation in first meeting.

#Possible steps for improvement:
*Have an indepth analysis of the sales cycle stages.
*Deciding if a customer has the affordability or is the right fit for the product before contacting.
* Improving first sales meeting strategies as most conversion rate depends a lot on first meting

#Team lead performance major insght :
Team 2 Working in UK created highest leads compared to others but the lead conversion rate was the lowest.

Managerial steps can be taken by
Going in depth about  the lead lost reason and trying to improve on that or give enhanced trainning to  representatives.
Finding out the possible lead  the reps are actually contacting or and judge if are actually a  good fit  to product or the right customer.

Overall, The sales lead performance was improved in a very good extent in March.leads creation numbers were going up, lead flow number were highest, more number of leads were won than previous two months. 
