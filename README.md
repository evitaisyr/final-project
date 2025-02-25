## Research Question
Which statistical metrics (MOV, SRS, ORtg, DRtg, Pace) are the strongest predictors of win percentage (WL%) in the NBA and WNBA? Specifically, how significant is Defensive Rating (DRtg) in determining team success? Do these relationships differ between the two leagues?

# NBA & WNBA Win Prediction Analysis
## Final Project Presentation

Click the link below to watch my final project presentation:
▶️ [Watch the Presentation](https://github.com/evitaisyr/final-project/raw/main/video1291189233.mp4)

## Project Framework
This analysis will determine the statistical factors that best predict team wins in the NBA and WNBA. Additionally, I will conduct an in-depth analysis of whether defense (Defensive Rating, DRtg) is a significant factor in both leagues. Specifically, this project includes:

* Calculate Win Percentage (WL%) for all NBA and WNBA teams across the 2022-24 seasons.
* Visualize relationships between key metrics (MOV, SRS, ORtg, DRtg, Pace) and team success (WL%).
* Perform Correlation Analysis to identify the strongest predictors of success.
* Compare statistical differences between high and low win percentage teams using T-Tests and box plots for    MOV and DRtg.
* Conduct Regression Analysis to quantify which metric has the greatest impact on win percentage.
* Perform a Residual Analysis to evaluate how well the regression model fits each team's performance.
* Include an Interactive Component:
  Select a team and see if they overperformed or underperformed based on actual vs. predicted wins.
  Adjust a team’s Margin of Victory (MOV) to observe how it would impact their predicted win total.

## Visualizations
1) Correlation Heatmap: Metrics vs. Wins
   * Objective: Identify which team statistics have the strongest correlation with win percentage (WL%).
   * Insight: Helps determine if the same metrics (e.g., MOV, SRS, ORtg, DRtg) are equally predictive in the       NBA and WNBA.
   * Visualization: Two heatmaps comparing the correlation of different stats with WL% in the NBA and WNBA.
   
2) Scatter Plot: DRtg vs. Wins (with Trend Line)
   * Objective: Investigate whether teams with better defensive ratings (lower DRtg) tend to win more games.
   * Insight: Compare NBA vs. WNBA to assess if defense plays a similar role in both leagues.
   * Visualization: Two scatter plots with trend lines showing the relationship between DRtg and WL%.
   
3) Bar Chart: DRtg by Team (Best & Worst Defenses)
   * Objective: Determine if the best defensive teams (lowest DRtg) are also the most successful.
   * Insight: Compare the best and worst defensive teams’ DRtg alongside their win percentage (WL%).
   * Visualization: Bar charts ranking teams by DRtg with WL% displayed above each bar.
  
4) Box Plot: MOV & DRtg Comparison for High vs. Low WL%
   * Objective: Compare how MOV (Margin of Victory) and DRtg (Defensive Rating) differ between high-win and       low-win teams in both leagues.
   * Insight: Determine if successful teams tend to have significantly higher MOV and lower DRtg.
   * Visualization: Four box plots (two for NBA, two for WNBA) showing MOV and DRtg distribution for high-        vs. low-win teams.
   
5) Regression Model: Predicting Wins from MOV
   * Objective: Use regression analysis to predict team wins based on their margin of victory (MOV).
   * Insight: Determine how well MOV predicts success and compare its impact in the NBA and WNBA.
   * Visualization: Scatter plots with regression lines showing actual wins vs. predicted wins.

6) Residual Analysis: Overperforming vs. Underperforming Teams
   * Objective: Analyze residuals from the regression model to identify teams that overperformed or         
     underperformed relative to expectations.
   * Insight: Compare NBA vs. WNBA residuals and highlight the largest over- and underperformers.
   * Visualization:
              Scatter plot of predicted wins vs. residuals, marking top and bottom outliers.
              Histogram of residuals to show overall model fit.
   
7) Interactive Feature: Team Performance vs. Model
   * Objective: Allow users to explore a specific team’s performance compared to the model’s predictions.
   * Features: Select a team and season to see their actual vs. predicted wins.
               Adjust the team's Margin of Victory (MOV) to see how it would change their predicted wins.
   * Visualization: Scatter plot highlighting the selected team’s position and a text-based summary.

## Conclusions from Visualizations
Graph 1: Correlation Heatmaps (NBA & WNBA)
   * MOV (Margin of Victory) and SRS (Simple Rating System) are the strongest predictors of WL% in both the       NBA and WNBA, with correlations above 0.96.
   * DRtg (Defensive Rating) has a weaker correlation with wins (-0.67 in the NBA, -0.78 in the WNBA). The        more negative number for the WNBA suggests defense plays a more important role for wins in this league.
   * Pace has little to no correlation with winning. Faster or slower style of play does not                      necessarily translate to more wins.
Key takeaway: While defense (DRtg) is somewhat important, offensive and overall efficiency (MOV, SRS, ORtg) are more strongly associated with winning in both leagues.

