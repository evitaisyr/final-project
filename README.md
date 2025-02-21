## Research Question
Which statistical metrics (MOV, SRS, ORtg, DRtg, Pace) are most predictive of win percentage? Does defensive rating (DRtg) have a significant impact on team success in the NBA and WNBA? Are these relationships similar across both leagues?

## Project Framework
This analysis aims to determine the statistical factors that best predict team wins in NBA and WNBA. Also, I will do in depth analysis on whether defense (DRtg) is a significant factor in both the NBA and WNBA. Specifically, I will:

Calculate Win Percentage (WL%) for all NBA and WNBA teams across three seasons 2022-24.
Visualize Relationships between key metrics (MOV, SRS, ORtg, DRtg, Pace) and team success (WL%).
Perform Correlation Analysis to identify the strongest predictors of success.
Conduct Regression Analysis to quantify which metric impacts win percentage the most.
Include an Interactive Component that allows users to chose a team and see whether they over or underperformed vs the model (actual wins vs predicted wins).

## Visualizations
1) Correlation Heatmap: Metrics vs. Wins
   Which stat has the strongest positive correlation with wins?
   Compare NBA vs. WNBA to see if the same metrics are predictive in both leagues

2) Scatter Plot: DRtg vs. Wins (with Trend Line)
   Do better defensive teams (lower DRtg) tend to win more games?
   Compare NBA vs. WNBA to see if defense is equally important in both leagues

3) Bar Chart: DRtg by Team (Best & Worst Defenses)
   Are the best defensive teams also the most successful?
   Sort teams by lowest (best) and highest (worst) DRtg. & compare their (WL%)
   
4) Regression Model: Predicting Wins from Key Metric
   Compare NBA vs. WNBA to see if this metric is more important in one league

5) Analyze Residuals from the Regression Model
   Compare NBA vs WNBA residuals and show top and bottom outliers 
   
6) Interactive Features:
   Chose a team and season to see how they performed vs the model
   Select a season for that team and adjust their MOV to see how this impacts wins
