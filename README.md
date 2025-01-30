# Supply-Chain-Optimization
Capacitated Plant Location Optimization


This project utilizes linear programming to solve a capacitated plant location problem, considering various costs (variable, fixed, freight, storage), 
emissions, and delivery constraints across multiple locations.
A linear programming model is developed to identify the minimum total costs for meeting consumer demand across five states, taking into account 
both low and high capacity plants along with various constraints.
The objective is to minimize the total cost while ensuring all demand and capacity constraints are met.

Features:

1.Cost Minimization: The model optimizes for total costs, considering fixed, variable, storage, and freight costs.
2.Production and Delivery: Determines the optimal production and delivery quantities for each location to minimize costs.
3.CO2 Emissions Constraints: Includes a constraint to ensure that CO2 emissions from production do not exceed a specified limit for each region.
4.Delivery Deadlines: The model respects delivery lead times and deadlines.
5.Multiple Scenarios: Can handle different scenarios, such as outsourcing to low-cost regions and adjusting for increased freight costs due to container shortages.

The output includes:

1.Total Costs: The total optimized cost per month.
2.Production and Plant Decisions: The optimal production and plant decisions for each location, in terms of units produced and whether the plant is active.
3.Production Summary: A summary of production quantities per location.
4.Visualizations: Plots of production scenarios to visualize different strategies, like outsourcing to low-cost regions.

Assumptions made for additional data:

1.Storage costs are 10% of fixed costs per year. So taking 10% of fixed costs and dividing by 30 (fixed costs are given per month) 
  to get the storage costs per unit per day.

2.Assuming vehicles run on diesel. 52 g of Carbon dioxide is release per metric ton for each kilometer travelled.


3.The following are the states considered for shipping:

1. New York(NY)
2. New Jersey(NJ)
3. Philadelphia(PA)
4. Massachusetts(MA)
5. New Hampshire(NH)

4.Assuming a standard delivery lead time of 3 days between the same state, delivery lead times of each location is taken 
based on the average time taken to go from 1 of the above state to the other.
Reference code:
https://github.com/samirsaci/supply-chain-optimization
