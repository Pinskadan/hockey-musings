# hockey-musings

Ice Hockey is my favorite sport, by far, and I am always interested in the weirdness 
of how Hockey is played and run. It's because of this that I'm dedicating some of my
educational time creating hypothetical situations and research through various tech programs.
So that's what this is.

This folder includes the following:
### NHL Live Standings
This Microsoft Excel file is a few things at once: 
  * On the left, a list of 1230 NHL games from the 2016-2017 season, with score and overtime status. Next to that is a category listing autofilled by Excel formula, dictating whether it was a regulation (3), overtime (2), or shootout (1) game.
  * Next to that, an excel formula listing the winning and losing team of each game.
  * From that given information, an entirely formula-generated pivot table of Total Wins, Total Losses, Games Played, Wins by category, Losses by category, points gained by those wins and losses according to the NHL rulebook, points remaining in the season for each team, and hypothetical points totals based on alternate systems (such as the one used by the KHL and the one suggested by hockey writer Andrew Berkshire).
  * An formula-generated listing of the playoff standings based on the current NHL setup of top three teams in each division plus two wild card teams per conference.
### Web.py
In order to help my excel file gain more data in real time, this (work-in-progress) script uses the Python module Beautiful Soup to grab data from the official NHL game sheets as they are updated, isolate the teams, score, and game status (regulation, OT, or SO) to add to an excel sheet. In the future, this will include every NHL game (thus the counter function in the code) and write the information to a CSV. That way, the Excel sheet can copy that info through VLOOKUP (I think...haven't tried that yet) and update the standings in real time.
