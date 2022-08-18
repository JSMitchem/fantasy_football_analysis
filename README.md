# 2021 Fantasy Football Analysis

## Motivation
  For my NSS Capstone project, I decided to do some technical analysis on the same topic I've been doing basic analysis on for 18 years - Fantasy Football

  Fantasy Football gives anybody the unique opportunity to compete with family or friends while simply sitting on your couch and spectating professional football.  As a kid I remember going to my grandparent's house every Sunday with all my cousins to watch football from noon until as late as our parents would allow us to stay.  We took many breaks during this time to go outside and play some 3 vs. 3 football ourselves.  We began our fantasy football league in 2003 between 6 cousins and my 4 uncles with a $10 buy in and the entire $100 prize pool being awarded to first place.  As we grew older, our fantasy football league got more intense with each passing year.  This upcoming season will be the 19th fantasy football season between our family and the prize pool has now grown to $1500 being rewarded to first place due to the buy in now being raised to a hefty $150.  I'm now in a few other leagues with my friends, but no league will ever matter to me as much as the one my family began almost 20 years ago.

#Data

Web Scraping
  [Pro Football Reference](https://www.pro-football-reference.com/years/2021/advanced.htm)
CSV Files
  [Advanced Sports Analytics](advancedsportsanalytics.com/nfl-raw-data)
  [Fantasy Pros](https://www.fantasypros.com/nfl/adp/ppr-overall.php)

#Main Questions

Which players were most consistent across the entire season while also being productive?
    -I solved this by first finding the standard deviation for each player across all 18 weeks.  I then divided the standard deviation by the mean to solve for the coefficient of variation.
    *Consistency = 100 - ((Standard Deviation / Mean) * 100)
What's a good way to value each player based on their position?
    -For this question, I based the solution on the fact that the average fantasy football league has 10 teams.  In a perfectly drafted league the 10 best performers at quarterback would be on every team.  We'll use the 10th best quarterback as the baseline comparison to compare to all other quarterbacks.  The baseline comparison for the positions in my project are the following: QB-10, RB-20, WR-20, TE-10
    *BL Comp = ((Player's points - Baseline player's points) / Baseline player's points) * 100)

#Power BI Dashboard
[Dashboard link](https://app.powerbi.com/view?r=eyJrIjoiNDg4ZjE4YjYtNDFiYS00OTk0LWI1MmItMTAxNjljMThlMTg5IiwidCI6IjEwMWRhNTg3LTE4NDMtNGY1Mi04YjhhLTE3YjA2OWM2NmQzMyIsImMiOjJ9)
