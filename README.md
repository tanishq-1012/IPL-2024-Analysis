# 🏏 IPL-2024-Analysis

## Overview
This project analyzes the IPL 2024 match between Royal Challengers Bengaluru (RCB) and Delhi Capitals (DC) using Python 🐍 . It provides insights into team performance, batting, bowling, partnerships, and match phases through various data visualizations.

## IPL 2024 RCB Vs DC Analysis: Dataset

The 📁 dataset we collected for this IPL match analysis contains the following columns:

1. `teams`: Indicates the batting team.
2. `over`: Over number in the match.
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

## Dataset 📁

The dataset has several null values. But we don't need to drop any row with null values in this case or fill any null values as it affect the data.

<img width="706" alt="Screenshot 2025-02-22 at 11 00 03 PM" src="https://github.com/user-attachments/assets/2fb91350-2f0c-4fd7-b978-fb9bf9a6aa85" />

## Plot 1 📊

<img width="872" alt="Screenshot 2025-02-22 at 11 00 38 PM" src="https://github.com/user-attachments/assets/76e865ff-6d15-49a3-ba14-ef6ecf957b17" />

The above plot shows the run distribution per over for both teams. Here are some insights:

1. The scoring rate for each team shows fluctuations throughout their inning, with spikes indicating overs with high scoring, likely due to boundaries or big hits.

2. Royal Challengers Bangalore(RCB) appears to have a couple of overs with significantly higher runs, suggesting aggressive batting.

## Plot 2 📊

<img width="935" alt="Screenshot 2025-02-22 at 11 00 59 PM" src="https://github.com/user-attachments/assets/09eed65d-5b84-4dfc-8c12-25dba1405efb" />

Key Oservations from the above graph include:

1. **AR Patel** from Delhi Capitals is the top scorer of the match, significantly outscoring others with a littel over 50 runs.

2. **RM Patidar** is the top scorer for Royal Challengers Bangalore, closely approaching 50 runs.

3. The graph display diverse contribution from both teams, with several players from both sides contributing notable scores.

## Polt 3 📈

<img width="1001" alt="Screenshot 2025-02-22 at 11 01 27 PM" src="https://github.com/user-attachments/assets/7b26ed6b-f733-4204-8d25-381f1a773188" />

The combined bar and line plot provides a comprehensive overview of the bowling performance of each team:

1. **Wicket Taken**: The bars indicate the numbers of wickets each bowler took during the match. The height of the bars reflects how succesful the bowlers were in terms of taking wickets. Bowlers from both teams contributed to taking wickets, with some notable performances that stand out due to higher bars.

2. **Economy Rate**: The line graph overlaid on the bar graph shows the economy rate(number of runs conceded per over) of each bowler. The economy rate is crucial as it indicates how economically a bowler has bowled in terms of runs given away. 

## Plot 4 📈

<img width="559" alt="Screenshot 2025-02-22 at 11 01 59 PM" src="https://github.com/user-attachments/assets/022ded80-281a-47fa-9a2e-0ad6057b2a70" />

This above pie chart graph analyze the type of dimissals that occured during the match to understand how most wickets were taken(e.g., caught, bowled, run out). This can provide insights into nature of pitch and the playing conditions.

## Plot 5 📉

<img width="841" alt="Screenshot 2025-02-22 at 11 02 29 PM" src="https://github.com/user-attachments/assets/7035d4f9-5eba-48d2-bf32-b5c354656284" />

The above graph performs partnerships Analysis by calculating and visualizing the most productive batting partnership in match. We'll look at runs scored per partnership and how long each partnership lasted in terms of balls faced:
The bar chart displays significant batting partnerships from the match, highlighting partnerships that scored more than 20 runs. Here's how these insights contribute to our analysis:

1. The chart identifies key partnerships that likely had a substantial impact on the match's outcomes, effectiveness of batting pairs.

2. It provides insights into which players were involved in pivotal stands, which can help in assessing player forms and team strategy.

## Plot 6 📉

<img width="841" alt="Screenshot 2025-02-22 at 11 02 42 PM" src="https://github.com/user-attachments/assets/270b468e-bc35-4594-bb2b-3fb78627d4af" />

The plot above provides a clear breakdown of the match into different phases; Powerplay, Middle, and Death, and illustrate how each team performed during these segments:

1. **Powerplay**: Both teams have a relatively low total of runs, with RCB losing more wickets than DC in this phase, as indicated by the height of orange line.

2. **Middle**: This phase shows the higest run-scoring for both teams, with DC scoring slightly more than RCB. The wickets lost remain controlled, suggesting stable innings from both teams.

3. **Death**: RCB has a sharp decreasein runs compared to the middle phase, while DC maintains a high run rate. Wickets lost by RCB increased significantly in this phase, marked by the orange line peaking near 4.5, indicating a possible collapse or aggressive batting that did not pay off.

## Plot 7(Data) 📁

<img width="382" alt="Screenshot 2025-02-22 at 11 06 28 PM" src="https://github.com/user-attachments/assets/02251b3b-5809-49f8-afba-45c8f14d861e" />

