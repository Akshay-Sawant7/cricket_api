# cricket_api
This application is for getting information of cricket matches through api
A Pythonic interface to cricbuzz, with options to get live scores, live commentary and scorecards.
Installation

pip install pycricbuzz
Features

Get information upcoming, live and recently concluded matches
series name
match status
venue
toss
match official
squads
Get mini scorecards for live matches
Batsman currently batting along with their scores,runs,fours,sixes etc.
Bowlers currently bowling along with their wickets,overs,maidens etc.
Summary of all the innings
Last three overs events
Current patnership and run rate
Commentary for live matches
Scorecard for live and past matches
Basic Usage

Import the pycricbuzz library.

from pycricbuzz import Cricbuzz
c = Cricbuzz()
Get all the matches(live,upcoming and recently finished matches)

print(c.matches())
Each match will have an attribute 'id'. Use this 'id' to get matchinfo, scorecard, brief score and commentary of matches.

Get information about a match

print(c.matchinfo(match['id']))
Get brief score of a match

print(c.livescore(match['id']))
Get scorecard of a match

print(c.scorecard(match['id']))
Get commentary of a match

print(c.commentary(match['id']))