Graph 2: Scatter Plot – DRtg vs. Wins
   * There is a negative trend, meaning teams with lower DRtg (better defense) tend to win more games.
   * The relationship appears stronger in the WNBA than the NBA, suggesting defense might be slightly more        impactful in the WNBA.
Key takeaway: Better defense correlates with more wins, but it is not the sole determinant of success. Other factors, like offensive rating and overall team strength, also matter.

Graph 3: Bar Chart – Best & Worst Defensive Teams
   * Some of the best defensive teams (low DRtg) have high win percentages, but this is not always           
     consistent.
   * In both leagues, some teams with strong defenses still have low WL%, implying that defense alone is not      enough to guarantee success.
Key takeaway: The best teams tend to have strong defenses, but elite defense does not always lead to elite winning percentages.

Graph 4: T-Tests – MOV & DRtg Comparison for High vs. Low WL%
   * MOV is significantly higher for high-win teams in both the NBA and WNBA (p < 0.00001, large effect           size).
   * DRtg is significantly lower for high-win teams, especially in the WNBA (stronger effect size in WNBA).
   * MOV is the biggest differentiator between winning and losing teams, with a slightly stronger role in         the NBA.
   * Defense (DRtg) is more important in the WNBA than in the NBA, but offense (MOV) still dominates.
Key takeaway: MOV is the most significant differentiator between winning and losing teams in both leagues, reinforcing its role as the primary predictor of success. While DRtg plays a more important role in the WNBA than in the NBA, offensive dominance (MOV) remains the most consistent factor in determining team success across both leagues.

Graphs 5 & 6: Regression Model – Predicting Wins
  * The regression model confirms MOV is the strongest predictor of wins in both leagues, aligning with the      correlation heatmap.
  * Due to high correlations between MOV, SRS, ORtg and DRtg including multiple metrics would introduce          multicollinearity leading to unreliable estimates. MOV serves as a composite measure for both offense        and defense performance making it the best standalone predictor.
  * Scatter plots with regression lines visually confirm that teams with a higher MOV (winning margin) tend      to win more games.
  * The high R-squared values (~0.92 for NBA, ~0.91 for WNBA) indicate that MOV accounts for the vast            majority of variance in team wins.
Key takeaway: MOV is the most reliable predictor of wins across both leagues. By capturing both offensive and defensive dominance, it serves as the best single metric for forecasting success. Teams that consistently win by larger margins are more likely to sustain long-term success.

Graph 7 & 8: Residuals Analysis (NBA & WNBA)
   * Some teams overperformed or underperformed based on the regression model.
   * This suggests that external factors (coaching, injuries, player performance, luck) impact wins beyond        just statistical metrics.
Key takeaway: The model is strong, but not perfect—teams can exceed or fall short of expectations due to non-statistical factors.

Graph 9: Interactive Model Output
   * This allows users to adjust a team's MOV and see how it affects their predicted wins.
   * It demonstrates that increasing MOV leads to more wins, reinforcing that MOV is the best predictor of        success.
Key takeaway: A higher MOV translates directly into more wins, emphasizing that winning by larger margins is a sign of strong performance.

## Overall Conclusion
This analysis examined the relationship between key basketball metrics and team success in both the NBA and WNBA. The findings consistently highlight Margin of Victory (MOV) as the strongest predictor of win percentage (WL%), outperforming other metrics such as Defensive Rating (DRtg), Offensive Rating (ORtg), and Pace.

Key Findings:
1) MOV and SRS are the best predictors of wins in both leagues, with a correlation exceeding 0.96. This suggests that teams that consistently win by larger margins tend to sustain success.
2) Defensive Rating (DRtg) has a moderate correlation with wins but is not as strong as MOV. The relationship is slightly stronger in the WNBA than the NBA, indicating defense plays a larger role in team success in the WNBA.
3) Regression analysis confirms that MOV alone explains over 90% of the variance in team wins, reinforcing that both offensive and defensive efficiency contribute to winning.
4) T-Tests show that high-win teams have significantly higher MOV and lower DRtg than low-win teams.
5) Multicollinearity prevents including multiple similar metrics (MOV, SRS, ORtg, DRtg) in the regression model simultaneously because they are highly correlated. MOV serves as a composite metric that captures both offensive and defensive performance.
6) Residuals analysis highlights teams that overperformed or underperformed expectations, suggesting that external factors such as coaching, injuries, and roster changes also impact team success.
7) The interactive component demonstrates how adjusting a team’s MOV directly impacts predicted wins, further emphasizing MOV as the best standalone predictor of team performance.
   
Final Takeaway:
While defense (DRtg) is an important factor, the data consistently shows that MOV is the most reliable indicator of team success. Teams that consistently maintain a high MOV tend to achieve sustained success, making it the most reliable single metric for predicting wins in both leagues.

(All data is from basketball-reference.com and was scraped for 2022-24 seasons for both leagues for all teams)
