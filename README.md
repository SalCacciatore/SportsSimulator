This package allows a user to simulate the results of a sporting event using the statistics of two teams.

The inputs are the points per game average, points per game standard deviation, points allowed per game average and points allowed standard deviation for the home team, the same metrics for the visiting team, the homefield advantage and the point spread.

To begin, install the package.

Next, import "sportssim" (from sals_sports_simulator import sportssim).

Now, you can "create" you teams given the following parameters:
-Offense (average scoring per match)
-Offensive standard deviation (standard deviation of points per match)
-Defense (average scoring allowed per match)
-Defensive standard deviation (standard deviation of points allowed per match)

To create the team, use the following format:
YourTeam = sportssim.Team(Offense, offensive standard deviation, Defense, Defensive standard deviation).

Do the same for the team you are comparing this team to.

Finally, use the multisim function to run the simulations.

Multisim takes the inputs:
-Number of simulations
-Home team
-Away team
-Home Field advantage
-Point spread

For example, if Team A was playing at home in a sport with a 1.5-point home field advantage and was a 5-point favorite over Team B, you'd run the following code to generate 1000 simulations:

sportssim.multisim(1000,TeamA,TeamB,1.5,-5)


Credit: https://www.playingnumbers.com/2019/12/how-to-simulate-nba-games-in-python/
