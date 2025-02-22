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

# Dependencies

Ensure you have the following libraries before running the scripts:

pip install pandas matplotlib seaborn

## Dataset

The dataset has several null values. But we don't need to drop any row with null values in this case or fill any null values as it affect the data.

<img width="706" alt="Screenshot 2025-02-22 at 11 00 03 PM" src="https://github.com/user-attachments/assets/2fb91350-2f0c-4fd7-b978-fb9bf9a6aa85" />

## Plot 1

<img width="872" alt="Screenshot 2025-02-22 at 11 00 38 PM" src="https://github.com/user-attachments/assets/76e865ff-6d15-49a3-ba14-ef6ecf957b17" />

The above plot shows the run distribution per over for both teams. Here are some insights:

1. The scoring rate for each team shows fluctuations throughout their inning, with spikes indicating overs with high scoring, likely due to boundaries or big hits.
2. Royal Challengers Bangalore(RCB) appears to have a couple of overs with significantly higher runs, suggesting aggressive batting.

## Plot 2

<img width="935" alt="Screenshot 2025-02-22 at 11 00 59 PM" src="https://github.com/user-attachments/assets/09eed65d-5b84-4dfc-8c12-25dba1405efb" />

Key Oservations from the above graph include:

1. **AR Patel** from Delhi Capitals is the top scorer of the match, significantly outscoring others with a littel over 50 runs.
2. **RM Patidar** is the top scorer for Royal Challengers Bangalore, closely approaching 50 runs.
3. The graph display diverse contribution from both teams, with several players from both sides contributing notable scores.


