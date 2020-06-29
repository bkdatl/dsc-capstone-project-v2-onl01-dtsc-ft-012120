# Capstone Project Requirements

## Introduction

Baseball statistics have been kept for generation upon generations. With the plethora of data available certain metrics can be measured to determine and evaluate play of teams and individual players. The challenge in baseball is that while it is a team sport, during batting you end up with one batter versus an entire team. My original plan for this project was to use the Microsoft 'Trueskill' library to create individual player metrics of that player versus a particular opponent. However, that quickly grew outside my capabilities at this time as creating an evaluation metric for both the individual player verses the entire 9 players on the team was extremely difficult. If you do a web search for predictive models for baseball, the results are very limited, this is because baseball has so many variables. Evaluating individual player performance is difficult enough, however when you add the complexity of additional environmental factors, pitch selection, walk/K rates, just to name a few, the evaluations become increasingly complex and difficult to manage and get meaningful results from.


## Objectives

Create models to determine the viability of predicting baseball game outcomes. 
Create models to determine player WAR performance over a season. 


## Technical Project Requirements
Python 3.6 or better
os
pandas 
seaborn
matplotlib
numpy
sklearn
TrueSkill* 
* Trueskill not required for main project, still troubleshooting trueskill library and fucntionality

## Datasets
csv_files/atl_wins.csv
csv_files/team_stats.csv
csv_files/batting_stats.csv
csv_files/sp_stats.csv


## Glossary of Baseball Statistics 
Rk -- Rank
This is a count of the rows from top to bottom.
It is recalculated following the sorting of a column.
Gtm -- Season Game Number for Team
Click to see season stats through the
end of this game for this player.
Number in parentheses indicates number
of team games the player did not play in from one appearance to next.
Date -- A number in parentheses indicates which game of a doubleheader.
Click dates for box scores of games or standings on this day.
Rslt -- Game Result for Team
W - Win, L - Loss, T - Tie (for a suspended game)
PA -- Plate Appearances
When available, we use actual plate appearances from play-by-play game accounts
Otherwise estimated using AB + BB + HBP + SF + SH,
which excludes catcher interferences.
When this color click for a summary of each PA.
AB -- At Bats
R -- Runs Scored/Allowed
H -- Hits/Hits Allowed
2B -- Doubles Hit/Allowed
3B -- Triples Hit/Allowed
HR -- Home Runs Hit/Allowed
RBI -- Runs Batted In
BB -- Bases on Balls/Walks
IBB -- Intentional Bases on Balls
First tracked in 1955.
SO -- Strikeouts
HBP -- Times Hit by a Pitch.
SH -- Sacrifice Hits (Sacrifice Bunts)
SF -- Sacrifice Flies
First tracked in 1954.
ROE -- Reached On Error
Times a batter reached due to an error
DOES NOT include a fielder’s choice where no out was recorded.
GDP -- Double Plays Grounded Into
Only includes standard 6-4-3, 4-3, etc. double plays.
First tracked in 1933.
For gamelogs only in seasons we have play-by-play, we include triple plays as well.
All official seasonal totals do not include GITP's.
SB -- Stolen Bases
CS -- Caught Stealing
BA -- Hits/At Bats
For recent years, leaders need 3.1 PA
per team game played
Bold indicates highest BA using current stats
Gold means awarded title at end of year.
OBP -- (H + BB + HBP)/(At Bats + BB + HBP + SF)
For recent years, leaders need 3.1 PA
per team game played
SLG -- Total Bases/At Bats or
(1B + 2*2B + 3*3B + 4*HR)/AB
For recent years, leaders need 3.1 PA
per team game played
OPS -- On-Base + Slugging Percentages
For recent years, leaders need 3.1 PA
per team game played
LOB -- Runners Left On Base
'# '-- Number of Players Used in Game
Thr -- Handedness of the opposing starter
Opp. Starter (GmeSc) -- The starter for the opposition and the game score they earned.