# IPL-2024-Analysis

# Overview
This project analyzes the IPL 2024 match between Royal Challengers Bengaluru (RCB) and Delhi Capitals (DC) using Python. It provides insights into team performance, batting, bowling, partnerships, and match phases through various data visualizations.

## IPL 2024 RCB Vs DC Analysis: Dataset

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

## Features

The project performs multiple analyses and visualizations using Pandas, Matplotlib, and Seaborn.

1. **Run Distribution Per Over**
Plots the total runs scored per over for both teams.
Uses a line plot to visualize scoring trends.

2. **Top Scorers Analysis**
Identifies the highest run-scorers from each team.
Displays a bar chart comparing individual contributions.

3. **Bowling Performance Analysis**
Calculates economy rate (runs conceded per over) for each bowler.
Displays wickets taken and economy rates using bar and line plots.

4. **Dismissal Types**
Analyzes how batters got out.
Uses a pie chart to visualize different modes of dismissals.

5. **Batting Partnerships**
Calculates significant partnerships (20+ runs).
Uses a bar plot to highlight top partnerships.

6. **Match Phase Analysis**
Divides the match into Powerplay (0-6 overs), Middle Overs (7-15), and Death Overs (16-20).
Analyzes run rates and wickets lost in each phase.

7. **Batter Strike Rate Calculation**
Computes strike rates of batters based on runs scored and balls faced.

## Dependencies

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

## Polt 3

<img width="1001" alt="Screenshot 2025-02-22 at 11 01 27 PM" src="https://github.com/user-attachments/assets/7b26ed6b-f733-4204-8d25-381f1a773188" />

The combined bar and line plot provides a comprehensive overview of the bowling performance of each team:

1. **Wicket Taken**: The bars indicate the numbers of wickets each bowler took during the match. The height of the bars reflects how succesful the bowlers were in terms of taking wickets. Bowlers from both teams contributed to taking wickets, with some notable performances that stand out due to higher bars.

2. **Economy Rate**: The line graph overlaid on the bar graph shows the economy rate(number of runs conceded per over) of each bowler. The economy rate is crucial as it indicates how economically a bowler has bowled in terms of runs given away. 

## Plot 4

<img width="559" alt="Screenshot 2025-02-22 at 11 01 59 PM" src="https://github.com/user-attachments/assets/022ded80-281a-47fa-9a2e-0ad6057b2a70" />

This above pie chart graph analyze the type of dimissals that occured during the match to understand how most wickets were taken(e.g., caught, bowled, run out). This can provide insights into nature of pitch and the playing conditions.

## Plot 5

<img width="841" alt="Screenshot 2025-02-22 at 11 02 29 PM" src="https://github.com/user-attachments/assets/7035d4f9-5eba-48d2-bf32-b5c354656284" />

The above graph performs partnerships Analysis by calculating and visualizing the most productive batting partnership in match. We'll look at runs scored per partnership and how long each partnership lasted in terms of balls faced:
The bar chart displays significant batting partnerships from the match, highlighting partnerships that scored more than 20 runs. Here's how these insights contribute to our analysis:

1. The chart identifies key partnerships that likely had a substantial impact on the match's outcomes, effectiveness of batting pairs.

2. It provides insights into which players were involved in pivotal stands, which can help in assessing player forms and team strategy.

## Plot 6

<img width="841" alt="Screenshot 2025-02-22 at 11 02 42 PM" src="https://github.com/user-attachments/assets/270b468e-bc35-4594-bb2b-3fb78627d4af" />


