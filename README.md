# Artificial-Intelligence-Fantasy-Football

Objective:
We want the optimal players on our roster, maximizing our fantasy score, with the constraint of only having $200 spend on the players, and backup players only being able to attain half of their points earned. 

Fantasy Football scores are calculated by dividing the number of points earned by the price associated with the respective player. Thus, its best to create a team roster that yields the most points possible (keeping cost of player in mind. An optimal balance between the most points earned and the least price associated with each player.)


Explaining My Results:
The code was able to create a 15-player team roster with a starting lineup position labeled as : ‘Starters’, and 6 bench slots labeled as: ‘Backup’. The code prints the fantasy points earned by each optimal player in the roster. Additionally, a count of total price keeps track of the sum of money spent on each player (195.3), to yield a fantasy football score of 1813.4 
Project Write-up:
A person builds a team roster by handpicking 15 football players from a larger pool of players with varying position types. The same player cannot be listed twice in one 15 player roster. We want the most optimal players on our roster to maximize our fantasy score. Thus, a person should create a team roster that yields the most points possible. Here’s the catch: each football player with the opportunity to be drafted has a price associated with them, and a person only has a total of $200 total to spend on the roster. The team roster itself consists of a startling lineup, and 6 bench slots. The starting lineup has one Quarterback, three Wide receivers, two Running backs, one Tight-end, one Kicker, and one Defense. All starting lineup positions listed can only house a player of that type. The bench slots can house any player position type. The players who do not make in your starting lineup will fill the bench slots. Unlike the starting lineup, the bench slots only generate half of the total points the player earned



Libraries/Dependencies to Install: 

!pip install pandas
!pip install ortools
from ortools.linear_solver import pywraplp
import pandas as pd
from google.colab import files

data file is called: 'fantasy_football_data.csv'

