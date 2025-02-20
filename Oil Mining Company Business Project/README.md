## Telecom Interconnect Churn Project

## Introduction
You work for the OilyGiant mining company. Your task is to find the best place for a new well.

## Description
Steps to choose the location:

- Collect the oil well parameters in the selected region: oil quality and volume of reserves
- Build a model for predicting the volume of reserves in the new wells
- Pick the oil wells with the highest estimated values
- Pick the region with the highest total profit for the selected oil wells
- You have data on oil samples from three regions. Parameters of each oil well in the region are already known.
- Build a model that will help to pick the region with the highest profit margin.
- Analyze potential profit and risks using the Bootstrapping technique.

## Conclusion
<b> Preparing the Data </b>

- Although there was no full row duplicates, there were duplicate ids that we had to remove.
- The id column will be dropped, as we do not need this for the model training.
- Region 1 and 3 had very similar distributions in their data, while Region 2 had low outliers and high outliers.

<b> Model Training </b>

The results show that:
- Region 1 has an RSME of about 37.82 and average volume of 92.39
- Region 2 has an RSME of about 0.89 and average volume of 69.36
- Region 3 has an RSME of about 39.96 and average volume of 95.09

From these results we can say that:
- Region 3 has the worst RSME and the average volume is higher than Region 1 and 2, which shows that the model inaccurately predicted volumes of the new wells compared to the other 2 regions
- Region 1 and 3 have very similar results of RSME and average volume which shows that these models have very similar predictions
- However Region 2 did show the best results and that gives us an idea of what model we should move forward with

<b> Profit Calculation Preparation </b>

- All of our conditional constant variables are set.
- An average volume of 111.11 is needed to garner profit from this project.

<b> Profit Calculation </b>

Based on the calculations we have:
- Region 1 has a profit of about \$33,318,619.
- Region 2 has a profit of about \$24,150,866.
- Region 3 has a profit of about \$28,213,466.

Region 1 shows promise of being the region of choice for our project.

<b> Bootstrapping Technique for Profit and Risk </b>

The results of our bootstrapping technique show that:

- Region 1 has the 2nd most average profit, as well as the 2nd highest risk of losses.
- Region 2 has the best average profit, as well as the lowest risk of losses.
- Region 3 has the least amount of profit, as well as the highest risk of losses.

We can see that average profit and risk of losses are correlated as the more profit you have, the less likely the risk of losses are.

The confidence interval of Region 2 also is the most narrow which shows results are much more consistent for this region.

From these results, Region 2 will be the area where we would decide to do our project on.

<b> Overall Conclusion </b>

From the results that were garnered, I would have to say that Region 2 would be the ideal candidate for the project as they have, on average, the most profit as well as the least amount of risk involved and the most narrow confidence interval.
