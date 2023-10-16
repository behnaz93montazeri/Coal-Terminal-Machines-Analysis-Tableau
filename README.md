# Coal-Terminal-Machines-Analysis-Tableau
## Project Description:

This project, inspired by a course on Udemy taught by Kirill Eremenko, aims to optimize the utilization of heavy machinery at a coal terminal using Tableau for data analysis and visualization. The primary goal is to identify which coal reclaimer machines require maintenance in the upcoming month to minimize downtime and associated revenue losses. The criterion for maintenance is based on the idle capacity of the machines.

## Project Challenge:

*Determine maintenance needs for machines that operate 24/7, with downtime costing millions of dollars.
*Maintenance required when there is an 8-hour period in the month with an average idle capacity exceeding 10%.
*Idle capacity is calculated using the formula: 
                          (Actual Tonnage - Nominal Capacity) / Nominal Capacity


## Three types of machines are considered in the project: 
                              Stackers, Reclaimers, and Stacker-Reclaimer machines.

## Challenges with the Dataset:

*Multiple sheets with data for different machines and varying dates.
*A solution involved creating a reference sheet with all dates for the specific month being analyzed.
*Utilized left joins to join all data sheets to the reference sheet.
*Calculated idle capacity using Tableau table calculations.

## Visualization and Analysis:

*A threshold of 10% idle capacity was set as a reference line.
*A calculation was used to convert negative idle capacity values to positive values using calcaution field for clarity.
*An 8-hour moving average was applied to analyze machine performance.
*Trendlines with p-values were used to identify maintenance needs.

Machine-Specific Insights:

*RL1 machine requires maintenance due to significant spikes in performance.
*RL2 and SR1 machines do not require immediate maintenance. However, the prediction cannot be accurate for the SR1 machine, since the p-value is above 0.05
*SR4A machine, although not needing maintenance this month, is likely to require maintenance in the coming month based on the trendline.
*SR6 machine exhibits a similar spike as RL2, possibly due to alternating machine operation.
