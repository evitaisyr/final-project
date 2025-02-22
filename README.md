## Research Question
Which statistical metrics (MOV, SRS, ORtg, DRtg, Pace) are the strongest predictors of win percentage (WL%) in the NBA and WNBA? Specifically, how significant is Defensive Rating (DRtg) in determining team success? Do these relationships differ between the two leagues?

## Project Framework
This analysis aims to determine the statistical factors that best predict team wins in NBA and WNBA. Additionally, I will conduct an in-depth analysis of whether defense (Defensive Rating, DRtg) is a significant factor in both leagues. Specifically, this project includes:

Calculate Win Percentage (WL%) for all NBA and WNBA teams across three seasons 2022-24.
Visualize Relationships between key metrics (MOV, SRS, ORtg, DRtg, Pace) and team success (WL%).
Perform Correlation Analysis to identify the strongest predictors of success.
Conduct Regression Analysis to quantify which metric has the greatest impact on win percentage.
Perform a Residual Analysis to evaluate how well the regression model fits each team's performance.

Include an Interactive Component: 1) Select a team and see if they overperformed or underperformed based on actual vs. predicted wins. 2) Adjust a team’s margin of victory (MOV) to observe how it would impact their predicted win total.

## Visualizations
1) Correlation Heatmap: Metrics vs. Wins
   Objective: Identify which team statistics have the strongest correlation with win percentage (WL%).
   Insight: Helps determine if the same metrics (e.g., MOV, SRS, ORtg, DRtg) are equally predictive in the       NBA and WNBA.
   Visualization: Two heatmaps comparing the correlation of different stats with WL% in the NBA and WNBA.
   
2) Scatter Plot: DRtg vs. Wins (with Trend Line)
   Objective: Investigate whether teams with better defensive ratings (lower DRtg) tend to win more games.
   Insight: Compare NBA vs. WNBA to assess if defense plays a similar role in both leagues.
   Visualization: Two scatter plots with trend lines showing the relationship between DRtg and WL%.
   
3) Bar Chart: DRtg by Team (Best & Worst Defenses)
   Objective: Determine if the best defensive teams (lowest DRtg) are also the most successful.
   Insight: Compare the best and worst defensive teams’ DRtg alongside their win percentage (WL%).
   Visualization: Bar charts ranking teams by DRtg with WL% displayed above each bar.
   
4) Regression Model: Predicting Wins from MOV
   Objective: Use regression analysis to predict team wins based on their margin of victory (MOV).
   Insight: Determine how well MOV predicts success and compare its impact in the NBA and WNBA.
   Visualization: Scatter plots with regression lines showing actual wins vs. predicted wins.

5) Residual Analysis: Overperforming vs. Underperforming Teams
   Objective: Analyze residuals from the regression model to identify teams that overachieved or                            underachieved.
   Insight: Compare NBA vs. WNBA residuals and highlight the largest over- and underperformers.
   Visualization:
            Scatter plot of predicted wins vs. residuals, marking top and bottom outliers.
            Histogram of residuals to show overall model fit.
   
6) Interactive Feature: Team Performance vs. Model
   * Objective: Allow users to explore a specific team’s performance compared to the model’s predictions.
   * Features: Select a team and season to see their actual vs. predicted wins.
             Adjust the team's Margin of Victory (MOV) to see how it would change their predicted wins.
   * Visualization: Scatter plot highlighting the selected team’s position and a text-based summary.

   ## Conclusions
   Graph 1: Correlation Heatmaps (NBA & WNBA)
   * MOV (Margin of Victory) and SRS (Simple Rating System) are the strongest predictors of WL% in both the        NBA and WNBA, with correlations above 0.96.
   * DRtg (Defensive Rating) has a weaker correlation with wins (-0.67 in the NBA, -0.78 in the WNBA) which        suggests defense plays a more important role for wins in the WNBA       
   * Pace has little to no correlation with winning, meaning a faster or slower style of play does not             necessarily translate to more wins.
   Key takeaway: While defense (DRtg) is somewhat important, offensive and overall efficiency (MOV, SRS,         ORtg) are more strongly associated with winning in both leagues.
   

