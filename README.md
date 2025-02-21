# IPL-2024-Analysis

# Overview
This project analyzes the IPL 2024 match between Royal Challengers Bengaluru (RCB) and Delhi Capitals (DC) using Python. It provides insights into team performance, batting, bowling, partnerships, and match phases through various data visualizations.

# IPL 2024 RCB Vs DC Analysis: Dataset

The  dataset we collected for this IPL match analysis contains the following columns:

1. teams: Indicates the batting team.
2. over: Over number in the match.
3. batter: The batsman facing delivery.
4. bowler: The bowler delivering the ball.
5. non_striker: The batsman at the non_striker's end.
6. runs_batter: Runs scored by the batter off the delivery.
7. runs_extras: Extra runs(like wides, no balls) were conceded during delivery.
8. run_total: Total runs scored from the delivery.
9. player_out: Name of the player out on the delivery(if any).
10. wicket_kind: Types of dismissal(if any).
11. filders: Names of the fielders involved in the dismissal(if any) 

# Features

The project performs multiple analyses and visualizations using Pandas, Matplotlib, and Seaborn.
1. Run Distribution Per Over
Plots the total runs scored per over for both teams.
Uses a line plot to visualize scoring trends.

2. Top Scorers Analysis
Identifies the highest run-scorers from each team.
Displays a bar chart comparing individual contributions.

3. Bowling Performance Analysis
Calculates economy rate (runs conceded per over) for each bowler.
Displays wickets taken and economy rates using bar and line plots.

4. Dismissal Types
Analyzes how batters got out.
Uses a pie chart to visualize different modes of dismissals.

5. Batting Partnerships
Calculates significant partnerships (20+ runs).
Uses a bar plot to highlight top partnerships.

6. Match Phase Analysis
Divides the match into Powerplay (0-6 overs), Middle Overs (7-15), and Death Overs (16-20).
Analyzes run rates and wickets lost in each phase.

7. Batter Strike Rate Calculation
Computes strike rates of batters based on runs scored and balls faced.
Displays the top 20 batters ranked by strike rate.