Now, let’s calculate the strike rates for all batters in this match and then analyze the data to see which players were the most effective in terms of scoring quickly. After calculating the strike rates, we can look at correlations with other variables such as runs scored or the phase of play during which the runs were scored. This can give us insights into which players accelerate scoring at crucial times or against specific bowlers.

Here are the top performers in terms of strike rate from the match:

1. **J Fraser-McGurk** had the highest strike rate at 262.50, scoring 21 runs from just 8 balls.
2. **Virat Kohli** also scored efficiently, with a strike rate of 192.86, making 27 runs from 14 balls.
3. **Rajat Patidar** contributed significantly with a strike rate of 152.94, accumulating 52 runs from 34 balls.

## Plot 8 📊

<img width="765" alt="Screenshot 2025-02-24 at 5 17 29 PM" src="https://github.com/user-attachments/assets/dfc9d7b3-a49d-4279-a206-efdad448577e" />

Now, let’s dive deeper by looking at how the strike rate varied with the phase of the game for these top performers. It could give insights into strategic scoring and game dynamics during different innings stages:

The bar chart illustrates how the strike rates of the top performers varied across different phases of the match:

**J Fraser-McGurk** stands out with a particularly high strike rate in the Middle phase, significantly higher than any other phase or player, suggesting a highly aggressive and effective batting performance during this part of the innings.

**V Kohli** and **RM Patidar** both have high strike rates in the Death phase, indicating their ability to accelerate scoring towards the end of the innings, which is crucial for setting or chasing targets.

**AR Patel** shows consistency in the Powerplay and Middle phases with a slightly reduced but still competitive strike rate, indicating his role as a steady opener or middle-order batter.

**KV Sharma** exhibits a lower strike rate in the Middle phase compared to others, suggesting a more conservative approach during this phase or difficulty in accelerating.

## Plot 9 📊

<img width="851" alt="Screenshot 2025-02-24 at 5 17 51 PM" src="https://github.com/user-attachments/assets/d83f3aa3-9723-4afc-8b3c-3b1d96d09279" />

To identify the turning point where Delhi Capitals (DC) might have lost the game and Royal Challengers Bangalore (RCB) gained the upper hand, we can analyze the cumulative run rate comparison throughout the innings and look at wicket fall events. Specifically, we can:

**Compare Cumulative Run Rates**: Plot the cumulative run rates of both teams throughout their innings to see where RCB started to outpace DC significantly.

**Wicket Analysis**: Examine the timings and impacts of wicket falls on the scoring rate and momentum for DC.

**High-Impact Overs**: Identify any overs where RCB took multiple wickets or DC had a significantly low scoring rate, which could indicate a loss of momentum.

The plot shows the cumulative runs scored by each team throughout their innings, with markers indicating wickets:

**Momentum Shifts**: The points where wickets are lost are crucial. Despite wickets, RCB’s run line does not show any drastic downturns, suggesting effective recovery by subsequent batters.

**Performance Analysis**: RCB’s ability to keep the run rate up despite losing wickets might indicate deeper batting strength or successful innings pacing strategies. In contrast, DC, while also increasing their score, does so at a less steep rate, possibly indicating fewer big overs.

## Plot 10 📊

<img width="877" alt="Screenshot 2025-02-24 at 5 18 19 PM" src="https://github.com/user-attachments/assets/ca70ecaa-367a-494f-bbe9-63543ed958fb" />

Now, let’s calculate the run rate for each over for both teams and see how the run rates changed throughout the innings, particularly focusing on the overs where wickets fell:

The plotted run rates for each over, along with the moments when wickets were taken (marked with large dots), provide insights into how the match’s dynamics evolved:

**RCB Run Rate Fluctuations**: RCB’s run rate shows significant fluctuations, peaking at around 3.5 runs per ball towards the end of the innings. The presence of wicket markers (red circles) indicates that wickets were taken during overs where the run rate was generally lower, which is typical as wickets tend to disrupt batting flow.

**DC Run Rate Patterns**: DC’s run rate starts strong but sees a sharp decline after the initial overs, stabilizing somewhat in the middle before another peak and subsequent fall towards the end. Wickets (blue circles) are taken in overs where the run rate drops, suggesting effective bowling from RCB during these times.

# Summary

The match between RCB and DC showcased a blend of strategic batting, aggressive bowling, and critical partnerships. RCB’s ability to maintain a higher cumulative run rate and effective wicket-taking in crucial overs contributed significantly to their victory. The detailed phase-wise and player-specific analysis not only highlights the dynamics of T20 cricket but also assists in understanding how momentum shifts and strategic decisions impact the game’s outcome.


# Tech Stack

1.Python 🐍

2.Pandas (Data manipulation)

3.Matplotlib & Seaborn (Data visualization)

# Dataset 📁

The dataset innings_deliveries.csv contains ball-by-ball match data, including:

1.Batters, Bowlers & Non-strikers

2.Runs (batter, extras, and total)

3.Wickets & dismissal types

4.Overs & match phases

# Sample Visualization

📌 **Run Distribution Per Over**
📈 Compares the scoring pattern of RCB and DC.

📌 **Top Scorers**
🏏 Displays highest run-scorers from each team.

📌 **Bowling Performance**
🎯 Wickets taken & economy rate visualization.
